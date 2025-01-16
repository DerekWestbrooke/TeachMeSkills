# Урок 18. Защита инфраструктуры приложений  

 ## ***Домашняя работа*** ##  
1) Установка ssh-server:  
  
![install_ssh_s](images/install_ssh_s.png)  

Установка 2FA:

![2FA](images/2fa.png)  
  
Настройка 2 fa путем добавления строки "auth required pam_google_authenticator.so" в файл /etc/pam.d/sshd c последующим перезапуском демона ssh и добавление возможности запроса кода аутентификации при входе в систему путем установления параметра ChallengeResponseAuthentication в положение yes:

![restart](images/restart.png)  
![settings](images/settings.png)  
  
Настройка Google Authenticator для генерации кодов TOTP путем установки параметров.Также нам представлен QR-code и секретный ключ:  

![google](images/google.png)  




  


