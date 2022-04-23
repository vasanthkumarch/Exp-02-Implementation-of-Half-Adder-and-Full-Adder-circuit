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
Developed by: Jagan a
RegisterNumber:212221230037

Half adder program:

module fulladd (a,b,sum,carry);
input a,b;
output sum,carry;
assign sum = (a^b);
assign carry = (a&b);
endmodule

Full adder program:

module fulladd (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = (a^b^c);
assign carry = ((a&b)|(a^b)&c);
endmodule
*/
Logic symbol & Truthtable
RTL realization

### Output:
### RTL:
Half adder:
![ha](https://user-images.githubusercontent.com/59290560/164895183-cf210728-cf36-43c1-ab2c-3e9fdfa29563.png)

full adder:
![fa](https://user-images.githubusercontent.com/59290560/164895201-2e43a558-c9fa-4fb0-a70a-c5c925274a70.png)


### TIMING DIAGRAM
Half adder:
![timing diagram ha](https://user-images.githubusercontent.com/59290560/164895288-11432b87-ea38-4407-8725-149daa8c09b2.png)

Full adder:
![timing diag fa](https://user-images.githubusercontent.com/59290560/164895316-2c188944-db35-4a0b-8c60-fd196a3652f8.png)


### TRUTH TABLE 
Half adder:
![tt ha](https://user-images.githubusercontent.com/59290560/164895238-d1881bdb-256f-4f44-becc-090b6461e32a.png)

Full adder:
![tt fa](https://user-images.githubusercontent.com/59290560/164895252-d62e3e91-42b5-406a-98bf-8c7f8414e739.png)


### Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
