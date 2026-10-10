🚗 EV Dashboard and ADAS Warning System

A simulation-based automotive embedded systems project integrating STM32 firmware, four ultrasonic sensors, virtual serial communication, and a Python Tkinter dashboard to demonstrate electric vehicle monitoring and basic obstacle detection.

📌 Project Overview :

The EV Dashboard and ADAS Warning System is a software-based simulation developed to explore the integration of embedded systems and automotive monitoring applications.

The project uses PICSimLab to simulate the microcontroller environment, STM32CubeIDE for firmware development, VSPE (Virtual Serial Ports Emulator) for serial communication, and Python Tkinter to create a graphical dashboard.

Four ultrasonic sensors are used for simulated obstacle detection around the vehicle. The system also incorporates simulated vehicle parameters such as accelerator input, temperature, battery State of Charge (SOC), and brake input.

The Python dashboard provides a graphical interface for monitoring the information transmitted from the simulated embedded system.

This project demonstrates the fundamental concepts behind an EV monitoring interface and a basic Advanced Driver Assistance System (ADAS).

🎯 Objectives

- Develop a simulated EV monitoring application using the STM32F103C8T6 microcontroller environment.
- Represent essential vehicle parameters, including accelerator input, temperature, battery SOC, and brake input.
- Use four ultrasonic sensors for multi-directional obstacle detection in the simulation.
- Establish serial communication between the simulated embedded system and the Python application using VSPE.
- Develop a desktop dashboard using Python Tkinter.
- Understand embedded firmware development, sensor integration, serial communication, and graphical data visualization.

🛠️ Technologies Used

Technology| Purpose
STM32F103C8T6 Blue Pill| Target microcontroller for the simulated embedded application
STM32CubeIDE| Firmware development and STM32 configuration
PICSimLab| Simulation and testing environment
VSPE| Virtual serial port communication
Python| Dashboard development and data handling
Tkinter| Graphical user interface
Ultrasonic sensors (×4)| Obstacle distance sensing in the simulation

🏗️ System Architecture

The project is organized into four main layers.

+------------------------------------+
|          PICSimLab                 |
|   Simulated STM32 + Sensor Inputs  |
|                                    |
|  Vehicle Parameters                |
|  Four Ultrasonic Sensors           |
+-----------------+------------------+
                  |
                  | Serial Data
                  v
+------------------------------------+
|              VSPE                  |
|       Virtual COM Port Pair        |
+-----------------+------------------+
                  |
                  | Serial Communication
                  v
+------------------------------------+
|          Python Application        |
|                                    |
|  Serial Data Reception             |
|  Data Processing                   |
|  Tkinter Dashboard                 |
|  Vehicle / Obstacle Visualization  |
+------------------------------------+

Data flow: Simulated sensor and vehicle data → STM32 firmware → virtual serial communication through VSPE → Python application → Tkinter dashboard.

The diagram represents the intended architecture. Successful end-to-end operation depends on the actual firmware, serial protocol, and simulation configuration.

## 🎥 Project Presentation

Watch the PowerPoint presentation explaining the **EV Dashboard and ADAS Warning System**, including the project overview, system architecture, working principle, and future enhancements.

▶️ **[Watch the Project Explanation on YouTube](https://youtu.be/osSQamRVhRE)**



⚙️ Working Principle

1. Vehicle Parameter Monitoring

Simulated input values represent accelerator position, temperature, battery State of Charge (SOC), and brake input. The embedded firmware processes the inputs according to the implemented logic.

2. Four-Ultrasonic-Sensor Obstacle Detection

Four ultrasonic sensors are used to represent obstacle detection in different directions around the simulated vehicle. Their distance measurements provide information about nearby obstacles.

3. STM32 Firmware Processing

The firmware is developed using STM32CubeIDE for the STM32F103C8T6 target. It handles the configured inputs, processes sensor information, and prepares the data for serial transmission according to the implemented communication protocol.

4. Virtual Serial Communication

VSPE provides a virtual COM port connection between the software components. The Python application reads the serial data through the configured port, avoiding the need for a physical UART connection between separate hardware devices.

5. Python Tkinter Dashboard

The Tkinter desktop application acts as the vehicle monitoring interface. It can display the vehicle parameters and ultrasonic sensor readings received through serial communication, depending on the implemented dashboard features.

6. ADAS Warning Logic

The ultrasonic distance readings can be evaluated against predefined distance thresholds to identify nearby obstacles and trigger proximity warnings. The exact warning behavior depends on the logic implemented in the firmware or dashboard.

✨ Project Highlights

- Simulation-based development: Explores embedded system functionality without requiring a physical hardware prototype.
- Multi-sensor obstacle detection: Uses four ultrasonic sensors to represent the surroundings of a simulated vehicle.
- Embedded-PC integration: Connects a simulated STM32 application with a Python desktop interface.
- Virtual serial communication: Uses VSPE to establish communication through virtual COM ports.
- Graphical monitoring: Uses Tkinter to build a desktop dashboard for vehicle and sensor information.
- Automotive application: Combines EV parameter monitoring with basic ADAS concepts in one project.


🧠 Concepts Learned

This project provides practical exposure to:

- STM32 microcontroller programming
- Embedded firmware developmen
- Sensor interfacing concepts
- Ultrasonic distance measurement
- Serial communication and virtual COM ports
- Python desktop GUI development with Tkinter
- Data reception and visualization
- Simulation-based embedded system testing
- Basic automotive monitoring and ADAS concepts

🔮 Future Enhancements

- Add real-time plots for vehicle parameters.
- Improve the visual representation of the four sensor directions.
- Implement configurable, color-coded proximity warnings.
- Add serial communication error handling and connection-status indicators.
- Introduce CAN communication concepts for automotive networking.
- Extend the simulation with additional vehicle monitoring functions.
- Validate the design on physical hardware in future work.

⚠️ Limitations and Disclaimer

- This project is simulation-based and has not been validated on a physical vehicle.
- The accuracy of sensor readings depends on the simulation and implemented models.
- The project demonstrates basic obstacle detection and warning concepts, not a certified ADAS implementation.
- It must not be used as a real-world collision prevention or vehicle safety system.

👩‍💻 Project Information

- Project Name: EV Dashboard and ADAS Warning System
- Domain: Embedded Systems / Automotive Electronics
- Target Microcontroller: STM32F103C8T6
- Simulation Environment: PICSimLab
- Firmware Development: STM32CubeIDE
- Communication: VSPE / Virtual Serial Ports
- Dashboard: Python Tkinter
- Sensor Configuration: Four ultrasonic sensors

---

Developed as an educational project to explore the integration of embedded systems, simulation, serial communication, and automotive dashboard development.
