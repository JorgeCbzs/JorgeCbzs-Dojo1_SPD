Ejemplo Documentación Dojos
Tinkercad

Integrantes
- Nicolas Dekker
- Ivo Curto
- Tobias Esquivel
- Jorge Cabezas
- Silvina Gauto
- Alvaro Braddy Calla Huangal
Proyecto: Contador binario.
Tinkercad

Descripción
Este programa controla un semáforo con dos luces de cada color (rojo, amarillo y verde) y un sonido para personas no videntes mientras la luz roja está encendida. 

Al principio se definen las constantes para los pines de los LEDs y el piezo. Tambien se establecen las variables para la duración de cada color del semáforo y para la frecuencia y duración del tono del piezo.

En la función "setup" se configuran los pines como entradas o salidas. En la función "loop" se maneja el patrón del semáforo y del pitido para no videntes. Primero se encienden los LEDs verdes por 5 segundos, luego los amarillos por 3 segundos y al final los LEDs rojos por 5 segundos con el sonido del piezo emitiendo dos pitidos por segundo.

Las funciones "encenderLed" y "apagarLed" sirven para encender y apagar los LEDs y son llamadas en la función "loop". La función "tone" sirve para generar un tono en el piezo y la función "noTone" para frenarlo.

Función principal
Estas funciones son las que se encargan de encender y apagar los leds

LEDROJAUNO , LEDROJADOS , LEDAMARILLAUNO , LEDAMARILLADOS , LEDVERDEUNO LEDVERDEDOS son #define que utilizamos para agregar los leds, asociandolo a pines de la placa arduino.

Tanto en la funcion encenderLed() como apagarLed() les pasamos por parametro dos luces leds (que son las que representarian un color
especifico del semaforo) y luego solo en la primera, el parametro tiempoEncendido que indicara cuanto tiempo queremos tomar al llamar a la funcion
delay() 

Ambas funciones usan la funcion digitalWrite() para controlar el estado de los pines de los leds (HIGH o LOW)


~ C++ (lenguaje en el que esta escrito)
void encenderLed(int led, int led2, int tiempoEncendido)
{
  digitalWrite(led, HIGH);
  digitalWrite(led2, HIGH);
  delay(tiempoEncendido);
}

void apagarLed(int led, int led2)
{
  digitalWrite(led, LOW);
  digitalWrite(led2, LOW);
}

🤖 Link al proyecto
https://www.tinkercad.com/things/4wSdNkLHMXV-dojo-1-primer-nivel/editel?sharecode=YGI5gMndS80Kb3AOLPkKdhnGCsdrxWjLDz4wGpRWCaQ
📺 Link al video del proceso
video
Fuentes
Consejos para documentar.

Lenguaje Markdown.

Markdown Cheatsheet.

Tutorial.

Emojis.

