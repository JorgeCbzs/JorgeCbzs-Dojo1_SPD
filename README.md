# Ejemplo Documentación Dojos
![Tinkercad](./img/ArduinoTinkercad.jpg)


## Integrantes 
- Nicolas Dekker
- Ivo Curto
- Tobias Esquivel
- Jorge Cabezas
- Silvina Gauto
- Alvaro Braddy Calla Huangal  


## Proyecto: Semaforo con sonido

## Descripción
Este programa controla un semáforo con dos luces de cada color (rojo, amarillo y verde) y un sonido para personas no videntes mientras la luz roja está encendida.

Al principio se definen las constantes para los pines de los LEDs y el piezo. Tambien se establecen las variables para la duración de cada color del semáforo y para la frecuencia y duración del tono del piezo.

En la función "setup" se configuran los pines como entradas o salidas. En la función "loop" se maneja el patrón del semáforo y del pitido para no videntes. Primero se encienden los LEDs verdes por 5 segundos, luego los amarillos por 3 segundos y al final los LEDs rojos por 5 segundos con el sonido del piezo emitiendo dos pitidos por segundo.

Las funciones "encenderLed" y "apagarLed" sirven para encender y apagar los LEDs y son llamadas en la función "loop". La función "tone" sirve para generar un tono en el piezo y la función "noTone" para frenarlo.

## Función principal
Estas funciones son las que se encargan de encender y apagar los leds

LED_ROJA_UNO , LED_ROJA_DOS , LED_AMARILLA_UNO , LED_AMARILLA_DOS , LED_VERDE_UNO LED_VERDE_DOS son #define que utilizamos para agregar los leds, asociandolo a pines de la placa arduino.

Tanto en la funcion encenderLed() como apagarLed() les pasamos por parametro dos luces leds (que son las que representarian un color especifico del semaforo) y luego solo en la primera, el parametro tiempoEncendido que indicara cuanto tiempo queremos tomar al llamar a la funcion delay()

Ambas funciones usan la funcion digitalWrite() para controlar el estado de los pines de los leds (HIGH o LOW)

~ C++ (lenguaje en el que esta escrito) void encenderLed(int led, int led2, int tiempoEncendido) { digitalWrite(led, HIGH); digitalWrite(led2, HIGH); delay(tiempoEncendido); }

void apagarLed(int led, int led2) { digitalWrite(led, LOW); digitalWrite(led2, LOW); }
~~~

## :robot: Link al proyecto
- [proyecto](https://www.tinkercad.com/things/4wSdNkLHMXV-dojo-1-primer-nivel/editel?sharecode=YGI5gMndS80Kb3AOLPkKdhnGCsdrxWjLDz4wGpRWCaQ)
## :tv: Link al video del proceso
- [video](https://www.youtube.com/watch?v=VyGjE8kx-O0)

---
### Fuentes
- [Consejos para documentar](https://www.sohamkamani.com/how-to-write-good-documentation/#architecture-documentation).

- [Lenguaje Markdown](https://markdown.es/sintaxis-markdown/#linkauto).

- [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

- [Tutorial](https://www.youtube.com/watch?v=oxaH9CFpeEE).

- [Emojis](https://gist.github.com/rxaviers/7360908).

---