# Robot_JohhnyV2

## Información de los motores Dynamixel MX-28

### Protocolo de comunicación TTL (usa un conector de 3 pines) Half duplex 

Protocolo TTL: Realiza comunicaciones a traves de variaciones de voltaje (0-5V), es asincrono (no depende de una señal de reloj), utiliza 2 puertos de comunicación TX(Transmite datos) y RX(Recibe datos). Entre 2 dispositivos se trabaja con la modalidad maestro-esclavo, es decir en este protocolo solo uno de los dispositvcos puede tener el control de la línea de comunicación.

Sensor de posición: Enconder absoluto
Modos de operación: Wheel mode and Joint mode
Resolución: 4096 pulsos/rev
Tasa de baudios: 7.834[bps] - 3[Mbps]
Retroalimentación: Posición, temperatura, carga, voltaje de entrada, etc.


Configuracion del entorno de Red 

cd /etc/netplan/
sudo nano 50-cloud-init.yaml

sudo netplan try
sudo netplan apply




