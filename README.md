# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
 

## Logic Diagram
## Procedure
1.Create a project with required entities.

2.Create a module along with respective file name.

3.Run the respective programs for the given boolean equations.

4.Run the module and get the respective RTL outputs.

5.Create university program(VWF) for getting timing diagram.

6.Give the respective inputs for timing diagram and obtain the results.
## Program:
/*
```
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by:Thenmohi P 
RegisterNumber:  212221230116
*/
module DE2(a,b,c,d,f1);
input a,b,c,d;
output f1;
wire x1,x2,x3,x4,x5;
assign x1=(~a)&(~b)&(~c)&(~d);
assign x2=(a)&(~c)&(~d);
assign x3=(~b)&(c)&(~d);
assign x4=(~a)&(b)&(c)&(d);
assign x5=(b)&(~c)&(d);
assign f1=x1|x2|x3|x4|x5;
endmodule
```
:
## RTL:
![d1](https://github.com/Thenmozhi-Palanisamy/Experiment--02-Implementation-of-combinational-logic-/assets/95198708/5ab2c60f-4580-4390-8c83-3c47e830b49c)

## Truth table
![image](https://github.com/Thenmozhi-Palanisamy/Experiment--02-Implementation-of-combinational-logic-/assets/95198708/b280551a-f504-449b-8050-3c61de9a5b15)

## output waveform
![d2](https://github.com/Thenmozhi-Palanisamy/Experiment--02-Implementation-of-combinational-logic-/assets/95198708/c5b83379-e0b6-42b9-b90d-8353134d814a)


## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
