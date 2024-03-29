# A 4-week Research Internship on RISC-V using VSDSquadron Mini RISC-V Dev Board

BOARD SPECS:

| CH32V003F4U6 chip with 32-bit RISC-V core based on RV32EC instruction set |
| ------------------------------------------------------------------------- 
| SRAM                                                                       2kb onchip volatile sram     16kb external program memory                                    |
| Processor                                                                  24 MHz                                                                                       |
| Sink Current per I/O Pin                                                   8 mA                                                                                         |
| Source Current per I/O Pin                                                 8 mA                                                                                         |
| Input voltage (nominal)                                                    5 V                                                                                          |
| I/O voltage                                                                3.3 V                                                                                        |
| Programmer/debugger                                                        Onboard RISC-V programmer/debugger, USB to TTL serial port support                           |
| SPI                                                                        1x, PC5(SCK), PC1(NSS), PC6(MOSI), PC7(MISO)                                                 |
| I2C                                                                        1x, PC1(SDA), PC2(SCL)                                                                       |
| USART                                                                      1x, PD6(RX), PD5(TX)                                                                         |
| External interrupts                                                        8 external interrupt edge detectors, but it only maps one external interrupt to 18 I/O ports |
| PWM pins                                                                   14X                                                                                          |
| Analog I/O pins                                                            10-bit ADC, PD0-PD7, PA1, PA2, PC4                                                           |
| Digital I/O pins                                                           15                                                                                           |
| Built-in LED Pin                                                           1X onboard user led (PD6)                                                                    |
| USB 2.0 Type-C                                                            
   

This repo is intended to document the weekly progress.


<details>
    <summary> TASK 1 </summary>

### The first online meet was held on 16th of Feb 2024 @6PM

1) install RISC-V GNU Toolchain 

2) install Yosys 

3) install iverilog 

4) install gtkwave

</details>	
	<details>
    <summary> TASK 2 </summary>
		
### The 2nd online meet was held on 20th of Feb 2024 @6PM

Identify Input ports, input waveforms, output ports and output waveforms for your design.

PROJECT SELECTED: Universal Asynchronous Receiver Transmitter protocol based on hardware transmitter 

# What is Universal Asynchronous Receiver Transmitter?

--> Universal asynchronous reciver / transmitter also know as UART. 
--> Protocol for exchanging serial data between two devices.
--> Uses only two wires 
    - TX to RX (each direction) 
--> Can be simplex, half duplx or full duplex 
    - Simples; in this data is sent in one direction only. 
    - half duplex; in this each side communicate but only one at a time.
    - full duplex; in this both side can transmit at the same time.
--> Data is transmitted as frames.

<img width="529" alt="image" src="https://github.com/arjitsaxena07/VSD-INTERNSHIP-/assets/83625986/89c9576f-fede-440e-a8d4-b273fa945696">

## Input Waveform 
<img width="905" alt="image" src="https://github.com/arjitsaxena07/VSD-INTERNSHIP-/assets/83625986/c217b747-4f65-49bc-89fb-d836be2ac4bc">

## Output Waveform
<img width="956" alt="image" src="https://github.com/arjitsaxena07/VSD-INTERNSHIP-/assets/83625986/dd5b2ffa-fbfb-462b-ad0a-65257a1a15eb">

</details>	
	<details>
    <summary> TASK 3 </summary>

###  The 3rd online meet was held on 22nd of Feb 2024 @6PM
Task: Basics of Functional Simulation. Upload lab snapshots from iverilog and gtkwave. 
