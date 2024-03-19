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
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
```
module booleanfunction_top(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u;
not(adash,a);
not(bdash,b);
not(cdash,c);
not(ddash,d);
not(ydash,y);
and(p,bdash,ddash);
and(q,adash,b,d);
and(r,a,b,cdash);
or(f1,p,q,r);
//type code for f2 as like f1
endmodule
```
Developed by:John Paul J 
RegisterNumber:212223230093


**Truth Table**
![image](https://github.com/JOHNSUBIK/BOOLEAN_FUNCTION_MINIMIZATION/assets/150279319/57bf201f-fced-46eb-85ac-bcb52e7d62b5)


**Output:**

**RTL**
![Screenshot 2024-03-19 205350](https://github.com/JOHNSUBIK/BOOLEAN_FUNCTION_MINIMIZATION/assets/150279319/61d06911-f8f9-4e6b-88b1-380dcd6307d3)


**Timing Diagram**
![Screenshot (21)](https://github.com/JOHNSUBIK/BOOLEAN_FUNCTION_MINIMIZATION/assets/150279319/d901d54a-f59b-45a0-a381-4ca11ed69d7a)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

