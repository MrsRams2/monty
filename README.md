0x19. C - Stacks, Queues - LIFO, FIFO

All your files will be compiled on Ubuntu 20.04 LTS using gcc, using the options -Wall -Werror -Wextra -pedantic -std=c89
A README.md file, at the root of the folder of the project is mandatory
Your code should use the Betty style. It will be checked using betty-style.pl and betty-doc.pl


Compilation & Output
Your code will be compiled this way:
$ gcc -Wall -Werror -Wextra -pedantic -std=c89 *.c -o monty

The Monty language
Monty 0.98 is a scripting language that is first compiled into Monty byte codes (Just like Python). 
It relies on a unique stack, with specific instructions to manipulate it. 
The goal of this project is to create an interpreter for Monty ByteCodes files.

The monty program

Usage: monty file
where file is the path to the file containing Monty byte code
If the user does not give any file or more than one argument to your program, print the error message USAGE: monty file, followed by a new line, and exit with the status EXIT_FAILURE
If, for any reason, it’s not possible to open the file, print the error message Error: Can't open file <file>, followed by a new line, and exit with the status EXIT_FAILURE
where <file> is the name of the file
If the file contains an invalid instruction, print the error message L<line_number>: unknown instruction <opcode>, followed by a new line, and exit with the status EXIT_FAILURE
where is the line number where the instruction appears.
Line numbers always start at 1
The monty program runs the bytecodes line by line and stop if either:
it executed properly every line of the file
it finds an error in the file
an error occured
If you can’t malloc anymore, print the error message Error: malloc failed, followed by a new line, and exit with status EXIT_FAILURE.
You have to use malloc and free and are not allowed to use any other function from man malloc (realloc, calloc, …)


0. push, pall
Implement the push and pall opcodes.

The push opcode

The opcode push pushes an element to the stack.

Usage: push <int>
where <int> is an integer
if <int> is not an integer or if there is no argument given to push, print the error message L<line_number>: usage: push integer, followed by a new line, and exit with the status EXIT_FAILURE
where is the line number in the file

2. pop
Implement the pop opcode.
The pop opcode
The opcode pop removes the top element of the stack.


3. swap
Implement the swap opcode
The swap opcode
The opcode swap swaps the top two elements of the stack.


4. add
Implement the add opcode.
The add opcode
The opcode add adds the top two elements of the stack.


5. nop
Implement the nop opcode.
The nop opcode
The opcode nop doesn’t do anything.

6. sub
Implement the sub opcode.
The sub opcode
The opcode sub subtracts the top element of the stack from the second top element of the stack.

7. div
Implement the div opcode.
The div opcode
The opcode div divides the second top element of the stack by the top element of the stack.

8. mul
Implement the mul opcode.
The mul opcode
The opcode mul multiplies the second top element of the stack with the top element of the stack

9. mod
Implement the mod opcode.
The mod opcode
The opcode mod computes the rest of the division of the second top element of the stack by the top element of the stack.

10. comments
Every good language comes with the capability of commenting. When the first non-space character of a line is #, 
treat this line as a comment (don’t do anything).

11. pchar
Implement the pchar opcode.
The pchar opcode
The opcode pchar prints the char at the top of the stack, followed by a new line.

12. pstr
Implement the pstr opcode.
The pstr opcode
The opcode pstr prints the string starting at the top of the stack, followed by a new line.

13. rotl
Implement the rotl opcode.
The rotl opcode
The opcode rotl rotates the stack to the top

14. rotr
Implement the rotr opcode.
The rotr opcode
The opcode rotr rotates the stack to the bottom.

15. stack, queue
Implement the stack and queue opcodes.
The stack opcode
The opcode stack sets the format of the data to a stack (LIFO). This is the default behavior of the program.

16. Brainf*ck
Write a Brainf*ck script that prints School, followed by a new line.
All your Brainf*ck files should be stored inside the bf sub directory
You can install the bf interpreter to test your code: sudo apt-get install bf
Read: Brainf*ck

17. Add two digits
Add two digits given by the user.
Read the two digits from stdin, add them, and print the result
The total of the two digits with be one digit-long (<10)


18. Multiplication
Multiply two digits given by the user.
Read the two digits from stdin, multiply them, and print the result
The result of the multiplication will be one digit-long (<10)


19. Multiplication level up
Multiply two digits given by the user.

