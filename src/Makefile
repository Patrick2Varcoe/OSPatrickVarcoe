all: task1.1 task1.2 task2.1 task2.2 task2.3

task1.1:  assemblyio.asm asm_io.asm asm_io.inc driver.c
	nasm -f elf asm_io.asm -o asm_io.o
	gcc -m32 -c driver.c -o driver.o
	nasm -f elf assemblyio.asm -o assemblyio.o
	gcc -m32 driver.o assemblyio.o asm_io.o -o task1.1.exe
task1.2:  task1.2.asm asm_io.asm asm_io.inc driver.c
	nasm -f elf task1.2.asm -o task1.2.o
	nasm -f elf asm_io.asm -o asm_io.o
	gcc -m32 -c driver.c -o driver.o
	gcc -m32 driver.o task1.2.o asm_io.o -o task1.2.exe
task2.1:  task2.asm asm_io.asm asm_io.inc driver.c
	nasm -f elf asm_io.asm -o asm_io.o
	gcc -m32 -c driver.c -o driver.o
	nasm -f elf task2.asm -o task2.1.o
	gcc -m32 driver.o task2.1.o asm_io.o -o task2.1.exe
task2.2:  task2.2.asm asm_io.asm asm_io.inc driver.c
	nasm -f elf asm_io.asm -o asm_io.o
	gcc -m32 -c driver.c -o driver.o
	nasm -f elf task2.2.asm -o task2.2.o
	gcc -m32 driver.o task2.2.o asm_io.o -o task2.2.exe
task2.3:  task2.3.asm asm_io.asm asm_io.inc driver.c
	nasm -f elf asm_io.asm -o asm_io.o
	gcc -m32 -c driver.c -o driver.o
	nasm -f elf task2.3.asm -o task2.3.o
	gcc -m32 driver.o task2.3.o asm_io.o -o task2.3.exe


