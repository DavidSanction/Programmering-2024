# Vejledning til studerende

I dette dokument skal du i grove træk beskrive din løsning til milepælsopgaven.

I skal kunne beskrive hvilke komponenter der er i basen, hvilket går i sektionen komponentliste.

Derefter skal i beskrive basen. Dvs. besvar hvilke komponenter bliver brugt til hvad? 

Hvordan er det blevet brugt? F.eks. hvilke funktioner giver det,

Hvad var udfordringerne undervejs i at få komponenterne til at virke?

Hvad virker godt/er du stolt af at have bygget?

Det i skriver i journalmappen er jeres uge til uge reflektioner, så dette Milepælsdokument er en opsamling til det hele, en oversigt. Dette dokument skal ikke være mere end 1 side eller 2, mens journalen er mere detaljeret.

## Opgave 1 - Base - Milepælsopgave

### Komponentliste

- **2x VXE 103450 3.7V 1800mAh Lipo Polymer Lithium Rechargeable Battery**
- **2x XL4005 5A DC-DC Step-Down Converter**
- **1x PCB**
- **2x L9110S H-Bridge Dual DC Stepper Motor Driver Controller**
- **4x DC Gear Motor 3V - 6V + Wheels**
- **1x ESP32 DevKit Udviklingsboard**

### Beskrivelse af basen

**3D Printed Acrylic/Plastic Base/Chassis for a Four-Wheeled Remote Controlled, Semi-Autonomous Rover**

### Material
The base is constructed from 3D printed acrylic or plastic.

### Design
The chassis is designed to accommodate four wheels, with mounting points for the components.

### Motors
- **Type**: Four DC gear motors are used, each capable of operating at 3V to 6V. These motors drive the wheels and provide the necessary torque for movement.

### Motor Drivers
- **Model**: Two L9110S H-Bridge dual DC motor driver controllers are employed. Each driver can control two motors.
- **Function**: These drivers receive control signals from the microcontroller and manage the direction and speed of the motors.

### Power Supply
- **Batteries**: Two VXE 103450 3.7V 1800mAh Lipo Polymer Lithium rechargeable batteries provide the primary power source for the rover.
- **Voltage Regulation**: Two XL4005 5A DC-DC step-down converters are used to step down the battery voltage to levels suitable for the motors and control electronics.

### Control Unit
- **Microcontroller**: An ESP32 DevKit serves as the central control unit, handling all processing and control tasks.
- **Programming**: The ESP32 is programmed to manage motor control, sensor inputs, and communication protocols, enabling both remote control and semi-autonomous operation.

### Sensors (Optional)
- **VL53L0X Time-of-Flight Sensor**: Provides precise distance measurements using laser-based time-of-flight technology, useful for obstacle detection and navigation.
- **HC-SR04 Ultrasonic Sensor**: Uses ultrasonic waves to measure distance to objects, aiding in obstacle avoidance.

### Joystick Controller (Optional)
- **Function**: Allows for manual control of the rover. The joystick sends control signals to the ESP32, which then adjusts the motor drivers accordingly.

### System Functionality

#### Power Distribution
The Lipo batteries supply power to the entire system. The step-down converters regulate this power, ensuring that the ESP32 and motor drivers receive the correct voltage and stable current.

#### Motor Control
The ESP32 sends PWM (Pulse Width Modulation) signals to the L9110S motor drivers, which then control the speed and direction of the DC motors. This allows the rover to move forward, backward, and turn.

#### Remote Control
The built-in Wi-Fi and Bluetooth capabilities of the ESP32 enable remote control of the rover. Commands can be sent from a smartphone, computer, or joystick controller to control the rovers movements.

#### Semi-Autonomous Operation
The ESP32 can be programmed for obstacle avoidance, path following, or other autonomous behaviors based on sensor inputs from the VL53L0X or HC-SR04 sensors.
