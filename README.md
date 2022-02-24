# 4-Bit Ripple Carry Adder
### ABSTRACT:-
##### In this paper design of 4-Bit ripple carry adder is proposed using a CMOS  full adder cell. Multiple full adder circuits can be cascaded in parallel to add an N-bit number .For N-bit parallel adder , there must be N number of full adder circuits. A ripple carry adder is a logic circuit in which the carry out of each full adder is the carry in of the succeeding next most significant full adder.To understand the working of a ripple carry adder completely , you need to have a look at the full adder too.Full adder is a logic circuit that add two input operand bits plus a carry in bit and output a carry out bit and sum bit. I have implemented Ripple Carry Adder with the help of CMOS Full adder.
### INTRODUCTION:-
##### 4 full adder circuits can be cascaded in parallel to add an 4-bit number. For an 4-bit parallel adder, there must be 4  full adder circuits. A ripple carry adder is a logic circuit in which the carry-out of each full adder is the carry-in of the succeeding next most significant full adder. It is called a ripple carry adder because each carry bit gets rippled into the next  stage. In a ripple carry adder the sum and carry out bits of any half adder stage is not valid until the carry in of that stage occurs.Propagation delays inside the logic circuitry is the reason behind this. Propagation delay is time elapsed between the application of an input and occurance of the corresponding output. Consider a NOT gate, When the input is “0” the output will be “1” and vice versa. The time taken for the NOT gate’s output to become “0” after the application of logic “1” to the NOT gate’s input is the propagation delay here. Similarly the carry propagation delay is the time elapsed between the application of the carry in signal and the occurrence of the carry out (Cout) signal.To understand the working of full adder completely , you need to have a look at the full adder too. Full adder is a logic circuit that add two input operand bits plus carry out bit and sum bit. A full adder can be made by two half adder circuit together .Alternatively the full adder can be made using NAND or NOR logic.Below the schematic diagram of Full Adder to add 1-Bit.
#### FULL ADDER:-
##### To understand the working of ripple carry adder completely, you need to have a look at the Full Adder too. Full Adder is a Logic circuit that add two input operand bits plus a Carry in bit and output a Cout bit and Sum out bit. The Sum out (Sout) of a full adder is the Xor of input input operand bits A,B and the carry in (Cin) bit. truth table and schematic of a 1-bit full adder is shown below.
##### there is a simple trick to find result of a full adder . consider the second last row of the truth table, here the operand are 1,1,0 ie (A,B,Cin). Add them together ie 1+1+0=10. In binary system , the number order is 0,1,10,11.......and so the result of 1+1+0 is 10 just like we get 1+1+0=2 in decimal system. 2 in the decimal system corresponds to 10 in the binary sysyetm.
#### BLOCK DIAGRAM OF FULL ADDER


#### TRUTH TABLE


##### A basic Binary Adder circuit can be made from standard AND and XOR gates allowing us to "add" together two single bit binary number, A and B.
#### circuit diagram
#### Ripple Carry Adder:-
##### 4 full adder circuits can be cascaded in parallel to add an 4-bit number.
##### block diagram of Ripple Carry Adder
### Simulation in Synopsis Tool
