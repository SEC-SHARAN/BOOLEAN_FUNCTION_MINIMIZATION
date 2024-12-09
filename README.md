# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
module experiment2(a,b,c,d,f1,w,x,y,z,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b&~c)|(~a&b&d)|(a&b&~c));
assign f2=((~y&z)|(x&y)|(w&y));
endmodule
```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: SHARAN S
RegisterNumber:24900120


**RTL realization**
![Screenshot 2024-12-09 103624](https://github.com/user-attachments/assets/bebe87b6-5a85-4e10-a7c6-4a5de7185e4e)

**Output:**

**RTL**

**Timing Diagram**
![Screenshot 2024-12-09 103653](https://github.com/user-attachments/assets/04d3ad9d-7d18-471b-a73f-1c8c102626ff)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

