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

/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: PAVITHRA Y
RegisterNumber:  212222050043

##Program 1:

module expfour(a,b,c,d,f);

input a,b,c,d;

output f;

wire f1,f2,f3;

assign f1 = (~c&~b&~a);

assign f2 = (~d&~c&~a);

assign f3 = (c&~(~b)&~a);

assign f= f1&~f2&~f3;

endmodule


PROGRAM 2:

module expfourtwo(a,b,c,d,f);

input a,b,c,d;

output f;

wire f1,f2,f3,f4;

assign f1 = c&(~b)&a;


assign f2 = d&(~c)&a;

assign f3 = c&(~b)&a;

assign f4 = ~(f1|f2|f3);

not(f,f4);

endmodule


*/
## RTL realization:


OUTPUT:
PEOGRAM 1
![program 1 RTL](https://user-images.githubusercontent.com/128951583/233844012-4eae7b07-b427-4bd1-9966-d6a18a01a6e6.jpg)

#PROGRAM 2:
![program 2 RTL](https://user-images.githubusercontent.com/128951583/233844053-8b0f776e-ccf7-464d-9bd2-57edcf899e30.jpg)

#TRUTH TABLE:
PROGRAM 1:
![program 1 Truth table](https://user-images.githubusercontent.com/128951583/233844275-d80737d3-b201-4225-a58c-2c2d66270825.jpg)

PROGRAM 2:
![program 2 Truth table](https://user-images.githubusercontent.com/128951583/233844310-a22d6460-542b-482c-95ab-ae5ef921629c.jpg)

## Timing Diagram:
PROGRAM 1:
![program 1 timing diagram](https://user-images.githubusercontent.com/128951583/233844142-5023af91-e01c-4eca-8020-d136f5b8ec48.jpg)

PROGRAM 2:
![program 2 timing diagram](https://user-images.githubusercontent.com/128951583/233844190-3a098866-7173-4127-a981-bd1291ca51c4.jpg)


## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
