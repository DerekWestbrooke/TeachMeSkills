# Урок 26. Scripting  

 ## ***Домашняя работа*** ##  
1) Данный скрипт install.sh устанавливает пакеты curl, wget, snap по желанию пользователя. При этом функция установки пакета func.sh вынесена в отдельный скрипт. Ниже приведен код скриптов install.sh и func.sh:  
* install.sh  
  
![install](images/install.png)  

* func.sh

![func](images/func.png)  

Далее данным скриптам был добавлено разрешение на исполнение:  
* install.sh  
  
![install_chmod](images/chmod_install.png)  

* func.sh

![func_chmod](images/chmod_func.png)  

Результат выполнения кода приведен ниже:

![result](images/script.png)  

2) Данный скрипт test.ps1 собирает информацию о БИОСе, процессоре, ОС, подключенных USB-устройств, а также запускает программуисходя из пути, введеного пользователем, при этом проверяя существование пути.
Код скрипта представлен ниже:

![ps_script](images/ps_script.png) 

Далее запускаем скрипт из комндной строки PowerShell, при этом разрешая исполнения путем добавления специального флага:  

![ps_command](images/ps_command.png)  

Результаты исполнения скрипта представлены ниже:  
![result1](images/result1.png)  
![result2](images/result2.png)  
![result3](images/result3.png)
![result4](images/result4.png)
