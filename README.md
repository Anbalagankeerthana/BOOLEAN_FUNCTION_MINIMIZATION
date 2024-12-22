![exp2 time](https://github.com/user-attachments/assets/baa46d00-93c0-448a-9475-48a2551f1a7a)![image](https://github.com/user-attachments/assets/fee89a67-ebde-4c12-918b-c1f09c6b5bd4)# BOOLEAN_FUNCTION_MINIMIZATION

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


**Output:**

**RTL**
![exp2 rtl](https://github.com/user-attachments/assets/41683677-0d0f-4fc7-9f0a-e55d50dc1f50)

**Timing Diagram**
![exp2 time](https://github.com/user-attachments/assets/6f96abe4-7de6-4fe7-aabc-6501c574fe12)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

