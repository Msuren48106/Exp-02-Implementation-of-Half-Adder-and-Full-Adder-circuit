Name: M.suren.
Reg no: 23005055

# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit

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

![291158234-37dd987c-bada-4f79-addf-77c71c83b02a](https://github.com/Msuren48106/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/150503875/9e70a1f3-2b27-4617-88c1-9cb950de75a7)

full adder

![image](https://github.com/Msuren48106/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/150503875/112d22cf-2d65-4417-8d8d-661faf0db261)


## TIMING DIAGRAM

![image](https://github.com/Msuren48106/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/150503875/21e24a03-2418-4c26-83ca-ccda665b731e)

![image](https://github.com/Msuren48106/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/150503875/0fd78aeb-9f98-4c92-b2a6-3cd850cc7483)


### TRUTH TABLE 

![image](https://github.com/Msuren48106/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/150503875/037348a7-d944-459b-b11f-2edd7cfa7a17)

![image](https://github.com/Msuren48106/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/150503875/00faf599-8418-43e3-ab35-fff0c55d910e)


### Result:
The design of the half adder and full adder is sucesfully proved
