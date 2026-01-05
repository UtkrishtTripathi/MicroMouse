# 🐭 WRC Micromouse – STM32 (Arduino IDE)

![Micromouse](render/img1.png)

A **maze-solving autonomous robot** built for the **WRC Micromouse Competition**, powered by an **STM32 microcontroller** and programmed using the **Arduino IDE**.  
This project focuses on high-speed maze-solving with smooth, precise movement, robust sensors, and optimized path planning.  

> Firmware is intentionally excluded; this repo focuses on **hardware design and fabrication assets**.

---

## 🧠 Overview

Micromouse is a robotics challenge where a small robot must explore and solve an **unknown maze** in the fastest time.  
Our STM32-based Micromouse combines reliable hardware with intelligent algorithms for competitive performance.  

The robot is equipped with:

- **IR Sensors** for wall detection  
- **Quadrature Encoders** to track movement precisely  
- **BNO085 Gyroscope/IMU** for smooth and accurate turns  
- **Flood-Fill Algorithm** for maze-solving  
- **Optimized path planning**, including diagonal movements  
- **On-board tactile buttons** for mode selection and tuning  

---

## ⚡ Key Features

- **STM32-based high-performance control board** for precise motion  
- **Smooth gyro-assisted turning** for fast and accurate navigation  
- **Robust sensor integration**: IR/TOF + encoders + gyroscope  
- **Optimized analog/digital routing** for reliable sensor readings  
- Symmetric PCB layout → predictable motion behavior  
- Board acts as both **control & structural element**  
- Tested in **real-world maze-solving scenarios**

---

## 🔧 Motor Driver Variants

Two PCB variants designed with the same geometry & sensor placements:

| Variant | Motor Driver | Notes |
|---------|--------------|-------|
| A       | TB6612FNG    | Robust dual H-bridge, high-current margin, early testing |
| B       | DRV8833      | Compact, efficient, thermally stable, alternative solution |

---

## 🖼️ PCB Layouts

**TB6612FNG Variant**  
![TB6612 Layout](path/to/tb6612_layout_image.png)

**DRV8833 Variant**  
![DRV8833 Layout](path/to/drv8833_layout_image.png)

---

## 🛠️ Assembled Hardware

**DRV8833 Variant – 4-layer SMD PCB**  
![DRV8833 SMD](path/to/drv8833_smd_image.png)  

**Motors Mounted**  
![DRV8833 Motors](path/to/drv8833_motors_image.png)  

**Side-by-Side Comparison**  
![Comparison](path/to/comparison_image.png)  

---

## 🏭 Fabrication

Recommended fabrication parameters:

- **4-layer PCB**  
- FR4 material, 1.6 mm thickness  
- Green solder mask  

Can be fabricated via **JLCPCB, PCBWay**, or other standard manufacturers.

---

## 📊 Project Status

- ✔ PCB designed & fabricated  
- ✔ Assembled and tested on robot  
- ✔ Multiple motor driver variants evaluated  
- ✖ Firmware excluded intentionally  

---

## 🙏 Acknowledgements

Inspired by open-source robotics PCBs.  
All circuitry, routing, component selection, and motor driver integration were **designed from scratch** for an STM32-based competitive Micromouse.  

---

## ⚠️ Disclaimer

This design is for **educational and experimental purposes**.  
The author assumes no responsibility for damage, malfunction, or misuse. Use at your own risk.
