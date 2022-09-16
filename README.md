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
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: DHANASHREE M
RegisterNumber:  212221230018
# HALF ADDER:
module EX2(A,B,sum,carry); 

input A,B; 

output sum,carry; 

xor(sum,A,B); 

and(carry,A,B); 

endmodule

# FULL ADDER:
module ex02(a,b,c,Sum,Carry);

input a,b,c; 

output Sum,Carry; 

assign Sum = ((a^b)^c);

assign Carry = ((a&b) | (b&c) | (c&a));

endmodule
*/
### Output:
HALF ADDER:
### RTL:
![Screenshot 2022-09-13 173126](https://user-images.githubusercontent.com/94165415/190642541-59477662-c2f6-4e87-8803-67f9ccb77492.png)
### TIMING DIAGRAM:
![TIME 1](https://user-images.githubusercontent.com/94165415/190645041-daa926be-b34e-40b7-88d5-8bbc1ef3d41c.png)
### TRUTH TABLE :
![truth table 1](https://user-images.githubusercontent.com/94165415/190644955-71669604-0b51-47e3-b5af-00e74a2267e3.png)
FULL ADDER:
### RTL:
![Screenshot 2022-09-16 181110](https://user-images.githubusercontent.com/94165415/190645163-8db49b97-2a14-4f7d-99a1-a5f5f711fa5e.png)
### TRUTH TABLE:
![truth table 2](https://user-images.githubusercontent.com/94165415/190645214-9f3332b6-d273-4267-98b3-c53d91546a6d.png)
### TIMING TABLE:
![TIME 2](https://user-images.githubusercontent.com/94165415/190645434-87defa9d-8f93-4a6b-8d9f-8d2a0204a225.png)

### Result:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming is successfully done.
