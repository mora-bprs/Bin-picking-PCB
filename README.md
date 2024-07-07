# Bin Picking Robot PCB

This repository contains the PCB design files for the bin picking robot project, developed using Altium Designer. The project has gone through two versions, with the second version incorporating improvements and changes based on component availability and expert guidance.

## Overview

. This project includes the following key features:

- **Microcontroller Unit (MCU):** The PCB is designed to accommodate an MCU for controlling various components.
- **Sensors:** Integration of membrane and pressure sensors for precise control and feedback.
- **Motor Driver:** To control the motors used in the robot.
- **Indicators and Display:** For user interface and debugging.
- **UART Ports:** For communication with other devices.
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
- `Block Diagram.png` - Block diagram of the PCB components.

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

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

Special thanks to Prof. Jayasingha for his guidance and support in developing this PCB.
