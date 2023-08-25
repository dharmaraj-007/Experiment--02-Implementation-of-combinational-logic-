# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

 

 
## Components Required:
1. Hardware – PCs, Cyclone II , USB flasher
2. Software – Quartus prime


## Theory:
 Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.

# Using AND gate:
  An AND gate is a fundamental digital logic gate that performs a logical conjunction on its input signals. It produces an output signal only when all of its input signals are high (logic level 1). If any of the input signals is low (logic level 0), the output of the AND gate remains low.
# using NOT gate:
A NOT gate, also known as an inverter, is a basic digital logic gate that performs the operation of negation on its input signal. In other words, it produces the opposite (complementary) output to its input. If the input is high (logic level 1), the output will be low (logic level 0), and if the input is low, the output will be high.
# using OR gate:
An OR gate is a fundamental digital logic gate that performs a logical disjunction on its input signals. It produces an output signal when at least one of its input signals is high (logic level 1). The output remains low only if all input signals are low (logic level 0).

## Procedure
```
1.Create a project with required entities.
2.Create a module along with respective file name.
3.Run the respective programs for the given boolean equations.
4.Run the module and get the respective RTL outputs.
5.Create university program(VWF) for getting timing diagram. 
6.Give the respective inputs for timing diagram and obtain the results.
```

## Program:
```
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: Dharmaraj S
RegisterNumber:  212222240025

module expression(a,b,c,d,f1);
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

## RTL diagram:
![de exp2 rtl](https://github.com/dharmaraj-007/Experiment--02-Implementation-of-combinational-logic-/assets/119560386/077f9fb4-2b9c-426c-a129-9160c5a87145)

## Truth Table:
![TT exp2](https://github.com/dharmaraj-007/Experiment--02-Implementation-of-combinational-logic-/assets/119560386/575af471-19fd-4bd2-a862-87c6e105e900)

## Output waveform:
![waveform ouput](https://github.com/dharmaraj-007/Experiment--02-Implementation-of-combinational-logic-/assets/119560386/8b92b2aa-e4b7-45ad-8909-5f43206260d5)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
