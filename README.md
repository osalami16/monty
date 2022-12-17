Monty Interpreter
A language interpreter made in the C programming language to manage stacks and queues (LIFO and FIFO). The aim is to interpret Monty byte codes files. Monty is a language that aims to close the gap between scripting and programming languages.
Requirements
•	Allowed editors: vi, vim, emacs
•	All your files will be compiled on Ubuntu 20.04 LTS using gcc, using the options -Wall -Werror -Wextra -pedantic -std=c90
•	All your files should end with a new line
•	A README.md file, at the root of the folder of the project is mandatory
•	Your code should use the Betty style. It will be checked using betty-style.pl and betty-doc.pl
•	You allowed to use a maximum of one global variable
•	No more than 5 functions per file
•	You are allowed to use the C standard library
•	The prototypes of all your functions should be included in your header file called monty.h
•	Don’t forget to push your header file
•	All your header files should be include guarded
•	You are expected to do the tasks in the order shown in the project
Compilation
To compile this project, you can use the following command:
$ make
Allowable opcodes and what they do
Opcode	functionality
Push	add element to the 'top' of stack and 'end' of queue
Pop	remove element from 'top' of stack and 'end' of queue
Pall	print every member of the structure
Pint	prints the member value at the top of stack
Swap	swaps the order of the 1st and 2nd elements in stack
Add	add top two member values
Sub	subtract the top element from the 2nd top element
Div	divide the 2nd element by the top element
Mul	multiply the top two elements of the stack
Mod	the remainder when the 2nd element is divided by the top element
Comment	there is the ability to parse comments found in byte code ->'#'
Pchar	print character at the top of the stack
Pstr	print the character at the top of the stack
Rotl	moves element at the top to the bottom of the stack
Rotr	the bottom of the stack becomes the top
queue, stack	toggles the doubly link list implementation style
Nop	opcode should do nothing
Examples: $ cat opcodetestfile.m
push 1
push 2
push 3
pall
$. /Monty file opcodetestfile.m
3
2
1
$

$ cat opcodetestfile.m
push 1
push 2
push 3
pall
rotl
pall
$ ./Monty file opcodetestfile.m
3
2
1
2
1
3
Exit Status
Exits with status EXIT_FAILURE
Compilation
All files were compiled on Ubuntu 14.04 LTS.
All programs and functions were compiled with gcc 4.8.4 using flags -Wall -Werror -Wextra and -pedantic.
Styling
All files have been written in the Betty Style.
Author    Omolola Taiwo


