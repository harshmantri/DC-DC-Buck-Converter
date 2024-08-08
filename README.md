# DC-DC-Buck-Converter
### Project Overview
This project involves the design and hardware implementation of a Buck Converter using the TL494 PWM generator IC. This was a group project that was done in the Power Electronics Course.
### Problem Statement
Design a Buck Converter with the following specifications:
* Input Voltage: 15 V
* Output Voltage: 10 V
* Switching Frequency: 10 kHz
* Output Current: 1 A

The project includes generating waveforms of inductor current and switch voltage in Continuous Conduction Mode (CCM) and demonstrating Discontinuous Conduction Mode (DCM) by changing the load resistance.
### Components and Equipment <br>
* Drive Circuit (TL494 PWM generator IC ): Generates the pulse width modulated signal to control the transistor.
* MOSFET: Acts as a high-speed switch controlled by the PWM.
* Diode: Provides a path for the inductor current when the switch is off.
* Inductor: Stores energy and helps in smoothing the current.
* Capacitors: Filters the output to reduce voltage ripple.
* Resistors: Used for sensing and feedback purposes.
* MOSFET driver: To connect the TL494 board and drive circuit.
* Rheostat: To change load resistance.
* Oscilloscope: To observe waveforms.
### Key Concepts
* #### Continuous Conduction Mode (CCM)
CCM occurs when the current through the inductor never falls to zero during the switching cycle. This mode is characterized by continuous current flow in the inductor.
* #### Discontinuous Conduction Mode (DCM)
DCM occurs when the current through the inductor falls to zero during part of the switching cycle. This mode is characterized by intermittent current flow in the inductor.
### Circuit Design
* #### TL494 PWM generator IC
The TL494 board generates the pulses for the DC-DC PE converters. Here is the connection diagram for the same:
![PWM(TL494)](https://github.com/user-attachments/assets/ed417843-2331-4d2c-89ca-3398a6cf3470)
* #### Interface circuit to driver IC
This connects the driver IC to the output obtained from the TL494 board. The circuit diagram for the same is shown below. 
![Screenshot 2024-08-08 191120](https://github.com/user-attachments/assets/c6dddce7-a381-4c9b-a536-b909715ed304)

* #### Buck Converter Circuit
A Buck Converter, or a step-down converter, is a DC-DC converter that steps down the voltage from its input to its output.

![Screenshot 2024-08-08 191145](https://github.com/user-attachments/assets/a6068b47-a1a6-41a9-b300-d3d385a25ba6)![buck_converter](https://github.com/user-attachments/assets/f490e202-5ef3-4427-a440-900cd9d5c56b)

### Implementation Steps
* *Circuit Design*: Design the circuit according to the specifications. Ensure that the components are rated for the required voltages and currents.
* *Component Selection*: Select appropriate components such as MOSFETs, diodes, inductors, and capacitors.
* *PCB Layout*: Design the PCB layout to ensure minimal noise and optimal performance.
* *Assembly*: Assemble the circuit components on the PCB.
* *Testing*: Test the circuit under various load conditions to verify performance in both CCM and DCM.
### Waveforms and Analysis
* *Gate Pulses*: The gate pulse (PWM output) waveform is shown in yellow.
* *Inductor Current & Switch Voltage*: The inductor Current & switch voltage is shown in blue.
#### Waveforms in CCM
* The resistance is around 20 ohms for stable graphs; correspondingly, we get the current as 1.0 A. The output voltage varies between 9-10V (due to nonidealities).

![ccm](https://github.com/user-attachments/assets/ce9ed58c-50f1-469d-9df3-db629a79b63e)

#### Waveforms in DCM
* We obtained DCM around 3kHz frequency.

![dcm](https://github.com/user-attachments/assets/d3b9c4eb-9fda-462a-ba82-b3ef844cbeda)

#### Switch Voltage

![switch_voltage](https://github.com/user-attachments/assets/4869adbf-6188-44d2-b62b-c2926a069661)

### Results and Observations
* Voltage Conversion: Successfully converted a 15V input to a stable 10V output with an output current of 1A.
* Mode Control: Demonstrated effective control and operation in both CCM and DCM.
* Precise PWM Control: The TL494 module provided precise PWM control, ensuring efficient and reliable performance of the buck converter.
### Conclusion
This project effectively showcased the ability to design, implement, and test a DC-DC buck converter using the TL494 module. The experience gained from this project will be valuable for future endeavors in power electronics and control systems.
### Complete Setup
![complete setup](https://github.com/user-attachments/assets/1986e3cb-5a9c-470c-a79e-2a0bf7b1006e)
