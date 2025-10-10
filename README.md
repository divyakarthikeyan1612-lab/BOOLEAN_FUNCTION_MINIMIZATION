# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
Boolean function minimization is the process of simplifying Boolean algebraic
 expressions to reduce the number of logic gates and complexity in a digital circuit,
 leading to more efficient, faster, and less costly hardware
 For minimizing Boolean expressions,we can use a set of rules and laws (like distributive,
 associative, and complement laws) to simplify Boolean expressions. This method
 focuses on applying algebraic manipulations to reduce the complexity of the expression
 by eliminating redundant terms.
 Identity Law A ⋅ 1 = A, A + 0 = A
 Null Law A ⋅ 0 = 0, A + 1 = 1
 Idempotent Law A ⋅ A = A, A + A = A
 Complement Law A ⋅ A′ = 0, A + A' = 1
 Distributive Law A ⋅ (B + C) = A ⋅ B + A ⋅ C
 De Morgan’s Law (A ⋅ B)′ = A′ + B', (A + B)′ = A′ ⋅ B′
 Absorption Law A ⋅ (A + B) = A, A + (A ⋅ B) = A
 Associative Law A + (B + C) = (A + B) + C, A.(B.C) = (A.B).C
 Commutative law A B = B A,A + B = B + A
 
**Logic Diagram**

IDENTITY LAW
<img width="713" height="370" alt="image" src="https://github.com/user-attachments/assets/a008ee2b-c898-4bb5-a07e-9f09d62e93fa" />

IDEMPOTENT LAW
<img width="264" height="169" alt="image" src="https://github.com/user-attachments/assets/e784aa4f-3f61-460e-985e-3ec2528075dd" />

COMPLEMENT LAW
<img width="281" height="157" alt="image" src="https://github.com/user-attachments/assets/5adefa2b-caf6-408d-b6a1-4f9c7e719ea6" />

DISTRIBUTIVE LAW
<img width="609" height="176" alt="image" src="https://github.com/user-attachments/assets/a749fd80-3373-489a-9ccf-9532e1376be5" />

DEMORGAN'S LAW
<img width="588" height="601" alt="image" src="https://github.com/user-attachments/assets/41bad2dc-e9af-4155-8aca-4b5ecdc5271b" />

ABSORPTION LAW
<img width="444" height="152" alt="image" src="https://github.com/user-attachments/assets/795658f3-9467-4201-9967-5dc131db3ade" />

ASSOCIATIVE LAW
<img width="300" height="324" alt="image" src="https://github.com/user-attachments/assets/6551a5e1-d28a-4e3e-8b55-52de8c82029f" />

COMMUTATIVE LAW
<img width="273" height="306" alt="image" src="https://github.com/user-attachments/assets/5f93fec9-9bf6-4fee-ab6f-a25c27203e05" />

NULL LAW
<img width="620" height="311" alt="image" src="https://github.com/user-attachments/assets/100ee87e-488d-4bfd-a207-48536617be32" />



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
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
assign f2=((~y & z)|( w & y )|(x & y));
endmodule


**RTL realization**

**Output:**
output 1 

<img width="1646" height="881" alt="image" src="https://github.com/user-attachments/assets/d6d72432-044d-4515-9340-f79c26683f15" />

output2 

<img width="1076" height="573" alt="image" src="https://github.com/user-attachments/assets/4196bfd2-7931-48bb-93b9-99708d9db03e" />



**RTL**

**Timing Diagram**
i)
<img width="1075" height="548" alt="image" src="https://github.com/user-attachments/assets/934014a2-67f1-46ac-b226-e690373f4cda" />

ii) 
<img width="1075" height="547" alt="image" src="https://github.com/user-attachments/assets/34c80de3-1883-4564-bd0a-3235e8a73dd5" />



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

