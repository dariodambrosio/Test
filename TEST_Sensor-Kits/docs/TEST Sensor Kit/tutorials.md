# 📚 Sensor Kits – Tutorials & Projekte

Willkommen im Projektbereich!  
Hier findest du praxisnahe Beispiele zum direkten Nachbauen mit unseren Sensor Kits. Die Anleitungen enthalten Schaltungen, Beispielcode und Erweiterungsideen.

---

## 🌡️ Temperatur und Luftfeuchtigkeit anzeigen

**Kit:** Basic / Pro  
**Sensor:** DHT22  
**Display:** OLED 0.96" I2C  
**Controller:** Arduino UNO

### 🛠️ Materialien

- DHT22 Sensor  
- OLED Display  
- Arduino UNO  
- Breadboard + Jumperkabel

### 💡 Aufbau

```text
DHT22       Arduino
---------------------
VCC    ->   5V  
DATA   ->   D2  
GND    ->   GND  

OLED        Arduino
---------------------
VCC    ->   5V  
GND    ->   GND  
SCL    ->   A5  
SDA    ->   A4  
