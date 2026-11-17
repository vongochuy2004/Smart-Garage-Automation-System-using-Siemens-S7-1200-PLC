# Smart-Garage-Automation-System-using-Siemens-S7-1200-PLC
Simulation of an automated garage management system using Siemens S7-1200 PLC and TIA Portal. The project integrates automatic ventilation control, vehicle detection, garage door operation, and visual status monitoring through sensors, motors, and indicator lights.
# Smart Garage Automation System using Siemens S7-1200 PLC

## 1. Project Overview

This project focuses on designing and simulating an automated garage management system using the **Siemens S7-1200 PLC (CPU 1214C DC/DC/DC)**.

The system integrates garage ventilation control, vehicle detection, automated garage door operation, and status monitoring. It uses multiple sensors, control switches, motors, and indicator lights to simulate the operation of a smart parking garage.

The control logic is developed and simulated using Siemens TIA Portal.

## 2. System Features

### 2.1. Ventilation Control
- Control four ventilation fans independently.
- Individual ON/OFF control for each fan.
- Monitor airflow conditions using airflow sensors (B1–B4).
- Display ventilation system status through indicator lights.

### 2.2. Vehicle Detection
- Use two vehicle detection sensors (B5 and B6).
- Detect vehicle presence in the garage entrance area.
- Support garage occupancy monitoring.

### 2.3. Automatic Garage Door Control
- Control the garage entrance door using motor M5.
- Support access control through an external card-operated switch (S10).
- Provide an internal manual door-opening switch (S11).

### 2.4. Status Monitoring
- Use indicator lights to display ventilation and garage operating conditions.
- Monitor the system through PLC digital inputs and outputs.

## 3. Hardware and Software

| Component | Description |
|---|---|
| PLC | Siemens S7-1200 CPU 1214C DC/DC/DC |
| Programming software | Siemens TIA Portal |
| Power supply | 24V DC |
| Sensors | Airflow sensors and vehicle detection sensors |
| Actuators | 4 ventilation fan motors and 1 garage door motor |
| Control devices | Push buttons and switches |
| Indicators | Signal lamps P1–P5 |

## 4. System I/O Configuration

### Digital Inputs

| Address | Symbol | Description |
|---|---|---|
| I0.0 | S0 | Main control button |
| I0.1 | S1 | Fan 1 ON |
| I0.2 | S2 | Fan 1 OFF |
| I0.3 | S10 | External garage door opening |
| I0.4 | S11 | Internal garage door opening |
| I1.0 | B1 | Fan 1 airflow sensor |
| I1.1 | B2 | Fan 2 airflow sensor |
| I1.2 | B3 | Fan 3 airflow sensor |
| I1.3 | B4 | Fan 4 airflow sensor |
| I1.4 | B5 | Vehicle detection sensor 1 |
| I1.5 | B6 | Vehicle detection sensor 2 |

### Digital Outputs

| Address | Symbol | Description |
|---|---|---|
| Q0.0 | Fan 1 | Fan 1 contactor |
| Q0.1 | Fan 2 | Fan 2 contactor |
| Q0.2 | Fan 3 | Fan 3 contactor |
| Q0.3 | Fan 4 | Fan 4 contactor |
| Q0.4 | M5 | Garage door motor control |
| Q0.5 | P1 | Ventilation status indicator |
| Q0.6 | P2 | Ventilation status indicator |
| Q0.7 | P3 | Ventilation status indicator |
| Q1.0 | P4 | Garage status indicator |
| Q1.1 | P5 | Garage status indicator |

*Note: The I/O table above follows the provided electrical connection diagram. The complete system design also includes individual ON/OFF switches for the remaining ventilation fans.*

## 5. System Architecture

The system consists of three main functional groups:

1. **Input Layer:** Push buttons, airflow sensors, and vehicle detection sensors collect operating conditions and operator commands.
2. **Control Layer:** Siemens S7-1200 PLC processes input signals and executes the control program.
3. **Output Layer:** Contactors, motors, and indicator lights perform the corresponding control actions and display system status.

## 6. Simulation

The project is designed for PLC programming and simulation in Siemens TIA Portal.

The simulation focuses on:
- Digital input/output operation.
- Individual ventilation fan control.
- Sensor signal monitoring.
- Garage door control.
- Indicator light operation.
- PLC control logic verification.

## 7. Skills Demonstrated

- Siemens S7-1200 PLC programming.
- TIA Portal development and simulation.
- Digital I/O configuration and addressing.
- Industrial electrical control fundamentals.
- Sensor and actuator integration.
- Motor control using contactors.
- PLC-based automation system design.

## 8. Project Scope

This project is an educational automation simulation intended to demonstrate PLC control logic, electrical I/O configuration, and integration of sensors and actuators in a garage management application.

---

**Technologies:** Siemens S7-1200 | TIA Portal | PLC Programming | Industrial Automation
