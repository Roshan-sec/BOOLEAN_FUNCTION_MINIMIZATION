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
~~~
input a,b,c,d;

output f1;

assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));

endmodule

module funct2(w,x,y,z,f2);

input w,x,y,z;

output f2;

assign f2=((~y & z)|( w & y )|(x & y));
~~~

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber:212225240123


**RTL realization**
<img width="461" height="316" alt="image" src="https://github.com/user-attachments/assets/0f7153a7-f8e9-440b-8ee1-bd795b7353d1" />


**RTL**
<img width="780" height="447" alt="image" src="https://github.com/user-attachments/assets/7f12179d-f970-4966-8fb9-4e9c95401fa9" />


**Timing Diagram**
<img width="1914" height="517" alt="image" src="https://github.com/user-attachments/assets/12414e06-dde6-495b-a9ce-285dd7fff3ce" />

<img width="1917" height="662" alt="image" src="https://github.com/user-attachments/assets/bfcbeeb6-93f7-47e5-ae15-d8f968998492" />


**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

