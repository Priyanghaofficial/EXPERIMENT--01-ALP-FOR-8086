# EXPERIMENT--01-ALP-FOR-8086
Name :PRIYANGHA G
Roll no :212223040157
Date of experiment :3/3/2025





## Aim: To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 8086  emulator 
## Theory 
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.


 ## Running the Emulator :
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	  Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color 
 
 
3.	write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 

4.	 Compile the program and check for the errors 
5.	Run (once there is no syntax error) 

6.	Click OK to see/view the output of your program on the Emulator screen. 


7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,
8.	 


![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)











9.	Click on emulate to start emulation 








![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)








10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 






![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)







## Programs for arithmetic  operations

## Addition  of 8 bit ALP 
```
org 100h
MOV CL,00H
MOV AL,[4200H]
MOV BL,[4201H]
ADD AL,BL
JNC L
INC CL
L:MOV [4202H],AL
MOV [4203H],CL
ret
```


## Output  
 ![Screenshot (607)](https://github.com/user-attachments/assets/84acf087-4c4c-4b9e-acfd-b40c7c986898)

## Subtraction   of 8 bit numbers  ALP
```
org 100h
MOV AL,[4300H]
MOV BL,[4301H]
SUB AL,BL
MOV [4302H],AL
ret
```
## Output  
![Screenshot (609)](https://github.com/user-attachments/assets/3fd9bf1d-bc60-4e16-aed1-cfd9fa4950a6)

## Multiplication alp 
```
org 100h
MOV AL,[4400H]
MOV BL,[4401H]
MUL BL
MOV [4402H],AX
ret

```
 ## Output  
![Screenshot (610)](https://github.com/user-attachments/assets/3e2256e5-c0e6-4656-a677-dc582fe7059e)


## Division alp 
```
org 100h
MOV AL,[4300H]
MOV BL,[4301H]
DIV BL
MOV [4302H],AX
ret

```

## Output  
![Screenshot (611)](https://github.com/user-attachments/assets/1441d3b0-f455-4a55-98ed-18888be96dbe)

## logical :
```
org 100h
          
MOV AX, 0A32H
MOV BX, 0B31H
MOV SI, 5000H
OR AX, BX
MOV [SI], AX
MOV AX, 0A32H
AND AX, BX
MOV [SI+2], AX  
MOV AX,0A32H
XOR AX, BX
MOV [SI+4], AX
MOV AX, 0A32H
NOT AX
MOV [SI+6], AX
ret

```
## output
![Screenshot (615)](https://github.com/user-attachments/assets/c19cd214-3cc1-43f0-81cb-48b571277da2)

## Result :
The execution of ALP on fundamental arithmetic and logical operations is successfully completed.
 








