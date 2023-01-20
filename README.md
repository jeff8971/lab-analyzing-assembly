# Lab Analyzing Assembly

This lab seeks to help you understand File I/O in c, along with seeing the basic assembly that is generated for programs before it goes into a binary form.

👉🏽 **Your Task** will be to write a small C program, that reads an assembly file, and prints out the number of instructions in that file and estimated  cycle count to run the program. 

For example, assume  assembly.s has the following code:
```
MOVQ a, %rax
MOVQ b, %rbx
ADDQ %rbx, %rax
IMULQ %rbx
MOVQ %rax, c
```

Running your program `> estimator.out assembly.s` would print the following to the screen.

```
ADD 1
MOV 3
MUL 1

Total Instructions = 5
Total Cycles = 7
```
MUL, IMULQ are the same thing, along with MOVQ and MOV, etc. 

Let's get started! 

## Paired Programming
Make sure to partner up (or group up). One person should be coding, while the other person is directing. Make sure to ask each other questions, along with the TAs as you work. 

After you determine the 'driver', have them clone this repo to their own computer. 

## Generating Assembly Files (10 Minutes)

Both gcc and clang allow you to generate the assembly file for their code.  Looking at [simple.c], we see a program that
simply adds two numbers, and then ends. However, [simple.s] is the assembly built from this program. This was done using the following option.

> clang -S simple.c

👉🏽 **Your Task** Write a **simple** c program, and generate the assembly file.

To help you better understand, you should write a simple/small C program. After you have completed the program, run the compiler with the `-S` option, to see the assembly generated. 

### Discussion
* What are some of the assembly commands generated? 
* Was there more than you expected? 
* Can you find the functions you wrote easily?

## Writing Estimator





## 📚 Resources

* [strstr() tutorial](https://www.tutorialspoint.com/c_standard_library/c_function_strstr.htm)



[simple.c]: simple.c
[simple.s]: simple.s