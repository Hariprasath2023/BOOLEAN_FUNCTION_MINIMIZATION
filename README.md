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

module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);

input A,B,C,D,W,X,Y,Z;

wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;

output F1,F2;

assign x1=(~A)&(~B)&(~C)&(~D);

assign x2=(A)&(~C)&(~D);

assign x3=(~B)&(C)&(~D);

assign x4=(~A)&(B)&(C)&(D);

assign x5=(B)&(~C)&(D);

assign x6=(X)&(~Y)&(Z);

assign x7=(~X)&(~Y)&(Z);

assign x8=(~W)&(X)&(Y);

assign x9=(W)&(~X)&(Y);

assign x10=(W)&(X)&(Y);

assign F1=x1|x2|x3|x4|x5;

assign F2=x6|x7|x8|x9|x10;

endmodule

Developed by: RegisterNumber:*/ VISAL R    24008707


**RTL realization**
![logic diagram](https://github.com/user-attachments/assets/b1649a3d-5a12-4de4-81e6-b8f82a1c3dd9)

**LOGIC SYMBOL & Truthtable**
![tabular collum](https://github.com/user-attachments/assets/569793be-c7e0-4f9a-ae86-79ce0451109d)
![output table](https://github.com/user-attachments/assets/0fec166c-9abc-4c7b-a190-254f734e594f)

**OUTPUT:**
![output](https://github.com/user-attachments/assets/e62d591c-0bfb-4ceb-8a2e-ee78a37dbba8)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

