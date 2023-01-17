# Esp32-Sensor-Interno-De-Efecto-Hall

code

void setup() {
  Serial.begin(115200);
}

void loop() {
  Serial.println("-250," + String(hallRead()) + ",250");
  delay(25);
}

el sensor de efecto hall detecta los campos magneticos y la posicion de ellos.
Los autos utilizan el sensor de efecto hall para detectar que el cinturon este puesto en el vehiculo
