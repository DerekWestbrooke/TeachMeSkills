# Урок 22. Vulnerability Assessment 

 ## ***Домашняя работа*** ##  
1) Установка OpenVAS и запсук службы:  
  
![install_ov](images/install_ov.png)  

Проверка состояния службы:

![ov_on](images/ov_on.png)  

Запуск настройки gvm командой "sudo gvm-setup". По окончании отобразиться логин и пароль, которые надо запомнить! Далее проверяем установку командой "sudo gvm-check-setup", доустанавливаем необходимые пакеты.

![passw](images/passw.png)  
  
Когда установка закончится и все необходимое будет установлено, отобразится строка:  

![setup](images/setup.png) 
  
Включение помощника:  

![helper](images/helper.png)  

Создание новых правил для FIN и SYN путем добавления текстового файла в папку /etc/suricata/rules:  

![rules](images/rules.png)  

Обновление службы:  

![updating](images/updating.png)

Далее переходим в браузер, вводим адрес из документации, а также данные для входа, которые мы запомнили. После этого мы увидим рабочее пространство:  

![launch_web](images/launch_web.png)  

![entrance](images/entrance.png) 

Для тестирования данной службы просканируем ВМ UBUNTU. Для этого сформируем задание. Результаты следующие:  
  
![results_1](images/results_1.png)  

![results_2](images/results_2.png)

2) Установка PatrOwl. Создаем папку, в которую клонируем проект:

![install_patr2](images/install_patr.png)  

Далее развертываем backendс помощью Docker-compose:  

![set_1](images/set_1.png)  

![set_2](images/set_2.png)  

Далее заходим в браузер, вводим "http://localhost:8083/", после чего вводим учетные данные (логин: admin, пароль: Bonjour1).



  



