# BOOLEAN_FUNCTION_MINIMIZATION

# AIM:

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

# Equipment Required:

Hardware – PCs, Cyclone II , USB flasher

# Software – Quartus prime:

# Theory:
Boolean function minimization is a fundamental concept in digital logic design aimed at reducing the complexity of logical expressions while maintaining their functionality. Here are a few theoretical perspectives on Boolean function minimization:

# Karnaugh Maps (K-Maps): #
Karnaugh Maps provide a graphical method for minimizing Boolean functions. They visually represent all possible combinations of input variables and their corresponding output values. By identifying adjacent groupings of 1s (or 0s) in the map, you can derive simplified expressions. This method is particularly useful for functions with a small number of variables, as it can become impractical for larger functions.

# Quine-McCluskey Algorithm: #
The Quine-McCluskey algorithm is a systematic approach to minimizing Boolean functions. It involves systematically combining minterms (or maxterms) to identify prime implicants, which are the smallest possible groupings that cover all essential terms. These prime implicants are then used to derive the minimized expression. While more computationally intensive compared to K-Maps, the Quine-McCluskey algorithm is efficient for functions with a larger number of variables.

# Implicant-Based Minimization: #
Boolean function minimization can also be approached by identifying essential prime implicants and eliminating redundant terms. Essential prime implicants are those that cover output states not covered by any other implicant. Redundant terms, on the other hand, can be eliminated if they are subsumed by other terms or combinations of terms. This approach is often used in combination with K-Maps or the Quine-McCluskey algorithm.

# Algebraic Manipulation: #
Boolean functions can also be minimized using algebraic manipulation techniques. These techniques involve applying Boolean algebra laws such as absorption, distribution, and complementation to simplify expressions. While algebraic manipulation can be intuitive for some functions, it may not always result in the most optimized expressions, especially for functions with many variables.

# Heuristic Methods: #
In addition to the systematic approaches mentioned above, heuristic methods can also be employed for Boolean function minimization. These methods often involve iterative algorithms that attempt to optimize expressions based on predefined criteria such as minimizing the number of terms or reducing the number of literals. Genetic algorithms, simulated annealing, and tabu search are examples of heuristic methods used in Boolean function minimization.

Overall, Boolean function minimization is a multifaceted topic with various methods and techniques available, each with its advantages and limitations. The choice of method depends on factors such as the complexity of the function, the number of variables involved, and the desired optimization criteria.

# Procedure:

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


# Program:
```
module exmp2(E ,F, A, B, C, D);
output E, F;
input A, B, C ,D;
assign E = A || (B && C) || ((!B) && D);
assign F = ((!B) && C) || (B && (!C) && (!D));
endmodule

```
# Developed by: Jabez S #
# Register Number: 212223040070 #

# RTL Realization:
![Screenshot 2024-03-18 085421](https://github.com/jabezs2005/BOOLEAN_FUNCTION_MINIMIZATION/assets/147473463/52220ad8-809a-413b-88c2-414d5b5944b5)

# Truth Table:
![Screenshot 2024-03-18 092347](https://github.com/jabezs2005/BOOLEAN_FUNCTION_MINIMIZATION/assets/147473463/cc4ab5dc-f37c-4105-b7ad-991131a7626d)

![Screenshot 2024-03-18 092407](https://github.com/jabezs2005/BOOLEAN_FUNCTION_MINIMIZATION/assets/147473463/6967d056-1d00-4dd2-b215-acbcd15d7f00)
# Timing: 
![Screenshot 2024-03-18 085246](https://github.com/jabezs2005/BOOLEAN_FUNCTION_MINIMIZATION/assets/147473463/ae12f02a-4cb5-4392-966a-e9819fe5c49d)

# Result:
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

