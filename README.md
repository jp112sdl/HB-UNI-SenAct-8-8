# HB-UNI-SenAct-8-8
## Universal 8fach-Aktor und 8fach-Sender (Taster [-RC] oder Schließerkontakt [-SC]) für HomeMatic

- Aufbau grundlegend wie [HB-UNI-SenAct-4-4](https://github.com/jp112sdl/HB-UNI-SenAct-4-4)
- Ansteuerung der Ausgänge erfolgt jedoch über einen PCF8574(A) Port Expander
  - Anpassung der I2C Adresse im Sketch ist ggf. notwendig:
  - `#define PCF8574_ADDRESS 0x38` bei Verwendung eines PCF8574A **(Default)**
  - `#define PCF8574_ADDRESS 0x20` bei Verwendung eines PCF8574
- Tastereingänge sind direkt am Arduino Pro Mini
Es wird die aktuellste Version (mind. V 1.25) des [JP-HB-Devices Addon](https://github.com/jp112sdl/JP-HB-Devices-addon/releases/latest) benötigt!
