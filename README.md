# Raspberry PI

Le manguie a [m4tu5](https://github.com/m4tu5) que cuando fuera a europa me la comprara.

## RaspBMC

Lo descargue del [sitio oficial](http://www.raspberrypi.org/downloads). 
Fue muy simple de instalar, solo hay que volcarlo a la microSD y al iniciar se realiza todo el resto, preferiblemente tiene que estar conectada a internet.
Funciona muy bien.

_**Nota:** Arora browser se instalo como parte de una actualización pero no funciona :(_

## GPIO

![Puertos GPIO](GPIOs.png)

compile la herramientas para manejar en [bash los puertos GPIO](http://elinux.org/Rpi_Low-level_peripherals#Bash_shell_script.2C_using_sysafs.2C_part_of_the_raspbian_operating_system).
Como la experiencia fue muy simple solo tuve que usar ... pensé en ponerle una interfaz más amigable a algunos puestos del GPIO. 
Copiándome de la experiencia del [Gamepad universal](http://wiki.hackcoop.com.ar/Gamepad_universal) de [li-kun](https://github.com/li-kun) use fichas banana y un envase de plástico duro hecho cortado a mano.
Y los conectores de led de unas PCs viejas que sirvieron para conectar el GPIO a las fichas banana.

![Conexiones GPIO a Ficha Banana](Raspberrypi_pcb_overview_v04.png)
> 0, 1, 4, 7, 8, 9, 10, 11, 14, 15, 17, 18, 21, 22, 23, 24, 25 deberia usar solo estos puertos

![foto del modelo terminado](2013-12-26-015233.jpg)
![foto del modelo terminado](2013-12-26-015347.jpg)

Aunque la salida de sonido no es análoga puede generar sonidos usando una modificación de `blink.c` para generar un pseudo-pwm.

### Pendientes

* Pull-up en los puertos
* ~~Probarlo bien~~
 * algunos puertos no andan, por que son internos del raspberry(24,25)
* Ejemplos de programación

## Material de terceros

* https://upload.wikimedia.org/wikipedia/commons/a/af/Raspberrypi_pcb_overview_v04.svg
