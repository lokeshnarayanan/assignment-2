# assignment-2
assignment

## Minimise the function using K map F(A,B,C)A'B'+BC'+BC+A'B'C' and simulate the logic diagram using verilog

## AIM:

TO design F(A,B,C)A'B'+BC'+BC+A'B'C' and simulate the logic diagram using verilog

## HARDWARE REQUIRED:

PC Cyclone || USB flasher

## SOFTWARE REQUIRED:

Quartus prime model sim

## THEORY

## INTRODUCTION:
 K map is a graphical method for simplifying Boolean expression it is used to minimise the boolean function by taking advantage of the properties of logic.
 
 to minimise the given boolean function using k-map table with the minterm of the function the minterm are trhe product of the variable and their complements that is the minterm of the function F(A,B,C)A'B'+BC'+BC+A'B'C' .
 
 Then we group together adjacent terms that have exactly one variable different between them. These groups of terms are called "groups of 1's" or "adjacent cells"

Finally, we can use the properties of Boolean algebra to simplify the expression using the following steps:

Combine the groups of 1's that have a 1 in the same cell.
Replace the Boolean variables in the expression with their complements, if it results in a smaller expression.
Use the standard Boolean identities to simplify the expression further.
After applying these steps, the simplified Boolean function will be the most reduced form possible.
The final minimized function will be F(A,B,C) = A′B'+BC′+BC+A'B′C′ = A′B' + (B + C)C' = A′B' + C'(B + C) = A′B'+C'

It is important to note that there are different methods to simplify Boolean functions and K-map is one of the most common methods.

## LOGICAL EXPRESSION:

F(A,B,C)=A'B'+BC'+BC+A'B'C'is 

F(A,B,C)=(A'*B')+(B*C')+(B*C)+(A'*B'*C') where '*' denotes logical AND operation and '+'denotes logical OR.
it is also possible to represent this function in the sum of product (sop)form :
F(A,B,C)=A'B'+BC'+BC+A'B'C' or in the product of sum (pos) form:F(A+B+C')(A+B+C)(A'+B'+C) BOTH forms are mathematicallyt equivalent but the sop form is more suited for implementation using AND - OR GATES

 ## Procedure:

1.start the module using module program().

2.Declare the inputs and outputs.

3.Use wire to assign intermediate outputs.

4.Use and gates to get the desired output.

5.End the module.

6.Generate RTL realization and timing diagrams.

PROGRAM:

Program to verify the truth table in quartus for the basic logic gates using Verilog programming.
Developed by: LOKESH N
RegisterNumber: 22008481

module logicdiagram(A,B,C,F);

input A,B,C;

output F;

assign F = (!A & !B) | (B & !C) | (B & C) | (!A & !B & !C);

endmodule

## OUTPUT:

## RTL Diagram
![image](https://user-images.githubusercontent.com/119393019/214244627-25b9dfe3-3515-4745-84a5-fbd197869778.png)

## RTL Timing Diagram:
![image](https://user-images.githubusercontent.com/119393019/214244443-2921b378-6547-4b59-a8d8-7c0c33ea4b1f.png)

## TRUTH TABLE:

![image](https://user-images.githubusercontent.com/119393019/214246703-d39c8b12-6b85-4cd8-80fe-1abf28284d03.png)

## RESULT

Hence  F(A,B,C)A'B'+BC'+BC+A'B'C' has been implemented and verified using verilog code programming and its output are validated
