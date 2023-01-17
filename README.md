# Esp32-Sensor-Interno-De-Efecto-Hall

code

void setup() {
  Serial.begin(115200);
}

void loop() {
  Serial.println("-250," + String(hallRead()) + ",250");
  delay(25);
}
