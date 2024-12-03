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

Developed by: S.Ravant Vignesh
RegisterNumber:24900151 */
i)
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

ii)
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule



**RTL realization**
![WhatsApp Image 2024-12-03 at 20 31 37_fa4fe34b](https://github.com/user-attachments/assets/3920f588-5f14-43c9-8b5d-3c9a05f187e9)
![WhatsApp Image 2024-12-03 at 20 31 37_8e296055](https://github.com/user-attachments/assets/ae0e577d-469c-4a5f-8670-e9f508f6b65b)


**Output:**

![WhatsApp Image 2024-12-03 at 20 31 38_7f653341](https://github.com/user-attachments/assets/f63b8923-fc5b-46b7-85f4-dd78d5228be8)
![WhatsApp Image 2024-12-03 at 20 31 38_60d604a6](https://github.com/user-attachments/assets/266c6a55-f0ef-4f6b-a41d-423567385c58)

**truth table**

![WhatsApp Image 2024-12-03 at 20 31 38_4c2cb37d](https://github.com/user-attachments/assets/fe14ad99-bea2-48d7-9475-5ab5336b7698)
![WhatsApp Image 2024-12-03 at 20 31 38_bfedabed](https://github.com/user-attachments/assets/b54a3449-52f6-4e76-a955-1872dac304e5)


**k map**

![WhatsApp Image 2024-12-03 at 20 31 39_3e52f71d](https://github.com/user-attachments/assets/c99adf14-68b2-4ed7-8c54-2175d14b802b)
![WhatsApp Image 2024-12-03 at 20 31 39_ceef6a94](https://github.com/user-attachments/assets/d0412058-dbac-458d-b85c-15f0b039bcdd)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

