# Experiment--02-Implementation-of-combinational-logic

### Name: Nijeesh NJ 
### RegisterNumber: 23010565

Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
#### Equipments Required: Hardware – PCs, Cyclone II , USB flasher
#### Software – Quartus prime


## Theory
 

## Logic Diagram
## Procedure
## Program:

Program to implement the given logic function and to verify its operations in quartus using Verilog programming.

module combinationalcircuit(f1,a,b,c,d);

input a,b,c,d;

output f1;

wire abar,bbar,cbar,dbar,x1,x2,x3,x4,x5;

assign abar=~a;

assign bbar=~b;

assign cbar=~c;

assign dbar=~d;

assign x1=abar&bbar&cbar&dbar;

assign x2=a&cbar&dbar;

assign x3=bbar&c&dbar;

assign x4=abar&b&c&d;

assign x5=b&cbar&d;

assign f1=x1|x2|x3|x4|x5;

endmodule

## Truth Table 
![image](https://github.com/Nijeesh-bit/Experiment--02-Implementation-of-combinational-logic-/assets/89188014/db13e505-3f57-4d10-b742-bfd8d44c944f)

## Wave Form
![image](https://github.com/Nijeesh-bit/Experiment--02-Implementation-of-combinational-logic-/assets/89188014/02ab5c60-9b8e-4e63-81e2-9e9d818fc869)

## RTL realization
![image](https://github.com/Nijeesh-bit/Experiment--02-Implementation-of-combinational-logic-/assets/89188014/1ff8f21c-94cc-4ef9-b0f8-d2d18dfa68d1)

## Output:
## RTL
## Timing Diagram
## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
