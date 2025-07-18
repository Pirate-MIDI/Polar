# Polar Controller DIY Build Guide

> ⚠️ This guide is for DIY builders and tinkerers. Pirate MIDI sells fully assembled units, but as part of our open-source commitment, we’re making this construction guide available for personal and non-commercial builds.

**[1. Hardware Assembly](https://github.com/Builty/TonexOneController/blob/main/WebConfiguration.md#entering-web-control)**

**[2. Installing Firmware](https://github.com/Builty/TonexOneController/blob/main/WebConfiguration.md#entering-web-control)**

**[3. Testing & Power-Up](https://github.com/Builty/TonexOneController/blob/main/WebConfiguration.md#entering-web-control)**

---

## 🧰 What You'll Need

Each variant of the Polar controller shares common elements. Below are general tools and materials you'll need.

### 🛠 Tools

- Soldering iron + solder
- Screwdriver set
- Heat-set insert tool or soldering iron with insert tip
- Flush cutters (for preparing wires)
- 3D printer (for enclosure) or printed parts
- Acrylic glue or double-sided tape (for protective overlay)
- JST crimping tool (if not using pre-crimped JST leads)

---

## 🔗 Polar Resources

- 📐 3D Enclosure Models: [Polar Pico](https://github.com/Pirate-MIDI/Polar/tree/main/Polar%20Pico), [Polar Mini](https://github.com/Pirate-MIDI/Polar/tree/main/Polar%20Mini), [Polar Plus](https://github.com/Pirate-MIDI/Polar/tree/main/Polar%20Plus), [Polar Max](https://github.com/Pirate-MIDI/Polar/tree/main/Polar%20Max)
- ⚡ Schematic & PCB Layout: [Polar Pico](https://github.com/Pirate-MIDI/Polar/tree/main/Polar%20Pico), [Polar Mini](https://github.com/Pirate-MIDI/Polar/tree/main/Polar%20Mini), [Polar Plus](https://github.com/Pirate-MIDI/Polar/tree/main/Polar%20Plus), [Polar Max](https://github.com/Pirate-MIDI/Polar/tree/main/Polar%20Max)
- 📄 [Firmware Source Code](https://github.com/Builty/TonexOneController)
- 📦 [Buy Pre-Assembled Units](https://piratemidi.com/)
- 📦 [Buy Waveshare ESP32 Boards](https://waveshare.com)

---

## 🔩 General Components List For All Variants

| Component                 | Description                                     |
|---------------------------|--------------------------------------------     |
| Custom PCB                | Input & power designed for each variant         |
| Waveshare Board           | ESP32-S3 Variants (main brain)                  |
| 3D Printed Enclosure      | STL provided; print in PLA or PETG (preferred)  |
| Heat-Set Inserts          | Brass M3                                        |
| M3 & M2 Screws            | Machine Thread (not tapping)                    |
| JST Connector             | For PCB to Waveshare connection                 |
| Acrylic Overlay (optional)| Laser-cut, protective top panel                 |

---

# 🔧 Hardware Assembly Instructions

Each variant has its own steps below. If you're unsure which variant you're building, check the product comparison table on [our website](https://piratemidi.com/products/polar).

---

## Polar Pico (No Screen)

Minimalist version – ideal for under-board use.

**[📺 Polar Pico Assembly Video Guide COMING SOON!]()**

### Parts List

- 1x Polar Pico PCB
- [1x Waveshare ESP32-S3 Zero](https://www.waveshare.com/esp32-s3-zero.htm)
- 1x 3D printed enclosure 
- [4x M3x4mmx5mm Heat-set Inserts](https://github.com/user-attachments/assets/3e2e96b9-6922-4ddc-a0e5-bb1fc9a778b4)
- 4x M3x7mm screws
- [1x JST-SH 12-pin Dual-Male Cable](https://github.com/user-attachments/assets/c0d687e7-e608-4e23-b043-ad0c6be05575)
- Optional: Acrylic Protective Overlay

### Steps

1. **Solder Waveshare headers to PCB**
   ![Step 1: Soldering headers](./images/pico_solder_headers.jpg)

2. **Heat-insert brass M3 inserts into 3D printed enclosure**
   ![Step 3: Heat set inserts](./images/pico_inserts.jpg)

3. **Mount PCB and Waveshare into enclosure and secure with screws**

4. *(Optional)* Apply acrylic overlay using adhesive or standoffs.

---

## Polar Mini (Screen, No Switches)

Screen-only version for visual feedback in tight spaces.

**[📺 Polar Mini Assembly Video Guide COMING SOON!]()**

### Parts List

- 1x Polar Mini PCB  
- [1x Waveshare ESP32-S3 1.69](https://www.waveshare.com/esp32-s3-lcd-1.69.htm)
- 1x 3D printed enclosure
- [4x M3x4mmx5mm Heat-set Inserts](https://github.com/user-attachments/assets/3e2e96b9-6922-4ddc-a0e5-bb1fc9a778b4)
- 4x M3x7mm screws
- [1x JST-SH 12-pin Dual-Male Cable](https://github.com/user-attachments/assets/c0d687e7-e608-4e23-b043-ad0c6be05575)
- Optional: Acrylic Protective Overlay

### Steps

(Same general steps as Pico, with attention to screen alignment)

1. **Connect PCB to Waveshare 1.69 module with JST cable**
   ![Step: Screen and MCU soldering](./images/mini_solder_screen.jpg)

2. **Heat-insert brass M3 inserts into 3D printed enclosure**

3. **Mount PCB and Screen into enclosures with care to align screen**

4. **Close enlclosure with screws**

5.  *(Optional)* Apply acrylic overlay using adhesive or standoffs.

---

## Polar Plus (Screen + 2 Footswitches)

**[📺 Polar Plus Assembly Video Guide COMING SOON!]()**

This version includes two footswitches for changing presets or other toggles.

### Additional Parts

- 2x Momentary, Normally Open (NO) footswitches   
- Wiring for switches

### Steps

1. **Solder wires to footswitches**
2. **Insert footswitches in enclosure and fasten**
3. **Solder footswitch wires onto PCB**
4. **Attach screen and MCU as per Mini**
5. **Secure all components into enclosure**
   ![Footswitch mounting](./images/plus_footswitches.jpg)
6. *(Optional)* Apply acrylic overlay

---

## Polar Max (Touchscreen + Full Control)

The flagship controller with touchscreen and full ToneX One editing onboard.

**[📺 Polar Max Assembly Video Guide](https://youtu.be/EYmiK8_B6EI)**

### Additional Parts

- [1x Waveshare 4.3b Touchscreen Module](https://www.waveshare.com/esp32-s3-touch-lcd-4.3b.htm) 
- 2x Momenatry Normally-Open (NO) Footswitches
- 1x JST-SH 12-pin connector with ferrules or open wires on other end

### Steps

1. **Install heat-set inserts**
2. **Solder wires to footswitches**
3. **Install footswitches into enclosure**
4. **Secure display into 3D printed housing**
5. **Fasten PCB to bottom plate of enclosure**
6. **Connect PCB and Waveshare with JST to Ferrules wire harness - See circuit diagram for details**
7. **Connect footswitches to PCB**
8. **Close enclosure and fasten with screws**
9. *(Optional)* Install overlay or protective cover

---

# 🖥️ Installing Firmware

To install the firmware, follow the instructions [found on the original project page here](https://github.com/Builty/TonexOneController/blob/main/FirmwareUploading.md).

---

# 🧪 Testing & Power-Up

1. Power via USB or 9V 2.1mm center-negative barrel jack  
2. Connect to [Web Configurator](https://github.com/Builty/TonexOneController/blob/main/WebConfiguration.md#entering-web-control) 
3. Test MIDI input and screen functionality.
   
   > ⚠️ Wired MIDI needs to be activated in the web configurator
4. Confirm footswitch response. (if applicable)

---

## 🧼 Tips & Troubleshooting

- If the 9v Power or MIDI input doesn't work, double-check the JST pinout or your manual wiring if you didn't use JST.
- Waveshare boards may not have factory firmware. Flash firmware before deciding your unit is "dead".
- Over-tightening screws can crack the enclosure. Don’t overdo it.
- If you have a construction issue, you can contact us in our [Discord Server](https://discord.gg/x722K7ksA6) (Polar Channel), or on the original open source project discussion tab. 

---

## 📸 Contributing

Found an error in these instructions? Feel free to submit a pull request!

---

## 📜 License

This project is licensed under the MIT License. Commercial resale of DIY units is not permitted under our license.
