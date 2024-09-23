

# EXPERIMENT 01- ARITHMETIC OPERATION AND LOGICAL OPERATION IN 8086
```
Name : Vignesh R
Roll no : 212223240177
Date : 12/08/2024
```


## Aim: 
  To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 8086  emulator 
## Theory 
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.


 ## Running the Emulator :
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	  Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color 
 
 
3.		write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 

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

## Addition  
```python
org 100h
mov al,024h;
mov bl,al;
add bl,al;
mov [0123h],bl;
ret
```

## Output  
 ![image](https://github.com/Jayakrishnan22003251/EXPERIMENT--01-ALP-FOR-8086/assets/120232371/ce0a7579-1e04-4f7e-8427-af7e0467ae2b)

## Subtraction 
```python
org 100h
mov al,024h;
mov bl,[0123h+02];
sub bl,al;
mov [0123h+04],bl;
ret
```
## Output
![image](https://github.com/Jayakrishnan22003251/EXPERIMENT--01-ALP-FOR-8086/assets/120232371/c8cc0918-d169-4573-bd2c-acd61e534281)

## Multiplication
```python
org 100h
mov bx,0015h;
mov al,[bx];
mul bl;
mov [0015h+04],al;
ret
```
 ## Output  
![image](https://github.com/Jayakrishnan22003251/EXPERIMENT--01-ALP-FOR-8086/assets/120232371/cb7911a3-753b-444b-ad1d-50114c64ca97)


## Division
```python
org 100h
mov bx,0040h;
mov al,[bx+02];
div bl;
mov [0040h+04],al;
ret
```
## Output  
![image](https://github.com/Jayakrishnan22003251/EXPERIMENT--01-ALP-FOR-8086/assets/120232371/8e1b0784-89f4-4e15-aada-85f2871a5ea2)

## Programs for logical  operations

## AND
```python
org 100h
mov bx,1000h;
and bx,1111h;
mov [0040h+02],bx;
ret
```
## Output 
![image](https://github.com/Jayakrishnan22003251/EXPERIMENT--01-ALP-FOR-8086/assets/120232371/380eb8b2-be95-414c-9eef-e7455ac8083a)

## OR
```python
org 100h
mov ax,[0040h+06];
mov bx,1000h;
or ax,bx;
mov [0040h+02],ax;
ret
```
## Output
![image](https://github.com/Jayakrishnan22003251/EXPERIMENT--01-ALP-FOR-8086/assets/120232371/372bd3ba-09b4-47c0-8cd3-2a6c5e9447b0)

## NOT
```python
org 100h
mov bx,0040h;
mov ax,[bx]; 
not al;
mov [0040h+04],ax;
ret
```
## Output
![image](https://github.com/Jayakrishnan22003251/EXPERIMENT--01-ALP-FOR-8086/assets/120232371/57ff6c88-2341-4eb3-bbfc-b1f9cb8fe8cc)

## XOR
```python
org 100h
mov bx,0040h;
mov ax,[bx]; 
xor ax,bx;
mov [0040h+04],ax;
ret
```
## Output
![image](https://github.com/Jayakrishnan22003251/EXPERIMENT--01-ALP-FOR-8086/assets/120232371/4ef2fb5c-0e99-4427-93b6-7cafa2ae77ff)

## Result :
Thus, ALP for fundamental arithmetic and logical operations are executed successfully.








