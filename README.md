# Robot_JohnnyV2

## Configuración en ROS


### Configuracion del entorno de Red 

cd /etc/netplan/
sudo nano 50-cloud-init.yaml

sudo netplan try
sudo netplan apply

### Conexión por ssh


### enviar un archivo desde mi pc a la raspberry via WIFI

scp ~/ros2_ws/src/dynamixel-workbench/dynamixel_workbench_controllers/src/move_dyn.cpp johnnyv2@192.168.0.100:~/ros2_ws/src/dynamixel-workbench/dynamixel_workbench_controllers/src/move_dyn.cpp 

## Información de los motores Dynamixel MX-28

### Protocolo de comunicación TTL -Half duplex (conector de 3 pines) 

 - TTL: Realiza comunicaciones a traves de variaciones de voltaje (0-5V), es asincrono (no depende de una señal de reloj), utiliza 2 puertos de comunicación TX(Transmite datos) y RX(Recibe datos). Entre 2 dispositivos se trabaja con la modalidad maestro-esclavo, es decir en este protocolo solo uno de los dispositvcos puede tener el control de la línea de comunicación.

### Características técnicas más relevantes

**Sensor de posición:** Enconder absoluto

**Modos de operación:** Wheel mode and Joint mode

**Resolución:** 4096 pulsos/rev

**Tasa de baudios:** 7.834[bps] - 3[Mbps]

**Retroalimentación:** Posición, temperatura, carga, voltaje de entrada, etc.

## comando scp
https://dabeen.medium.com/tips-using-scp-with-password-bd2ed6d9aecd

#Comandos de la raspberry
shutdown now -Para apagar la raspberry
reboot - para reiniciarla

sudo dmesg | grep tty - para visualizar el nombre de los puertos seriales conectados

