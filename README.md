# ESP32-S3-Custom-DevBoard

A custom ESP32-S3 development board featuring USB-C connectivity, Li-Ion battery charging, buck-boost power regulation, RGB status indication, and expansion support for future sensor integration.

---

## Component Description

### ESP32-S3-MINI-1-N8
The ESP32-S3-MINI-1-N8 serves as the main microcontroller of the board. It provides Wi-Fi and Bluetooth connectivity, USB communication support, GPIO interfaces, and executes the firmware controlling the entire system.

**Functions:**
- Wireless communication
- USB communication
- Data processing
- GPIO control
- Future sensor interfacing

---

### USB-C Connector
The USB-C connector provides power input and allows programming and communication between the ESP32 and a computer.

**Functions:**
- Power input
- Firmware uploading
- Serial communication
- Battery charging source

---

### MCP73831 Battery Charger
The MCP73831 is a dedicated Li-Ion battery charging IC used to safely charge a single-cell lithium-ion battery from the USB-C power source.

**Functions:**
- Battery charging
- Charge current regulation
- Battery management
- Charging protection

---

### Li-Ion Battery Connector
The battery connector provides an interface for connecting a rechargeable single-cell lithium-ion battery.

**Functions:**
- Portable operation
- Energy storage
- Backup power source

---

### TPS63001 Buck-Boost Converter
The TPS63001 converts the varying battery voltage into a stable 3.3V supply required by the ESP32 and other onboard components.

**Functions:**
- Voltage regulation
- Battery voltage conversion
- Stable 3.3V generation
- Power efficiency optimization

---

### ESD7104MUTAG ESD Protection IC
The ESD protection device protects the USB data lines from electrostatic discharge and voltage spikes.

**Functions:**
- USB protection
- Static discharge protection
- Transient voltage suppression

---

### WS2812B RGB LED
The WS2812B is an addressable RGB LED used for visual status indication and debugging.

**Functions:**
- RGB status indication
- System state visualization
- User feedback
- Debugging assistance

---

### RESET Button
The RESET button is connected to the ESP32 enable pin and allows manual restarting of the microcontroller.

**Functions:**
- System reset
- Firmware restart
- Fault recovery

---

### BOOT Button
The BOOT button is connected to GPIO0 and is used to place the ESP32 into firmware download mode for programming.

**Functions:**
- Enter bootloader mode
- Firmware flashing
- Recovery programming

---

### GPIO Expansion Headers
The GPIO headers expose ESP32 pins for future expansion and peripheral integration.

**Functions:**
- Sensor expansion
- Peripheral interfacing
- Prototyping support
- Future hardware upgrades

---

### Capacitors
Capacitors are used throughout the design for power supply filtering, decoupling, and voltage stabilization.

**Functions:**
- Noise reduction
- Voltage stabilization
- Power filtering
- Improved reliability

---

### Resistors
Resistors are used for pull-up networks, current limiting, voltage feedback, and configuration of various circuits.

**Functions:**
- Current limiting
- Pull-up networks
- Voltage feedback
- Signal conditioning

---

### Inductor (2.2 µH)
The inductor is a critical component of the TPS63001 switching regulator and enables efficient voltage conversion.

**Functions:**
- Energy storage
- Power conversion
- Switching regulation support

---

## Hardware Architecture

USB-C → MCP73831 → Li-Ion Battery → TPS63001 → 3.3V Rail → ESP32-S3

---

## Future Expansion

Planned future revisions may include:

- BME680 Environmental Sensor
- BH1750 Ambient Light Sensor
- MPU6050 IMU
- VL53L0X Distance Sensor
- OLED Display Support

---

## Status

- [x] Schematic Design
- [x] PCB Layout
- [ ] PCB Fabrication
- [ ] Assembly
- [ ] Testing
- [ ] Firmware Development

---

## Author

**Prathamesh Galphade**

Designed using KiCad.
