# Урок 17. Защита инфраструктуры приложений  

 ## ***Домашняя работа*** ##  
1) Установка docker командой sudo apt intall docker и проверка работоспособности.    
  
![test](images/test.png)  

Установка Ubuntu и проверка контрольной суммы скаченной и эталонной версии:  
  
![image_ubuntu](images/image_ubuntu.PNG)  
![comparing](images/comparing.png)  

Просмотр всех установленных образов:  

![images](images/images.png) 

Добавление пользователя в группу docker для запуска без sudo  и результат:  

![launch](images/launch.png)  
![without_sudo](images/without_sudo.png)  

Вход в контейнер и результат вывода команды whoami:  

![whoami](images/whoami.png)  

Для добавления нового пользователя в контейнер необходимо написать Dockerfile, который будет брать за основу текущее изображение и добавить в него пользователя. Файл
, построение образа и результат команды whoami внутри контейнера приведен ниже:

![adduser](images/adduser.png)  
![new_ubuntu](images/new_ubuntu.png)  
![tms_user](images/tms_user.png)  

Сканирование контейнера с помощью trivy:  

![trivy](images/trivy.png)  

По результатам сканирование видны 6 узвимостей, из которых 5 низкого уровня и 1 среднего. В таблице приведены их названия, классификация и описание.
















