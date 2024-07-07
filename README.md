# Bin Picking Robot PCB

This repository contains the PCB design files for the bin picking robot project, developed using Altium Designer. The project has gone through two versions, with the second version incorporating improvements and changes based on component availability and expert guidance.

## Overview

The bin picking robot PCB is a component of a robotic system designed for demonstration purposes.This project includes the following key features:

- **Microcontroller Unit (MCU):** ATmega328P for controlling various components.
- **Sensors:**  Integration of a membrane sensor and a pressure sensor for precise control and feedback.
- **Motor Driver:** DRV8825 to control the stepper motors used in the robot gripper.
- **Indicators and Display:**  LEDs and a OLED display for user interface.
- **UART Ports:** For communication with main devices(get coordinates).
- **Power Input and Regulators:** To ensure stable power supply to all components.

## Block Diagram

![Block Diagram](https://github.com/mora-bprs/Bin-picking-PCB/blob/main/Schematic%20Design/Block%20Diagram.png)

## Versions

### Version 1
- **MCU:** ATmega2560
- **Reason for Change:** Due to the unavailability of ATmega2560 components on the Mouser website.

### Version 2
- **MCU:** ATmega328P
- **Guidance:** This version was developed under the guidance of Prof. Jayasingha.
- **Improvements:** Adjustments based on component availability and expert recommendations.

## Repository Structure

- `Version1/` - Contains design files for the first version of the PCB.
- `Version2/` - Contains design files for the second version of the PCB.
- `Schematic designs` - Schematic designs of the PCB components.
- `PCB design` - - Final PCB design files.

## Main SchDoc
![main](https://github.com/mora-bprs/Bin-picking-PCB/blob/main/Schematic%20Design/Main%20SchDoc.png)

## MCU SchDoc
![mcu](https://github.com/mora-bprs/Bin-picking-PCB/blob/main/Schematic%20Design/MCU%20SchDoc.png)

## Motor Driver SchDoc
![motor driver](https://github.com/mora-bprs/Bin-picking-PCB/blob/main/Schematic%20Design/MotorDrive%20SchDoc.png)

## Power SchDoc
![power schdoc](https://github.com/mora-bprs/Bin-picking-PCB/blob/main/Schematic%20Design/Power%20SchDoc.png)

## Bill of Materials (BOM)

| Comment            | Description                               | Designator                             | Footprint                   | LibRef                | Quantity |
|--------------------|-------------------------------------------|----------------------------------------|-----------------------------|-----------------------|----------|
| 06035C104KAT4A     |                                           | C1, C3, C4, C8, C9, C11                | CAPC1608X90X35LL15T15       | CMP-2006-04390-1      | 6        |
| B2B-XH-AM_LF__SN_  | Connector                                  | PWRIN_J1, SENSOR_1, SWITCH-INT, TXRX_2 | B2BXHAMLFSN                 | B2B-XH-AM_LF__SN_     | 4        |
| B4B-XH-A_LF__SN_   | Connector                                  | DISPLAY, J1, SENSOR_2, TXRX_1          | B4BXHALFSN                  | B4B-XH-A_LF__SN_      | 4        |
| EEE-1EA470WP       | Capacitor Polarised                        | C20, C21                               | EEE1AA101SP                 | EEE-1EA470WP          | 2        |
| ERJ-3RSFR10V       | Resistor                                   | R4, R5                                 | ERJ3_B_BQ_BW_LW_(0603)      | ERJ-3RSFR10V          | 2        |
| ERJ-S1TD4533U      | Resistor                                   | R7, R8                                 | ERJS1T_U1T_(2512)           | ERJ-S1TD4533U         | 2        |
| GCM31CR71H225KA55K | Ceramic Capacitor for Automotive 2.2uF     | C17, C18                               | FP-GCM31C-0_2-e0_3_0_8-MFG  | CMP-06035-059276-1    | 2        |
| RT1206BRD0710KL    | RES 10.0K OHM 1/4W .1% SMD 1206            | R2, R11                                | FP-RT1206-MFG               | CMP-2003-04273-2      | 2        |
| 02015C560KAT2A     |                                           | C19                                    | CAPC0603X33X15ML03T05       | CMP-2010-00470-1      | 1        |
| 06035A220JAT4A     |                                           | C5                                     | CAPC1608X90X35NL15T15       | CMP-2006-04271-1      | 1        |
| 12065C332KAT2A     | General Purpose Ceramic Capacitor, 1206    | C15                                    | FP-1206-L_3_2_0_2-W_1_6_0-IPC_C | CMP-04427-015080-1 | 1        |
| 1571634-2          | SWITCH TACTILE SPST-NO 0.05A 24V           | SW1                                    | FP-1571634-2-MFG            | CMP-03407-000008-1    | 1        |
| 3540100KJT         | Resistor                                   | R9                                     | RESC7142X120N               | 3540100KJT            | 1        |
| 61300211121        | Connector                                  | J2                                     | HDRV2W110P0X254_1X2_508X254X854P | 61300211121    | 1        |
| AORN1001AT5        | Resistor Network                           | RN2                                    | SOIC127P607X173-8N          | AORN1001AT5           | 1        |
| APT2012SECK_J3-PRV | LED                                        | MOTOR                                  | APT2012SECKJ3PRV            | APT2012SECK_J3-PRV    | 1        |
| ATmega328P-AU      | 8-bit AVR Microcontroller                  | U1                                     | 32A_M                       | CMP-0095-00269-2      | 1        |
| BD03               | Switch                                     | S1                                     | BD03                        | BD03                  | 1        |
| C0603C104K5RAC3190 | Capacitor                                  | C22                                    | C0603                       | C0603C104K5RAC3190    | 1        |
| C0603C105K3PACTU.  | Capacitor                                  | C10                                    | CAPC1608X95N                | C0603C105K3PACTU.     | 1        |
| C0805C474J5REC7800 | Capacitor                                  | C13                                    | CAPC2012X110N               | C0805C474J5REC7800    | 1        |
| C1210C475J5RACAUTO | Capacitor                                  | C7                                     | C1210                       | C1210C475J5RACAUTO    | 1        |
| CAY16-103J4GLF     | Resistor Network                           | RN1                                    | CAY16-J4                    | CAY16-103J4GLF        | 1        |
| CD1206-S01575      | Diode                                      | D1                                     | DIOC3215X95N                | CD1206-S01575         | 1        |
| CGRA4007-G         | Integrated Circuit                         | D3                                     | DIOM5127X229N               | CGRA4007-G            | 1        |
| CL31B106KBHNNNE    | CAP CER 10UF 50V X7R 1206                  | C2                                     | FP-CL31B106KBHNNNE-MFG      | CMP-2000-07530-2      | 1        |
| CRCW251249K9FKEG   | Resistor                                   | R10                                    | RESC6332X70N                | CRCW251249K9FKEG      | 1        |
| CSTCE16M0V53-R0    | Crystal or Oscillator                      | Y1                                     | CSTCE16M0V53R0              | CSTCE16M0V53-R0       | 1        |
| CV201210-100K      | Inductor                                   | L1                                     | INDC2012X145N               | CV201210-100K         | 1        |
| DRV8825PWP         | Stepper Motor Controller IC               | U3                                     | PWP0028C_L                  | CMP-1685-00019-1      | 1        |
| ERA-2AEB152X       | Resistor                                   | R3                                     | ERA2AED122X                 | ERA-2AEB152X          | 1        |
| ERJ-3GEYJ105V      |                                           | R1                                     | RESC1608X55X30NL15T15       | CMP-2000-00706-1      | 1        |
| GRM21BR60J226ME39L | Chip Multilayer Ceramic Capacitors         | C16                                    | FP-GRM21B-0_15-MFG          | CMP-2007-03385-2      | 1        |
| GRM31C5C1H104JA01L | Chip Multilayer Ceramic Capacitors         | C6                                     | FP-GRM31C-0_2-e0_3_0_8-IPC_B | CMP-06035-003994-1  | 1        |
| GRM155R71H103JA88D | Chip Multilayer Ceramic Capacitors         | C12                                    | FP-GRM155-0_05-IPC_A        | CMP-2008-04636-2      | 1        |
| GRM155R71H222JA01D | Chip Multilayer Ceramic Capacitors         | C14                                    | FP-GRM155-0_05-IPC_C        | CMP-2008-04651-2      | 1        |
| KPT-2012SGC        | LED                                        | POWER                                  | LEDM2012X120N               | KPT-2012SGC           | 1        |
| LM5012DDAR         | Integrated Circuit                         | IC1                                    | SOIC127P600X170-9N          | LM5012DDAR            | 1        |
| LP2985-33DBVR      | Single Output Low Noise LDO                | U2                                     | DBV0005A_M                  | CMP-0758-00080-2      | 1        |
| PH2-06-UA          | Connector                                  | ICSP1                                  | HDRV6W64P254_2X3_762X500X901P | PH2-06-UA           | 1        |
| PJ-102BH           | Through Hole Right Angle DC Power Jack     | J3                                     | CUI-PJ-102BH_V              | CMP-2000-06901-1      | 1        |
| RC0402FR-074K7L    | Resistor                                   | R6                                     | RESC1005X40N                | RC0402FR-074K7L       | 1        |
| SPX1117M3-L-5-0_TR | Power Supply                               | PS1                                    | SOT230P700X170-4N           | SPX1117M3-L-5-0_TR    | 1        |
| SRR1280-330M       | FIXED IND 33UH 3.5A 57 MOHM SMD            | L2                                     | FP-SRR1280-MFG              | CMP-2000-07148-2      | 1        |
| TC33X-2-103E       | Variable Resistor                          | VR1                                    | TC33X2503E                  | TC33X-2-103E          | 1        |
| V8P12-M3_86A       | Diode                                      | D2                                     | V8P12M386A                  | V8P12-M3_86A          | 1        |



## Getting Started

To get started with this project:

1. Clone the repository:
    ```sh
    git clone https://github.com/mora-bprs/Bin-picking-PCB.git
    ```
2. Open the design files in Altium Designer.
3. Review the block diagram and design files for an overview of the PCB layout and components.

## Contribution

If you would like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch:
    ```sh
    git checkout -b feature-branch
    ```
3. Make your changes and commit them:
    ```sh
    git commit -m 'Add some feature'
    ```
4. Push to the branch:
    ```sh
    git push origin feature-branch
    ```
5. Create a new Pull Request.

## Acknowledgments

Special thanks to Prof. Jayasingha for his guidance and support in developing this PCB.
