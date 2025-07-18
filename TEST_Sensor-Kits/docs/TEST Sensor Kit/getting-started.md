# Erste Schritte

Willkommen zu deinem neuen Sensor Kit!  
Diese Anleitung hilft dir beim Einstieg.

## 1. Hardware vorbereiten

- Öffne das Kit und überprüfe den Lieferumfang
- Schließe dein Board (z. B. Arduino Uno) an deinen PC an

## 2. Software installieren

- Bibliotheken hinzufügen:
  - `Adafruit_Sensor`
  - `DHT`
  - `BME280`

## 3. Erstes Sensorprojekt

```cpp
#include <DHT.h>
DHT dht(2, DHT22); // DHT an Pin 2

void setup() {
  Serial.begin(9600);
  dht.begin();
}

void loop() {
  float temp = dht.readTemperature();
  Serial.println("Temp: " + String(temp));
  delay(1000);
}
