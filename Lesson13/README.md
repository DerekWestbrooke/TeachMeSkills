# Урок 13. Безопасность Windows OS

## ***Домашнее задание:*** ##  

1. Заходим в ServerManager. Далее Manage->Add roles and features, устанавливаем на Role-based or features-based installation, далее выбираем сервер, указываем AD Domain Service, указываем доменное имя и нажимаем установку:  
  
![sm](images/sm.png)  

![set1](images/set1.png)  

![set2](images/set2.png)  

![set3](images/set3.png)  

![set4](images/set4.png)  
  
Меняем имя компьютера на ns1. Результат по первому пункту:

![names](images/names.png)  

2) Устанаваливаем DNS-сервер таким же образом, как и AD: Manage->Add roles and features, устанавливаем на Role-based or features-based installation, далее выбираем сервер, указываем DNS Server, и нажимаем установку. Переходим в Tools, DNS, выбираем FORWARD LOOKUPZONES и основной домен (в моем случае - westbrooke.local). Там создаем записи через New Record, Host A, далее запполняем форму с указанием имени хоста и его IP:

![kali_aaa](images/kali_aaa.png)  

![kali_note](images/kali_note.png)  

Также заполняем и для ubuntu (host - ubuntu, ip - 10.10.0.10). Далее пингуем доменное имя на примере ubuntu:  

![w-u](images/w-u.png)  

![w-k](images/w-k.png)  

![dig_u](images/dig_u.png)  

![dig_k](images/dig_k.png)




  
