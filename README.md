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
```
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: S.Shanmathi
RegisterNumber: 212222100049
# FULL ADDER:
module add(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum =(a^b^c);
assign carry =((a&b)|(a^b)&c);
endmodule
# HALF ADDER
module add(x,y,s,c);
input x,y;
output s,c;
xor(s,x,y);
and(c,x,y);
endmodule
```
*/
Logic symbol & Truthtable
RTL realization

### Output:
## RTL
# FULL ADDER:
![image](https://user-images.githubusercontent.com/121243595/234776534-2babd134-d77c-421c-927d-d0ff1c6e1fc2.png)

# HALF ADDER:
![image](https://user-images.githubusercontent.com/121243595/234779032-46311d2b-d843-4352-9c87-b97e0737155d.png)

### TIMING DIAGRAM
# FULL ADDER:
![image](https://user-images.githubusercontent.com/121243595/234778400-d27e7d89-fee5-456a-a037-47a53c74c0fd.png)
# HALF ADDER:
![image](https://user-images.githubusercontent.com/121243595/234779373-0cecf3b3-9db2-4da4-bc06-32b15f837f24.png)


### TRUTH TABLE 
# FULL ADDER:
![image](https://user-images.githubusercontent.com/121243595/234778696-b3334407-4c60-43f3-bd11-2c43a4ba0c33.png)
# HALF ADDER:
![image](https://user-images.githubusercontent.com/121243595/234780160-83b4cad7-01b7-463f-8c67-381cc5fcbc81.png)

### Result:
Therefore,half adder and full adder is verified
