# Урок 20. Основные виды СЗИ  

 ## ***Домашняя работа*** ##  
1) Установка Suricata:  
  
![install](images/install.png)  

Запуск Suricata:

![start](images/start.png)  
  
Обновление правил Suricata:  

![update](images/update.png)  

Создание новых правил для FIN и SYN путем добавления текстового файла в папку /etc/suricata/rules:  

![rules](images/rules.png)  

Обновление правил Suricata с учетом новых:  

![new_rule_update](images/new_rule_update.png)  

Перезапуск Suricata:

![restart](images/restart.png)  

Для тестирования работы Suricata установим h3pings на ВМ Ubuntu, с которой будем генерировать Syn-пакеты и отправлять их на ВМ Kali Linux:  

![h3pings](images/h3pings.png)  

Открываем файл логов Suricata с помощью jq и видим следующую запись,  в котором и отображается информация по перехвату Syn-пакета с указанием адресов, портов и протокола:  

![SYN](images/SYN.png)  


  


