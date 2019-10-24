# Robótica en educación Primaria: Scratch, Echidna y Makey-makey

## CEP Priego-Montilla

## Octubre de 2019

### José Antonio Vacas @javacasm

![CCbySA](./images/Licencia_CC.png)

## http://bit.ly/RPPriego

# [Echidna](http://echidna.es/)

Echidna es un escudo/shield de Arduino y que incluye mucho sensores y componentes ya soldados, de manera que podemos trabajar con Arduino sin necesidad de saber manipular la electrónica necesaria

Ha sido diseñado por unos profes: Jorge Lobo, José Pujol y Xavier Rosas

![Echidna](./images/echidnashield.png)


![Echidna esquema](./images/EschidnaShield-esquema.png)

## Entornos de programación

Se puede programar con cualquier entorno donde se programe Arduino (IDE, Ardublocks, biblock, mBlock, etc.)

[MakeBlock](https://ide.mblock.cc/)

[Bitbloq](https://bitbloq.bq.com)

## Programación

### Usaremos el IDE de mBlock https://ide.mblock.cc 

Soporta Bluetooth Controller, Codey Rocky, HaloCode, mBot, MotionBlock, Neuron, mBot Ranger, Ultimate 2.0, Arduino Uno, Arduino Mega2560, Nova Pi, MegaPi Pro


### Necesitamos el mblock mlink  https://www.mblock.cc/en-us/download/

![mlink instalar](./images/InstalarMlink.png)

[Guía de instalación](https://www.mblock.cc/doc/en/basics/mlink-quick-start-guide.html#mlink-quick-start-guide)

### Ejecutamos mLink

En windows
 
![mLink icon](https://www.mblock.cc/doc/en/basics/images/mlink-4.png)

En osX

![mlink osX](https://www.mblock.cc/doc/en/basics/images/mlink-8.png)

En linux

    sudo mblock-mlink start
    
    
    
### Seleccionamos el dispositivo

Y pulsamos conectar

![conectar](https://www.mblock.cc/doc/en/basics/images/chromebook-7.png)

## Ejemplos

### Hello LED!!

Haremos parpadear el led Rojo

![Hello LED!](./images/HelloLed!.png)

[Proyecto](https://planet.mblock.cc/project/102035)

### Led RGB

![Mezcla colores](./images/Colores-MezclaRGB.jpeg)

[Selector de colores](https://htmlcolorcodes.com/es/)

Utilizamos el led RGB (conectado a lo pines digitales 9,5,6)

Y a la vez haremos que se vayan leyendo los colores en inglés, con la extensión Text To Speech.

Parece que hay algo de desajuste. Tendremos que mejorar la comunicación con ... mensajes    

![Programa Arduino](./images/Colores-Arduino.png)
![Programa Osito](./images/Colores-Osito.png)

[Programa](https://planet.mblock.cc/project/projectshare/101707)


### Nivel de luz

Usaremos los 3 leds de colores para indicar el nivel de luz:
* Rojo: luz baja
* Amarillo: nivel de luz medio
* Verde: luz suficiente

![NivelLuminoso](./images/NivelLuminoso.png)

[Proyecto](https://planet.mblock.cc/project/102785)

### Controlando el movimiento de Osito con el Joystick

Sabemos que el joystick está conectado a los pines analógicos A0 (eje x) y A1 (eje y). Vamos a ver los valores que encontramos.

Vemos como la lectura de los sensores analógicos fluctúa, es algo normal. Un hardware más preciso (y caro) tendría una lectura más exacta.

Creamos una variables x e y para Arduino y comprobamos los valores del joystick

![Joystick Arduino](./images/Joystick-Arduino.png)

![Joystick Osito](./images/Joystick-Osito.png)

[Proyecto](https://planet.mblock.cc/project/102052) 

### Controlar el movimiento de Osito con el acelerómetro

Modificar el ejemplo anterior para que controlemos a Osito con el acelerómetro

Pista: modificar el programa para usar el sensor adecuado

[Proyecto](https://planet.mblock.cc/project/102061)

### Controlamos la posición de 2 servos usando el joystick

![2xServos-Joystick](./images/2xServos-Joystick.png)

Controlamos la posición de 2 servos usando el joystick

[Proyecto](https://planet.mblock.cc/project/102156)

### Haciendo ruído

Veamos como hacer sonido con el zumbador: activamos y desactivamos rápidamente

Un poquito de física sobre frecuencias y periodos....

![Frecuencias y periosdos](./images/frecuenciaYperiodo.png)

![Sonido 440Hz Original](./images/Sonido440HzOrig.png)

Veremos que en modo "en vivo" no es suficientemente rápido y tenemos que irnos a modo Arduino

![Sonido 440Hz](./images/Sonido440.png)

[Programa](https://planet.mblock.cc/project/102073)

Ejercicio: Ver como cambia el movimiento al enviar el programa anterior de los servos en modo Arduino

## Más prácticas

1. [Puesta en marcha](https://docs.google.com/presentation/d/1NYOY1towdBt71wKYxt_jLBhTYYsIkpvGYDGA5utdINU/pub?start=false&loop=false&delayms=3000&slide=id.g1d7972fb46_0_58)
2. [Señales digitales - Morse](https://docs.google.com/presentation/d/e/2PACX-1vRHtGnZqarnsH3gNz8kqsuLxwNFLnBqoz2RtxcgU1ee6OVge2knzkpjZ1kya5J7RGla3NIzE5lV3HL1/pub?start=false&loop=false&delayms=3000&slide=id.g5e67d40e2f_0_222)
3. [Sensores analogicos](https://docs.google.com/presentation/d/e/2PACX-1vQl1u6t4B8fF9CyEKpBzi6zhQfons3dBTU3hWeYcLKatMsjhb707f7ea7WMNLnrVktEjDrQGy8ZD-5l/pub?start=false&loop=false&delayms=3000&slide=id.g22833a02f3_0_0)
4. [Pulsadores y condicionales - Ejemplo de Quiz](https://docs.google.com/presentation/d/e/2PACX-1vTPm4czxn9bT9avK2kgZA-RMyvMCv9TGb5pXj3y3I5W7a4qFAO077c0neYWXSbvUYp1NCmHUIzXBhN3/pub?start=false&loop=false&delayms=3000&slide=id.p)
5. [Modo Makey-Makey](https://docs.google.com/presentation/d/1HBhSaJAErg5IXbYpjDPuCQDJVzoYAWjmVivMPmMvfrI/pub?start=false&loop=false&delayms=3000&slide=id.g22833a02f3_0_0)
6. [Luces psicodélicas](https://catedu.gitbooks.io/programa-arduino-con-echidna/content/tema_2_salidas_de_echidna/21_luces.html)
6.5 [Servo](https://catedu.gitbooks.io/programa-arduino-con-echidna/content/55-rele.html)
7. [TeleSketch](https://catedu.gitbooks.io/programa-arduino-con-echidna/content/3_entradas_de_echidna/33_joystick/331-telesketch.html)
8. [Bluetooth](https://catedu.gitbooks.io/programa-arduino-con-echidna/content/5_extensiones/51_bluetooth.html)
9. [Ultrasonidos](https://catedu.gitbooks.io/programa-arduino-con-echidna/content/5_extensiones/54-ultrasonidos.html)

## Documentación

[Documentación de Javier Quintana para Catedu](https://catedu.gitbooks.io/programa-arduino-con-echidna/content/) [PDF](https://legacy.gitbook.com/download/pdf/book/catedu/programa-arduino-con-echidna) [Ejemplos](https://github.com/JavierQuintana/Echidna)

[Echidna Shield para educación](https://www.programoergosum.com/cursos-online/robotica-educativa/604-robotica-educativa-con-echidna-shield/introduccion)
