# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
```
Developed by:Sharon Harshini L M

RegisterNumber:212223040193
```

```
module expno2(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(~A)&(~C)&(~D);
assign x3=(~B)&(~C)&(~D);
assign x4=(~A)&(~B)&(~C)&(~D);
assign x5=(~B)&(~C)&(~D);
assign F1=x1|x2|x3|x4|x5;
endmodule
```

**RTL Realization**

![image](https://github.com/user-attachments/assets/5abc9bac-0f0a-4d36-90c4-d1c612765140)


**Truthtable**
![image](https://github.com/user-attachments/assets/fb1ccf54-a22c-4f39-9f3b-fd7ce642c987)

**Timing Diagram**
![image](https://github.com/user-attachments/assets/e3d35e69-d89c-423c-a28b-337617f8f5ad)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

