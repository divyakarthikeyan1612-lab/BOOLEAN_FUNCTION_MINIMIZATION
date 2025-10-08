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

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

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
<img width="1646" height="881" alt="image" src="https://github.com/user-attachments/assets/4b53a64e-d54e-476c-97d4-b00bfb277266" />

**RTL**

**Timing Diagram**
<img width="1920" height="978" alt="Screenshot (65)2" src="https://github.com/user-attachments/assets/ea0facda-c0d2-4216-81ed-7bef85e86509" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

