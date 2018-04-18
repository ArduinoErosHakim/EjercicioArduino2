# Práctica MarkDown 2 by *Eros* & *Hakim*
___

### Componentes:
- Tres leds
- Una protoboard o breadboard
- Una placa Arduino R3
___
### Código fuente
~~~C
// the setup routine runs once when you press reset:
void setup() {
  // initialize the digital pin as an output.

  for ( int i = 11 ; i <= 13 ; i++)
  {
    pinMode(i, OUTPUT);
  }

}

// the loop routine runs over and over again forever:
void loop() {
  
  for (int i=11 ; i <= 13 ; i++)
  {
       digitalWrite( i , HIGH) ;
       delay (200) ;
       digitalWrite( i , LOW);
       delay (200) ;
  }
}

~~~
___
### Imágenes
![Imagen Arduino](D:\DAM\Entornos/de/Desarrollo\Tercera/Evaluación\arduino.jpg "Arduino")
___
### Funcionalidad
Realiza intervalos de luz sostenida de hasta cuatro segundos para reiniciarse de nuevo tras un segundo inactivo. 