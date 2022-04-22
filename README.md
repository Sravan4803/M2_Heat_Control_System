# embedded_systems_project--B Sravan Kumar

## Heat Control System 

### Theory

The heat control system is basically used to control the temperature of a car seat. When a user or driver of the car gets seated on a car, the button sensor gets activated. After that, the user gets access to turn on the heater. The temperature sensor keeps monitoring the temperature and sends the analog value to the microcontroller. The microcontroller processes the analog input of the temperature sensor and outputs a temperature value through serial communication. All the activities of the control system are done on a microcontroller called Atmega328.

### Simulation

The functionality of the heat control system is coded in embedded c and the working is demonstrated using simuation in a software called SimulIDE.
Below shows two images where in the 1st image shows the status of the simulation when the system is OFF and the second image shows the status of the system when it is ON. 

#### ON
![ON]![Simulation_ON](https://user-images.githubusercontent.com/101509869/164460202-388ece5f-6d09-4fb9-be7d-4b2365c79813.PNG)


#### OFF
![OFF]![Simulation_OFF](https://user-images.githubusercontent.com/101509869/164460405-4f6b9cde-5a50-4237-968e-d380518a396c.PNG)


#### Outputs

|Circuit|RAM Table|
|:--:|:--:|
![Circuit](https://user-images.githubusercontent.com/101509869/164460604-0f456f0d-7880-4daf-bfe6-b2209c53fb94.gif)|![RAM_table](https://user-images.githubusercontent.com/101509869/164460695-b5238126-daef-4fe5-9e41-56421080bff6.gif)|

|CRO|Serial Monitor|
|:--:|:--:|
![Oscilloscope](https://user-images.githubusercontent.com/101509869/164460743-64ef4c37-1883-4fb1-baa9-8571aa772c55.gif)|![Serial_Monitor](https://user-images.githubusercontent.com/101509869/164460781-8b1f1f48-6942-4c3f-8455-1ea909a8bfd0.gif)|


### Functionality 

* When the two switches are closed, the first LED glows indicating the actuation of the system and the heater.
* Next the analog input from the temperature sensor is received and digitized.
* The digitized temperature input is visualized using Pulse Width Modulation.
* The corresponding temperature values based on the digitized temperature input is transmitted by the UART protocol. Here the data is displayed on the serial monitor.

# Batches

|BULID|CPPCheck|C-CPP|Codacy|CodeQuality|CodeGrade|
|:--:|:--:|:--:|:--:|:----:|:----:|

[![Build-Linux](https://github.com/Sravan4803/M2_Heat_Control_System/actions/workflows/bulid_linux.yml/badge.svg)](https://github.com/Sravan4803/M2_Heat_Control_System/actions/workflows/bulid_linux.yml)|![Cppcheck Analyse](https://github.com/Sravan4803/M2_Heat_Control_System/actions/workflows/cppcheck.yml/badge.svg)](https://github.com/Sravan4803/M2_Heat_Control_System/actions/workflows/cppcheck.yml)

