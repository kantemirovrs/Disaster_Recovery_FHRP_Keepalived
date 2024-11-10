# Disaster_Recovery_FHRP_Keepalived-Кантемиров Роман
#-----
#Задание 1
#скриншот, где виден процесс настройки маршрутизатора
![z11.png](https://github.com/kantemirovrs/Disaster_Recovery_FHRP_Keepalived/blob/main/img/z11.png)
#Для проверки корректности настройки, разорвите один из кабелей между одним из маршрутизаторов и Switch0 и запустите ping между PC0 и Server0.
![z12.png](https://github.com/kantemirovrs/Disaster_Recovery_FHRP_Keepalived/blob/main/img/z12.png)


#-----
#Задание 2
#Два сервера: MASTER (192.168.0.108) BACKUP (192.168.0.103) virtIP (192.168.0.101)
#
# скрин до отключения nginx на MASTER (192.168.0.108) - web-сервер 192.168.0.101 доступен на MASTER (192.168.0.108)
 
![z21.png](https://github.com/kantemirovrs/Disaster_Recovery_FHRP_Keepalived/blob/main/img/z21.png)

#Конфиг /etc/keepalived/keepalived.conf, скрипт, состояние демона keepalived после отключения nginx на MASTER (192.168.0.108) 

![z24.png](https://github.com/kantemirovrs/Disaster_Recovery_FHRP_Keepalived/blob/main/img/z24.png)

#Скрин после отключения nginx на MASTER (192.168.0.108) - web-сервер 192.168.0.101 доступен на BACKUP (192.168.0.103) 

![z25.png](https://github.com/kantemirovrs/Disaster_Recovery_FHRP_Keepalived/blob/main/img/z25.png)
