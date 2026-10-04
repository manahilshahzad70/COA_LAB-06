# COA_LAB-06

Computer Organization and Architecture Lab

# Computer Organization & Architecture Lab

## Lab 06 – Use of Venus Simulator for RISC-V Procedure Execution

### Lab Description

The purpose of this lab was to understand procedure execution, stack operations, and function calls in RISC-V assembly language. In this lab, different programs were implemented and executed using the Venus RISC-V Simulator to understand how procedures receive arguments, return results, preserve registers, and perform calculations.

The tasks implemented in this lab were:

1. Procedure Call and Return
2. Stack Operations and Register Values
3. Mathematical Expression Using a Procedure
4. Area and Perimeter of a Square
5. Polynomial Calculation
6. Conditional Procedure Calls
7. Conditional Function Execution
8. Fibonacci Series With and Without Recursion

### Task 1 – Procedure Call and Return

A RISC-V procedure was examined and corrected to ensure that the correct result was returned to the main program. The procedure calculates 3 + 1000 and returns 1003 in register `a0`. This value is added to 2500, producing the expected result of 3503 in register `t1`.

### Task 2 – Stack Operations and Register Values

Stack operations were implemented to store and retrieve register values using the `sw` and `lw` instructions. Space was allocated on the stack, values were stored at different offsets, and the stack pointer was restored after loading the values. The resulting register values were `t4 = 10`, `t2 = 15`, and `t3 = 5`.

### Task 3 – Mathematical Expression Using a Procedure

A procedure named `EqSolver` was implemented to calculate the expression `(a + b)(a - b)`. The values 5 and 3 were passed through argument registers, and the `add`, `sub`, and `mul` instructions were used to calculate the result. The final result returned by the procedure was 16.

### Task 4 – Area and Perimeter of a Square

Two procedures, `AreaFinder` and `PerimeterFinder`, were designed to calculate the area and perimeter of a square. The side length of 5 was passed to both procedures through register `a0`. The area was calculated by multiplying the side length by itself, while the perimeter was calculated by multiplying it by 4. The resulting area was 25 square units, and the perimeter was 20 units.

### Task 5 – Polynomial Calculation

A procedure named `EqSolver` was implemented to evaluate the polynomial `x^3 + 5x^2 + 6x`. The input value `x = 2` was passed through register `a0`, and multiplication and addition instructions were used to calculate the expression. The procedure returned the final result of 40.

### Task 6 – Conditional Procedure Calls

Conditional branching was used to select one of three procedures, `F1`, `F2`, and `F3`, based on the values of registers `s0` and `s1`. The `beq` and `blt` instructions determined which procedure to execute. For `s0 = 3` and `s1 = 2`, procedure `F2` was called to calculate the cube of 3, producing the result 27.

### Task 7 – Conditional Function Execution

Conditional branching was used to select one of three functions, `fun1`, `fun2`, and `fun3`. The program initialized both `s0` and `s1` to 4 and used the `beq` instruction to determine the appropriate function. Since the values were equal and nonzero, `fun2` was called to calculate the cube of 4, producing the result 64.

### Task 8 – Fibonacci Series With and Without Recursion

The Fibonacci sequence was implemented using both iterative and recursive approaches in RISC-V assembly. The iterative implementation used a loop to calculate successive Fibonacci numbers, while the recursive implementation called the procedure repeatedly and used the stack to preserve return addresses and intermediate values. For the input `n = 7`, both implementations produced the result 13.

### Software Used

- Venus RISC-V Simulator
- RISC-V Assembly Language

### Conclusion

This lab provided practical experience in writing and executing RISC-V assembly programs using the Venus Simulator. It helped demonstrate procedure calls, stack management, conditional execution, arithmetic calculations, and the implementation of iterative and recursive algorithms.
