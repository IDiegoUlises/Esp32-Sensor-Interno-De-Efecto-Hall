# Esp32 Sensor Interno De Efecto Hall

### Codigo
```c++
#include <driver/adc.h>

//Se declara un variable para guardar el valor del sensor
int sensor = 0;

void setup() 
{
  //Inicia el puerto serial
  Serial.begin(9600);
}

void loop() 
{
  //Realiza la lectura del sensor
  sensor = hall_sensor_read();

  //Imprime el valor del sensor
  Serial.println(sensor);
  
  //Retardo para no llenar la pantalla
  delay(500);
}

```
