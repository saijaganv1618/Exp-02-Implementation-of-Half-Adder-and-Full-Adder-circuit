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
Developed by: Jagan.a
RegisterNumber: 212221230037
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
![ha](https://user-images.githubusercontent.com/59290560/164895440-2949b321-df1a-4320-987c-5f46b7011797.png)

Full adder:
![fa](https://user-images.githubusercontent.com/59290560/164895457-f2d79b60-4096-4f6d-a00c-b700067b8732.png)

### TIMING DIAGRAM:
Half adder:
![timing diagram ha](https://user-images.githubusercontent.com/59290560/164895517-c8a1762c-f14a-43f0-a80f-1904bd6bf39e.png)


Full adder:
![timing diag fa](https://user-images.githubusercontent.com/59290560/164895521-c3a4d5f8-9dd3-4fda-9255-355a0d3763c7.png)



### TRUTH TABLE: 
Half adder:
![tt ha](https://user-images.githubusercontent.com/59290560/164895486-70df18c0-a6ec-428a-ac2b-f622909289e4.png)

Full adder:
![tt fa](https://user-images.githubusercontent.com/59290560/164895496-19d85047-4930-4ad7-b23a-307a20d584ea.png)




### Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
