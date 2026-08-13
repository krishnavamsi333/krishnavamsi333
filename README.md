<div align="center">

# Krishna Vamsi Kasimalla

**Power Electronics & Robotics Engineer**

Building high-efficiency power conversion hardware and autonomous systems — from LTspice to field-tested PCBs and ROS 2 stacks.

[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kasimallakrishnavamsi333@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/krishnavamsikasimalla)
[![Portfolio](https://img.shields.io/badge/Portfolio-4A154B?style=for-the-badge&logo=googlechrome&logoColor=white)](https://krishnavamsi333.github.io/Portfolio/)

`Vijayawada, India` · `Open to full-time roles` · `Power Electronics · Embedded · Robotics`

</div>

---

## About

I design power electronics — DC-DC converters, battery management systems, motor drives — and build autonomous robots on ROS 2. My work sits at the seam between the two: hardware that has to survive real loads, and firmware that has to make correct decisions in milliseconds.

Alongside that, I lead the **EV Club at VRSEC**, where we design and build prototype electric vehicles, and I write open-source tools for the workflow gaps I keep hitting in my own projects.

---

## Tech Stack

**Languages & Frameworks**
![C/C++](https://img.shields.io/badge/C%2FC%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![ROS 2](https://img.shields.io/badge/ROS_2_Humble-22314E?style=flat-square&logo=ros&logoColor=white)
![MATLAB](https://img.shields.io/badge/MATLAB_%2F_Simulink-0076A8?style=flat-square&logo=mathworks&logoColor=white)
![FreeRTOS](https://img.shields.io/badge/FreeRTOS-3CB371?style=flat-square)

**Hardware**
![STM32](https://img.shields.io/badge/STM32-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)
![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=flat-square&logo=espressif&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi-A22846?style=flat-square&logo=raspberrypi&logoColor=white)
![Jetson](https://img.shields.io/badge/NVIDIA_Jetson-76B900?style=flat-square&logo=nvidia&logoColor=white)

**EDA & Tooling**
![KiCad](https://img.shields.io/badge/KiCad-1B4FBB?style=flat-square&logo=kicad&logoColor=white)
![Altium](https://img.shields.io/badge/Altium-A5915F?style=flat-square&logo=altiumdesigner&logoColor=white)
![LTspice](https://img.shields.io/badge/LTspice-0047AB?style=flat-square&logo=analogdevices&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-E95420?style=flat-square&logo=ubuntu&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

| Domain | Focus |
|---|---|
| **Power Electronics** | Buck/boost converters, inverters, motor drives, power stage layout |
| **Battery Systems** | BMS firmware, SoC/SoH estimation, cell balancing, CAN telemetry |
| **Renewable Energy** | Solar MPPT control, grid-tie inverters |
| **Robotics & Autonomy** | ROS 2, SLAM, Nav2, LiDAR + odometry fusion, path planning |
| **Embedded Systems** | Real-time firmware, FreeRTOS, CAN / UART / I²C, interrupt-driven design |

---

## Projects

### 48V Lithium BMS with Active Cell Balancing
`STM32H7` `Embedded C++` `CAN FD` · Production-ready prototype

- Real-time monitoring of 16 series cells to ±10 mV via differential ADC sampling
- Switched-resistor active balancing: pack imbalance from 2.5 V → <0.1 V in ~2 hours
- Safety-critical firmware — over-current cutoff under 2 ms, over-temperature and deep-discharge protection
- Validated over 500+ charge/discharge cycles from −10 °C to 60 °C

**Result:** ~15% more usable energy density than passive balancing.

<br/>

### Solar MPPT Charge Controller
`STM32F4` `MATLAB/Simulink` `LTspice` · Prototype → PCB

- Perturb & Observe MPPT hitting 95.3% peak efficiency, converging in under 2 seconds across 200–1000 W/m²
- 600 W input rating with 12/24/48 V charging modes and soft-start PWM
- 40-hour field log under variable cloud cover held 94.7% average efficiency

**Result:** 18–22% higher daily energy harvest vs. constant-voltage charging.

<br/>

### Agri-Bot — LiDAR Autonomous Field Robot
`ROS 2 Humble` `Python` `Cartographer` `Nav2` · Field-tested on 5 hectares

- 2D SLAM with under 5 cm localisation error in GPS-denied rows
- RPLiDAR A1 fused with wheel odometry and IMU for drift-resistant pose estimation
- Dynamic Window Approach avoidance at ~95% detection on rocks and furrows
- Containerised ROS 2 stack on a Raspberry Pi 4 with MQTT telemetry

**Result:** 80% less manual surveying time across 50+ autonomous missions.

<br/>

### DC-DC Converter Design & PCB Layout
`LTspice` `Altium` `STM32F1` · Buck and boost topologies

- Boost: 12 V → 48 V, 100 W continuous, for solar + battery hybrid systems
- Buck: 48 V → 12 V multi-output auxiliary supply with integrated over-current sensing
- ≥92% efficiency at rated load; ±5% line/load regulation, <50 mV ripple under step transients
- 4-layer layout with dedicated power/ground planes and star-point distribution

**Result:** Hand-soldered prototypes, zero magic smoke.

---

## Open-Source Tools

**[DBC2DBF Converter](https://dbc2dbf-tool.onrender.com/)** — browser-based CAN database `.dbc` → DBF conversion with batch processing and signal-mapping validation. Built for EV powertrain and motorsport teams working across incompatible CAN toolchains. *React + Python, deployed on Render.*

**[KiBOM Procurement Tool](https://kibom.onrender.com/)** — upload a KiCad BOM, get back a procurement-ready CSV with MPNs, Digi-Key/Mouser links, aggregated pricing and stock levels. Replaces hours of manual supplier mapping.

---

## Writing

| Guide | Covers |
|---|---|
| [**KiCad PCB Design**](https://krishnavamsi333.github.io/kicad-guide/) | Schematic capture, footprint libraries, layout practice for power boards |
| [**Raspberry Pi Setup**](https://krishnavamsi333.github.io/RPI/) | OS setup, GPIO, ROS 2 on Pi, real-time considerations |

---

## Experience

**President — Electric Vehicle Club, VRSEC** · 2023–Present
Grew the club from 8 to 50+ active members and ran 12+ technical workshops. Led design and assembly of two prototype electric motorcycles (0–60 km/h in 6.5 s). Raised ₹50,000+ in sponsorship and managed component procurement.

**Power Electronics Research (Academic)** · 2023–2024
Simulated and validated MPPT algorithms for solar systems, characterised DC-DC converter topologies under dynamic thermal load, and mentored 5+ junior students on embedded and robotics projects.

---

## Education

**B.Tech, Electrical Engineering** — V.R. Siddhartha Engineering College, Vijayawada · 8.2/10 · 2024

Certifications: FreeRTOS Fundamentals (STMicroelectronics) · ROS 2 Humble · Advanced C++ for Embedded Systems · MATLAB/Simulink for Control Systems

---

## Currently

```text
→ 48V BMS ........ PCB manufacturing and field testing
→ Solar MPPT ..... prototype assembly, efficiency validation
→ Agri-Bot ....... LiDAR + stereo fusion for obstacle classification
→ Learning ....... GaN power stages for >1 MHz converters
→ Next ........... open-source ROS 2 perception stack for agri robots
```

---

<div align="center">

[![Stats](https://github-readme-stats.vercel.app/api?username=krishnavamsi333&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true&title_color=A855F7&text_color=FFFFFF)](https://github.com/krishnavamsi333)
[![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=krishnavamsi333&layout=compact&theme=tokyonight&hide_border=true&title_color=A855F7&text_color=FFFFFF)](https://github.com/krishnavamsi333)

</div>

---

## Open To

Full-time work in power electronics, BMS, embedded firmware, renewable energy, or autonomous robotics — and collaborations on open-source ROS 2 and EV powertrain projects. Happy to talk mentoring on power electronics simulation, ROS 2, or KiCad/Altium workflows.

<div align="center">

**[Email](mailto:kasimallakrishnavamsi333@gmail.com)** · **[LinkedIn](https://www.linkedin.com/in/krishnavamsikasimalla)** · **[Portfolio](https://krishnavamsi333.github.io/Portfolio/)**

*Build. Test. Learn. Iterate. Ship.*

</div>
