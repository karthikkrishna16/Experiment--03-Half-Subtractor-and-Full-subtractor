# Experiment--03-Half-Subtractor-and-Full-subtractor
## Implementation-of-Half-subtractor-and-Full-subtractor-circuit
## AIM:
To design a half subtractor and full subtractor circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime
## Theory
Subtractor circuits take two binary numbers as input and subtract one binary number input from the other binary number input. Similar to adders, it gives out two outputs, difference and borrow (carry-in the case of Adder). There are two types of subtractors.

## Half Subtractor Full Subtractor
## Half Subtractor
The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed.
![half-subtractor9](https://user-images.githubusercontent.com/36288975/166112538-58c3bc7c-ee5d-4e6a-ac8d-8e8328efe27a.png)


Sum = X'Y+XY' = X ⊕ Y
Carry=X'Y

## Full Subtractor
A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow. 
![full-subtractor6](https://user-images.githubusercontent.com/36288975/166112541-24c68359-3de8-4674-ae22-8272ffc385ed.png)


Diff = A ⊕ B ⊕ Bin B = A'Bin + A'B + BBin

## Procedure

STEP 1: Use module project name(input,output) to start the Verilog
programmming.
STEP 2: Assign inputs and outputs using the word input and output
respectively.
STEP 3: Use defined keywords like wire,assign and required logic gates to
represent the boolean
expression.
STEP 4: Use each output to represnt onre for differnce and the other for
borrow.
STEP 5: End the verilog program using keyword endmodule.

## Program:
/*
Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
Developed by: T H KARTHIK KRISHNA
RegisterNumber: 23014165 
*/

### code:

half subtractor:

![image](https://github.com/karthikkrishna16/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/148514663/73cc36a9-69cf-4f48-ad1f-f9b386b303c8)

full subtractor:

![image](https://github.com/karthikkrishna16/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/148514663/fa70566a-1009-497c-abe2-643335e5140f)


### Output:

Truthtable:

half subtractor:

![image](https://github.com/karthikkrishna16/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/148514663/d2fe2f29-d6b1-4aae-a90d-def123967a6f)

full subtractor:

![image](https://github.com/karthikkrishna16/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/148514663/aec11f04-35ff-48f9-9d0a-e741d43d52b0)

###  RTL realization:

half subtractor:

![image](https://github.com/karthikkrishna16/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/148514663/ee90a913-f3b4-4a4d-9172-79899923ec26)

full subtractor:

![image](https://github.com/karthikkrishna16/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/148514663/bba610a2-8c9b-4f1e-85ff-527726a67816)

### Timing diagram:

half adder:

![image](https://github.com/karthikkrishna16/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/148514663/a2a5d580-8baf-472e-9e10-03211cf05090)

full adder:

![image](https://github.com/karthikkrishna16/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/148514663/0afd15e2-ae18-455b-ba78-016530d34fec)

### Result:
Thus the half subtractor and full subtractor circuits are designed and the truth tables is verified using quartus software.
