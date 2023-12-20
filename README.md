# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program: 
/*
~~~
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: M.suren.
RegisterNumber: 23005055
half adder
module digitalexpthree(A,B,sum,carry)
input A,B;
output sum,carry;
xor(sum,A,B);
and(carry,A,B);
endmodule

full adeer
module digitalexpthreeone(A,B,sum,carry)
input A,B,C;
output sum,carry;
assign sum = ((A^B)^C);
assign carry = ((A&B) | (B&C) | (C&A));
endmodule
~~~
*/
RTL realization

half adder

![digital exp-three half-adder](https://github.com/Msuren48106/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/150503875/40d20cd9-c389-47a6-a95f-821b36e0e205)

full adder

![digital exp-three full-adder](https://github.com/Msuren48106/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/150503875/c1ebdf75-9378-466b-9760-9626490f2a76)
### TIMING DIAGRAM

### TRUTH TABLE 

### Result:
The design of the half adder and full adder is sucesfully proved
