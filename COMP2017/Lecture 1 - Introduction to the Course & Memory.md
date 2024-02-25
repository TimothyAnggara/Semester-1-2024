### Assessments
- In Class tasks
	- Weekly (Tutorials)
	- 10%
	- Needs at least 40% in at least 5 of the class tasks
	- How to get 100?
		- Get 100% in seven of the class tasks
- A1
	- 10 March
	- 5%
- A2
	- 28 March
	- 10%
- A3 Tests
	- 12 May
	- 5%
- A3
	- 19 May
	- 20%
- Final Exam
	- Formal Exam period
	- 50%

### Unix Commands
- `echo "string`
	- Prints a string into the terminal
	- `echo | cut -b 3-5`
		- Splits the string from the 3rd letter into the 5th letter and prints to terminal
- `<, >, |`
	- A pipe operator
		- Takes input from a file into a program
		- Save output from a program into a file
- `diff`
	- Checks the difference between two files
		- If nothing is returned then everything is okay
		- If someone is printed then something is different
- `echo $?`
	- Prints to the terminal the exit code
		- 0 = Okay
		- non-zero = not okay
#### Example:
- Lets say we want to test a program if it matches the expected output with the example input
	- `./myscript.sh < test1.in > actual_output.txt`
	- `diff test1.expected actual_output.txt`
		- In the line above, we are passing input into a script and saving it into a output file
		- Afterwards we check the output of the program with actual_output.txt
	- We can do this is one line by:
		- `./myscript.sh < test1.in | diff - test1.expected`

### Memory
- Foundation of everything in this course
![[Pasted image 20240224140940.png]]

- Memory is the storage of short-term data which is composed of addresses and values
	- Memory is stored in 1 bytes which contains 8 bits
		- 0000 0000
- Where and how do we store data into memory?
	- `int x = 7;`
	- With the C programming language, it first ask how big is an int?
		- On a 64 bit machine, 8 bytes large
		- C has fixed bit-width size
	- A computer has two types of memory
		- Physical memory - The memory we have on the computer
		- Virtual memory - Memory that does not physically exist
			- Has $2^{48}$ bytes
 ![[Pasted image 20240224193054.png]]
	- When we call `int x = 7;`
		- It first reside it in virtual memory 
		- When we want to use it, the computer copies it to physical memory and x is given to the CPU
	- There are 4 parts of the virtual memory
		![[Pasted image 20240224193813.png]]
- How does the computer how which code to execute?
	- It has its own miniature program run by the CPU
		- "Fetch, Decode, Execute"
			- It executes programs line by line
			- "Fetch" - Fetches the line in the program to be executed
			- "Decode" - Which circuits in the CPU is needed to run the program and which data is needed to be run the program
			- "Execute" - Executes the line
		- Computer viruses main idea is to manipulate this miniature program to execute something malicious
		- Always occuring and you can't stop
		- It loops all the time
#### Memory of a Computer : Addressing Systems
- Memory is all about addresses and values
	- Address = location in memory of the value
	- Values are an arbitrary number of the bits
		- This arbitrary number of bits has values because we made it to make it have value
		- First bit of a value is stored at the address
- Computers have two functions
	- Calculate
	- Copy memory
- Computers are constantly copying values from one address to another address
	- All calculations rely on memory being organised:
		- Correct values were copied into the area of memory
			- With the correct addresses
			- At the right time
### C-Language
- A compile time language
	- Unmanaged - No garbage collector
- Has text pre-processing language built-in
	- `#include <stdio.h>`
- Differences between Java to C
	- References are called "pointers" in C
	- No garbage collection
	- No classes or Objects
	- C is closer to underlying machine
	- C has simple memory model
	- No polymorphism or inheritance in C
- Running C Code
	- Create a program text in a file with the suffix ".c"
	- Compile the program using gcc
		- `gcc hello.c -o hello`
	- Run the program
		- `./hello`
- Arrays and memories
	- Arrays in C must have a defined size before the program gets executed
		- During the compilation phase
		- We forbid variable length arrays because of bad programming practice
```
int array[5];
array[0] = 5;
*(array) = 5; // Same as the line above

array[3] = 8;
*(array+3) = 8; // Same as the line above
```
- Functions in C
	- A function in C consist of:
		- Name of function
		- Return type of function
		- Parameter list and their types
	- To externally import functions, we use the `extern` keyword for use the `#include <filename.f>`
		- `extern int foo();`
	