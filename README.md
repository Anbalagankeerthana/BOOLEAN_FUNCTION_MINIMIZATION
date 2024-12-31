# EXP 2: BOOLEAN_FUNCTION_MINIMIZATION
# DATE : 3rd OCT 2024
**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
Boolean Function Minimization is the process of reducing a Boolean expression to its simplest form without changing its functionality. This minimization reduces the number of gates and inputs required, optimizing circuit design.

Logic Gates: Fundamental building blocks like AND, OR, and NOT gates are used to implement Boolean expressions. Karnaugh Map (K-map): A graphical technique for minimizing Boolean expressions by grouping terms based on commonalities. The given Boolean functions can be minimized as follows:

F1 = A’B’C’D’ + AC’D’ + B’CD’ + A’BCD + BC’D The terms can be simplified using K-map techniques to reduce the complexity of the circuit. F2 = xy’z + x’y’z + w’xy + wx’y + wxy Similar simplification can be done for this function to reduce the gate count. The resulting minimized expressions are implemented using Verilog HDL and simulated on the Quartus Prime tool. The outputs can then be verified on an FPGA board (e.g., Cyclone II).

**Logic Diagram**
![{93B168F8-5775-49F7-A14D-C5F19FC6369F}](https://github.com/user-attachments/assets/5d0cdb8f-1b0b-437b-81e9-9ecc9fde6a7d)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
```
module exp2(a,b,c,d,f1,w,x,y,z,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b&~d)|(~a&b&d)|(a&b&~c));
assign f2=((~y&z)|(x&y)|(w&y));
endmodule
```

Developed by:keerthana A  RegisterNumber:24900259


**RTL realization**
![398568829-090e9d0a-2f43-4497-90b8-78621fb69f7c](https://github.com/user-attachments/assets/c1109d0b-41ca-4d11-95ab-5f34fd02bdf9)

**Output:**
![398569399-ccece52c-e2f1-4705-943f-6fb14bc6fef8](https://github.com/user-attachments/assets/1f39845c-847f-4ebc-bbf7-f99b7c54030d)

**RTL**
![exp2 rtl](https://github.com/user-attachments/assets/41683677-0d0f-4fc7-9f0a-e55d50dc1f50)

**Timing Diagram**
![exp2 time](https://github.com/user-attachments/assets/6f96abe4-7de6-4fe7-aabc-6501c574fe12)
**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

