# Урок 19. Основные виды СЗИ  

 ## ***Домашняя работа*** ##  
1) Установка ClamAV:  
  
![cav_install](images/cav_install.png)  

Далее останавливаем сервис командой sudo systemctl stop clamav-freshclam для обновления баз данных и вводим команду автообновления:
  
![update_virus_db](images/update_virus_db.png)  
  
Далее запускаем сервис:  
  
![start_service](images/start_service.png)  
  
Запуск сканирования в терминале:  
  
![scan](images/scan.png) 
  
Установка GUI вводом команды sudo apt install clamtk, обновление БД в GUI:  
  
![cl_gui](images/cl_gui.png)  
![update_gui_db](images/update_gui_db.png)  
  
Сканирование файла:  
  
![file_anal](images/file_anal.png) 



  
Настройка 2 fa путем добавления строки "auth required pam_google_authenticator.so" в файл /etc/pam.d/sshd c последующим перезапуском демона ssh и добавление возможности запроса кода аутентификации при входе в систему путем установления параметра ChallengeResponseAuthentication в положение yes:

![restart](images/restart.png)  
![settings](images/settings.png)  
  
Настройка Google Authenticator для генерации кодов TOTP путем установки параметров.Также нам представлен QR-code и секретный ключ:  

![google](images/google.png)  




  


