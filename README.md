# 4-Bit Ripple Carry Adder
### ABSTRACT:-
In this paper design of 4-Bit ripple carry adder is proposed using a CMOS  full adder cell. Multiple full adder circuits can be cascaded in parallel to add an N-bit number .For N-bit parallel adder , there must be N number of full adder circuits. A ripple carry adder is a logic circuit in which the carry out of each full adder is the carry in of the succeeding next most significant full adder.To understand the working of a ripple carry adder completely , you need to have a look at the full adder too.Full adder is a logic circuit that add two input operand bits plus a carry in bit and output a carry out bit and sum bit. I have implemented Ripple Carry Adder with the help of CMOS Full adder.
### Tools Used:
• Synopsys Custom Compiler:

The Synopsys Custom Compiler™ design environment is a modern solution for full-custom analog, custom digital, and mixed-signal IC design. As the heart of the Synopsys Custom Design Platform, Custom Compiler provides design entry, simulation management and analysis, and custom layout editing features. This tool was used to design the circuit on a transistor level.

• Synopsys Primewave:

PrimeWave™ Design Environment is a comprehensive and flexible environment for simulation setup and analysis of analog, RF, mixed-signal design, custom-digital and memory designs within the Synopsys Custom Design Platform. This tool helped in various types of simulations of the above designed circuit.

• Synopsys 28nm PDK:

The Synopsys 28nm Process Design Kit(PDK) was used in creation and simulation of the above designed circuit.
### INTRODUCTION:-
 4 full adder circuits can be cascaded in parallel to add an 4-bit number. For an 4-bit parallel adder, there must be 4  full adder circuits. A ripple carry adder is a logic circuit in which the carry-out of each full adder is the carry-in of the succeeding next most significant full adder. It is called a ripple carry adder because each carry bit gets rippled into the next  stage. In a ripple carry adder the sum and carry out bits of any half adder stage is not valid until the carry in of that stage occurs.Propagation delays inside the logic circuitry is the reason behind this. Propagation delay is time elapsed between the application of an input and occurance of the corresponding output. Consider a NOT gate, When the input is “0” the output will be “1” and vice versa. The time taken for the NOT gate’s output to become “0” after the application of logic “1” to the NOT gate’s input is the propagation delay here. Similarly the carry propagation delay is the time elapsed between the application of the carry in signal and the occurrence of the carry out (Cout) signal.To understand the working of full adder completely , you need to have a look at the full adder too. Full adder is a logic circuit that add two input operand bits plus carry out bit and sum bit. A full adder can be made by two half adder circuit together .Alternatively the full adder can be made using NAND or NOR logic.Below the schematic diagram of Full Adder to add 1-Bit.
#### FULL ADDER:-
To understand the working of ripple carry adder completely, you need to have a look at the Full Adder too. Full Adder is a Logic circuit that add two input operand bits plus a Carry in bit and output a Cout bit and Sum out bit. The Sum out (Sout) of a full adder is the Xor of input input operand bits A,B and the carry in (Cin) bit. truth table and schematic of a 1-bit full adder is shown below.
 there is a simple trick to find result of a full adder . consider the second last row of the truth table, here the operand are 1,1,0 ie (A,B,Cin). Add them together ie 1+1+0=10. In binary system , the number order is 0,1,10,11.......and so the result of 1+1+0 is 10 just like we get 1+1+0=2 in decimal system. 2 in the decimal system corresponds to 10 in the binary sysyetm.
#### BLOCK DIAGRAM OF FULL ADDER
#### ![block digram of full adder](https://user-images.githubusercontent.com/98162318/155466077-5086d4e5-27c4-4e92-969f-51ec3a03e042.jpg)
#### TRUTH TABLE
#### ![truth table](https://user-images.githubusercontent.com/98162318/155466455-53b4e1bd-4fce-41b3-b55c-ab9f3e9d515a.jpg)
##### A basic Binary Adder circuit can be made from standard AND and XOR gates allowing us to "add" together two single bit binary number, A and B.
#### circuit diagram
#### ![full adder](https://user-images.githubusercontent.com/98162318/155469394-6dd0ea48-a1e7-4858-ab5b-b705ae2d0a54.jpg)

####
#### Ripple Carry Adder:-
##### 4 full adder circuits can be cascaded in parallel to add an 4-bit number.
#### ![image](https://user-images.githubusercontent.com/98162318/155469872-79c37002-0f67-404f-b330-d539a8c77b8f.png)



### Simulation in Synopsis Tool
#### First i crate a INVERTER using CMOS
####Truth table of Not gate
![image](https://user-images.githubusercontent.com/98162318/155522496-3beac014-141e-4a1d-a087-b6648a7bb5cb.png)
#### Symbol of Inverter
![NOT_GATE](https://user-images.githubusercontent.com/98162318/155496184-9b1bba50-3d92-4d54-a7a6-4385ab2a6d86.png)
#### Schematic Diagram of Inverter
![NOT_Schematic](https://user-images.githubusercontent.com/98162318/155495030-477dec1b-93db-4dcf-9fd3-6bfd0b3190c4.png)
 ### XOR GATE
 #### Xor gate truth table
 ![image](https://user-images.githubusercontent.com/98162318/155521725-52c1f901-319a-446b-9ae8-51777d485224.png)


#### Xor Gate Symbol
![Xor_symbol](https://user-images.githubusercontent.com/98162318/155496784-872d4790-fa16-43d3-a44c-265c1f298f4f.png)
#### Xor Gate Schematic Diagram
![XOR_Schematic](https://user-images.githubusercontent.com/98162318/155496860-48569fe0-3c1e-46d5-ad8f-74d9b70ac024.png)

### NAND GATE:-
#### Truth table of NAND GATE
![image](https://user-images.githubusercontent.com/98162318/155520929-21b722cd-237c-49de-b003-0e06aa92df83.png)
#### Symbol of NAND Gate
![NAND_Symbol](https://user-images.githubusercontent.com/98162318/155498078-56e7e2a2-e9c9-4175-ae49-1052064004bd.png)
#### Schematic Diagram of NAND Gate
![NAND_Schematic](https://user-images.githubusercontent.com/98162318/155498088-49238e68-0db5-4c06-a23e-e49cbffe2e20.png)
### 1-Bit Full Adder
#### Schematic Diagram of 1-Bit Full Adder Using NAND Gate, NOT Gate, NOR Gate, XNOR Gate.

![1_Bit_Full_Adder1](https://user-images.githubusercontent.com/98162318/155498267-15247761-e004-4d5a-8983-0d83e4e39af9.png)
### Ripple Carry Adder
#### Schematic Diagram of 4-Bit Ripple Carry Adder.

![Screenshot from 2022-02-24 09-39-49](https://user-images.githubusercontent.com/98162318/155499027-f12c0e56-fcb0-4835-b4c0-ada249e81a48.png)
## RESULT

![result](https://user-images.githubusercontent.com/98162318/155503665-5730b947-6944-4a9c-9219-718bf1cdba9d.png)
### WAVEFORM OBSERVATIONS:-


![DocScanner 24-Feb-2022 5-26 pm](https://user-images.githubusercontent.com/98162318/155519794-504263ea-8132-46aa-9be3-ff2f694562a4.jpg)
	
# Acknowledgements:
• <a href='https://www.iith.ac.in/events/2022/02/15/Cloud-Based-Analog-IC-Design-Hackathon/'>Cloud Based Analog IC Design Hackathon</a></br>
• <a href='https://www.synopsys.com/'>Synopsys India</a></br>
• <a href='https://www.vlsisystemdesign.com/'>VLSI System Design (VSD) Corp. Pvt. Ltd India</a></br>



