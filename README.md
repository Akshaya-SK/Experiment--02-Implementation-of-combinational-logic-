# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 ## NAME: AKSHAYA S K
 ## REGISTER NUMBER:212223040011
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
 Hardware – PCs, Cyclone II , USB flasher
 Software – Quartus prime


## Theory
 A combinational circuit is a circuit in which the output depends on the present combination of inputs. Combinational circuits are made up of logic gates. The output of each logic gate is determined by its logic function. Combinational circuits can be made using various logic gates, such as AND gates, OR gates, and NOT gates.

## Procedure

## Program:
```
module ex_02(a,b,c,d,f1);
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

## RTL realization
![293328819-0b10e8d3-3edb-4adb-8b8a-37017a8b2e87](https://github.com/Akshaya-SK/Experiment--02-Implementation-of-combinational-logic-/assets/149347593/f1485473-21e7-4c64-a9c0-8588164b60ae)

## Output:
## RTL
![293328819-0b10e8d3-3edb-4adb-8b8a-37017a8b2e87](https://github.com/Akshaya-SK/Experiment--02-Implementation-of-combinational-logic-/assets/149347593/3f1b2203-97f7-4ef5-91e2-e618f179c90b)

## TRUTH TABLE
![Uploading 293330224-0a3bc6fb-6b81-47b3-81f2-83403e6d5db8.png…]()

## Timing Diagram
![Uploading 293330449-dd2320c7-7c99-48df-833b-18d01e1e0e00.png…]()

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
