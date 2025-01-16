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

2) Установка YARA.

![yara](images/yara_install.png)  

Предполагается, что злоумышник знает про папку с важными документами на нашем ПК. Для того, чтобы нанести ущерб нашей компании он создал 2 зловреда: 1 - .exe с обновлением
программы, которая имеется в нашем ПК, полученный посредством социальной инженерии через email от вегдора ПО; второй - скрипт, который попросил запустить и проанализировать наш "друг", который был взломан накануне. .exe - шифрует папку "Документы" по заданному ключу, а .py - также шифрует данную папку.  Hash данных файлов представлен ниже:  

![hash](images/hash.png)  

Проверка данных файлов с помощью написанных правил YARA:  

![yara_check_1](images/yara_check_1.png)  
![yara_check_2](images/yara_check_2.png)



  



  


