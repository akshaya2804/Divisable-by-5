Overview

This project implements two separate functionalities in SystemVerilog:

Pattern Generator: Generates a sequence of numbers in steps of 10, starting from 9, stopping at 59.

Divisible-by-5 Generator: Randomly generates numbers between 0 and 100 that are divisible by 5.

Part 1: Pattern Generator

Key Components

Class Definition

The pattern_generator class encapsulates the functionality for generating the sequence.

It contains:

value: An integer variable initialized to 9.

new function: A constructor to initialize the value variable.

generate_next task: Generates the next number in the sequence and prints it. If the sequence exceeds 59, it displays "End of sequence."

Testbench

The testbench (tb_pattern_generator) creates an object of the pattern_generator class and generates the sequence by calling the generate_next task in a loop using the repeat construct.

It Works


Initialization

The pattern_generator class initializes the starting value to 9 using the constructor (new).

Generate Sequence

The generate_next task checks if the current value is less than or equal to 59.

If true, the value is printed, and 10 is added to it.

If the value exceeds 59, the task displays "End of sequence."

Testbench Execution

The testbench creates an instance of the pattern_generator class.

It uses a repeat loop to call the generate_next task six times.

Output

The output of the program is:

 9 19 29 39 49 59
