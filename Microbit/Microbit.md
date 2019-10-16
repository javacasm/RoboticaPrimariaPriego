# BBC-microbit

![microbit front](http://microbit.org/images/microbit-front.png)
![microbit back](http://microbit.org/images/microbit-back.png)

[Fundación microbit](http://microbit.org/es/)

[Microbit es totalmente opensource](https://www.microbit.co.uk/open_source)

[Github de microbit](https://github.com/bbcmicrobit)

### [Hardware](http://microbit.org/es/hardware/)


![hardware](http://microbit.org/images/microbit-hardware.png)
![pinout](https://cdn-blog.adafruit.com/uploads/2017/03/microbit_pinout_v10.png)

![pinout2](https://microbit.org/images/microbit-pins.jpg)

#### Alimentación

Funciona a 3V y dispone de un conector de bateria y de alimentación por USB (MicroUSB)


#### Micro
ARM M0 (32 bits) a 16MHz con 16k de RAM


#### [Sensores](https://microbit.org/guide/features/)

* Acelerómetro
* Brújula
* 2 Botones
* 3 entradas analógicas (0,1,2)
* 20 pines I/O


#### Comunicaciones

[Bluetooth](http://microbit.org/es/mobile/) de bajo consumo

Comunicaciones via radio entre distintas microbits

[App microbit](https://play.google.com/store/apps/details?id=com.samsung.microbit&hl=es) Nos permite interaccionar con la placa e incluso programarla


#### Leds

25 (5x5) leds programables individualmente

### Programación

[Revisión sobre las diferentes plataformas](https://hackaday.com/2017/12/02/exploring-the-bbc-microbit-software-stack/)

[Programando con bloques](https://pxt.microbit.org/?lang=es)

[Programando en python](http://python.microbit.org/)

[Python en Mibrobit](https://www.python.org/community/microbit/)

[Programando con el IDE de Arduino](https://learn.adafruit.com/use-micro-bit-with-arduino?view=all)

[Flappy bird en python](https://www.elecfreaks.com/12454.html)

### Dónde comprarlo

[Revendedores](http://microbit.org/es/resellers/)

[También en Amazon](https://www.amazon.es/BBC-MB80-Micro-Bit/dp/B01G8WUGWU/ref=sr_1_2?ie=UTF8&qid=1492513787&sr=8-2&keywords=microbit)


Complementos/shields

[Placa adaptadora 3.3v/5v y de fácil conexión de sensores](https://www.elecfreaks.com/12396.html)

### Robots

http://www.instructables.com/id/Remote-Controlled-Microbit-Robot/

![robot](https://cdn.instructables.com/F0W/1HA0/J30ST2ON/F0W1HA0J30ST2ON.LARGE.jpg)

#### [MaQueen](./MaQueen.md)

![Maqueen](https://raw.githubusercontent.com/DFRobot/DFRobotMediaWikiImage/master/Image/ROB0148Maqueen.jpg)


### Documentación

[Getting started](http://microbit.org/es/start/)

[Placa conexión con octupus](https://www.elecfreaks.com/12396.html)

[Usando la Brújula](https://www.elecfreaks.com/12412.html)

[Arcade in javascript](https://www.elecfreaks.com/12416.html)

### Recursos

[Nice review](https://www.youtube.com/watch?v=7qnSsc54bEQ)
* Usar  url sencillas y que estén visibles
* CPU https://en.wikipedia.org/wiki/Micro_Bit#Hardware
        Nordic nRF51822 – 16 MHz 32-bit ARM Cortex-M0 microcontroller, 256 KB flash memory, 16 KB static ram
 
Permite usar Batería con voltaje entre  https://support.microbit.org/support/solutions/articles/19000013982-how-do-i-power-my-micro-bit-

* Sensor de temperatura está en la CPU (https://microbit.org/es/guide/temperature/)

No necesitamos instalar nada, funciona via web y en tablet/móviles  

Se puede programar con bloques, javascript, python, C++ de Arduino...

# Programación con bloques https://makecode.microbit.org/

El simulador es interactivo y cambia la imagen del simulador a medida que usamos diferentes bloques

Los programas se guardan por defecto en nuestro navegador

Seleccionamos el idioma

![language](./images/SelecionarIdioma.png)

La pantalla: 
* A la izquierda, Podemos simular nuestro programa
* Centor las paletas de bloques
* Bloques de mi programa

![inicio](./images/Incio_bloques.png)

Añadir nuestros bloques en onStart (para que se ejecute al principio) o forever (para que se ejecute repetitivamente)

EJEMPLO [HOLA MUNDO](https://makecode.microbit.org/_MfyHdrLXVWqL)

![HolaMundo](./images/HolaMundo.png)

Podemos cambiar el nombre
 
Una vez que tenemos un programa vamos a reprogramar la Microbit

1. Conectamos el microbit
1. Aparece una unidad llamada Microbit
1. Descargamos el programa
1. Lo copiamos a la unidad Microbit (veremos como parpadea el led naranja)
(En un tablet o móvil necesitaremos un cable OTG)

Usamos el sensor de temperatura (que está en la CPU con lo que no es muy preciso)


EJEMPLO de temperatura
1. Mostrar temperatura
1. Mostrar la temperatura en forma de barra

[Control de temperatura](https://makecode.microbit.org/_LesCE2h70PAT)

![ControlTemperatura](./images/ControlTemperatura.png)

EJEMPLO: Control de iluminación digital y analógico


[Control de iluminación](https://makecode.microbit.org/_YqD3MePtK6gU)

![Control iluminación](./images/ControlIluminacion.png)



[Control de iluminación II](https://makecode.microbit.org/_7ayKTtKvXFcc)

![ControlIluminacionII](./images/ControlIluminacionII.png)

[ControlIluminacion III](https://makecode.microbit.org/_TVJAFy9mjJ3Y)

![ControlIluminacion2](./images/ControlIluminacionIII.png)

## Eventos

Pulsaciones de botones o cambios de pines, agitado

EJEMPLO: [¿a quién le toca?](https://makecode.microbit.org/_f9EhoRAp1eoR)
* boton A incrementa
* B decrementa 
* agitado pone número aleatorio

![A quien le toca](./images/AquienLeToca.png)

## Juegos

Hay una paleta de juegos que incluyen sprites, puntuaciones, etc

Los leds se direccionan así
(0,0) ..... (4,0)
...          ...
(0,4) ..... (4,4)

EJEMPLO: marcianitos simples

EJEMPLO: [piedra, papel o tijera](https://makecode.microbit.org/_0Xi5xA7gweK5)

![Piedra Papel Tijera](./images/PiedraPapelTijera.png)

EJEMPLO: dado digital

### Extensiones

Permiten usar extensiones que añaden más bloques 


PROYECTO termostato: los botones fijan la temperatura objetivo y la otra barra nos muestra la temperatura actual

PROYECTO maquinilla de numeros (innalámbrica)



# TODO

¿Recuperar programas de otro navegador?
Trabajar con la comunicacion serie
    
