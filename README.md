# USB_TO_UART-CP2102

This is a simple and compact USB to UART (serial) converter board designed using the **CP2102 IC** from **Silicon Labs**, with a USB-C input interface. The board was created in **KiCad** and is suitable for use in embedded system development, serial debugging, or programming microcontrollers like STM32, ESP32, Arduino, and more.

## 🔍 About the CP2102

The **CP2102** is a popular single-chip USB to UART bridge manufactured by **Silicon Labs**. It integrates a USB 2.0 transceiver, a crystal-less oscillator, EEPROM, and UART logic in one compact package, making it ideal for simple, low-cost serial communication with PCs or other USB hosts.

### 💡 Where It's Commonly Used

- USB serial debug tools
- Microcontroller bootloader interfaces
- Firmware flashing tools for ESP8266 / ESP32
- Industrial sensor-to-PC interfaces
- USB-based serial consoles (Linux serial TTY access)

---

## 🔗 Features

- USB to UART bridge using **CP2102**
- USB-C connector for modern device compatibility
- 0603 SMD components for compact layout
- Designed using KiCad 6+
- Gerbers ready for fabrication

---

| File/Folder  | Description                                                                 |
| ------------ | --------------------------------------------------------------------------- |
| `.kicad_pro` | KiCad project file (project configuration)                                  |
| `.kicad_sch` | Schematic file (circuit design)                                             |
| `.kicad_pcb` | PCB layout file (2D + 3D design of the board)                               |
| `gerbers/`   | Folder containing Gerber files and drill data for PCB fabrication           |
| `.step`      | 3D model of the assembled PCB for enclosure design and mechanical CAD usage |

---

## ⚙️ Comparison with Other USB-to-UART Chips

| Chip        | Manufacturer   | Max Baud Rate | Supply Voltage | Notes |
|-------------|----------------|---------------|----------------|-------|
| **CP2102**  | Silicon Labs   | ~1 Mbps       | 3.3V or 5V     | Reliable, widely supported               |
| CH340G      | WCH (China)    | ~921.6 kbps   | 5V             | Cheap, needs driver on Windows           |
| FT232RL     | FTDI           | ~3 Mbps       | 3.3V / 5V      | Expensive but robust and driver-friendly |
| PL2303      | Prolific       | ~1 Mbps       | 3.3V / 5V      | Less reliable in some OS versions        |

> 💬 The **CP2102** offers a good balance of **cost, stability, and driver support** (native support in Windows, Linux, macOS). It is more stable than CH340G, and more affordable than FT232RL.

---

## 🏗️ Applications

- Serial console access for Linux/Raspberry Pi
- Programming ESP8266/ESP32 boards
- USB-based microcontroller bootloader communication
- Debugging UART output of embedded systems

---

## 📌 Notes

- TX, RX, GND, 3.3V/5V, and DTR/RTS signals can be broken out depending on layout.
- USB-C connector provides better mechanical strength than micro-USB.
- LDO regulator is optional; useful if powering external 3.3V peripherals.

---

## 📤 License

This hardware design is open source and released under the **MIT License**. You are free to use, modify, and distribute it.

---

## 🖼️ Preview

3d Images are added with FRONT,BACK,and ISOMETRIC views.

---
🔗 GrabCAD Model (3D STEP File)

Check out the 3D model of this project on my GrabCAD profile:
👉 https://grabcad.com/maathes.thilak-1

You can view, download, and integrate the .STEP file for enclosure development or CAD simulation.

---

## 🤝 Contributions

Feel free to fork, improve, or suggest enhancements via pull requests or issues!

