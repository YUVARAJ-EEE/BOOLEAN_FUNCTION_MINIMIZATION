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
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```

Developed by: YUVARAJ M RegisterNumber: 212224050062


**RTL realization**
**Output:**
**RTL**

Boolean function minimization f1

![image](https://github.com/user-attachments/assets/35c2069b-49c5-43ba-925d-32cfd67a4c25)

![image](https://github.com/user-attachments/assets/acc828ab-d2e0-43bc-972c-538381f92630)






**Timing Diagram**
![image](https://github.com/user-attachments/assets/fb688224-b386-4378-ac42-8cee4eba380d)

![image](https://github.com/user-attachments/assets/7c13d84e-1281-4621-9dc0-fb5e5c17d0d6)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

