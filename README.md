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
STEP 1: Use module project name(input,output) to start the Verilog programmming.

STEP 2: Assign inputs and outputs using the word input and output respectively.

STEP 3: Use defined keywords like wire,assign and required logic gates to represent the boolean
expression.

STEP 4: Use each output to represnt onre for differnce and the other for borrow.

STEP 5: End the verilog program using keyword endmodule.



Write the detailed procedure here 


## Program:
/*
Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.

Developed by: R.Monish

RegisterNumber:  212223220061

*/

CODE:

HALF SUBTRACTOR:

![Exp4 hs code](https://github.com/monishr288/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/147474049/39d203b6-45e4-497f-95ee-5950573b5cb1)


FULL SUBTRACTOR:

![Exp4 fs code](https://github.com/monishr288/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/147474049/b43e2f35-f5c8-45e1-97dd-94e6f4bd8de4)


## Output:

## Truthtable

HALF SUBTRACTOR:

![Exp4 truthtable hs](https://github.com/monishr288/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/147474049/e1c68c2c-b504-444a-9bc4-601998cbc6b6)

FULL SUBTRACTOR:

![Exp4 truthtable fs](https://github.com/monishr288/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/147474049/3728edb8-a7ee-4183-83cf-608d0df65113)


##  RTL realization
HALF SUBTRACTOR:

![Exp4 hs RTL diagram](https://github.com/monishr288/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/147474049/b947065f-b608-4c85-a843-92ab6a0cd1ab)

FULL SUBTRACTOR:

![Exp4 fs RTL diagram](https://github.com/monishr288/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/147474049/8399a829-61c0-4789-9b66-05d6972fed63)



## Timing diagram 
HALF SUBTRACTOR:

![hs wave](https://github.com/monishr288/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/147474049/669315aa-15eb-4d90-ae40-2a4447137b1c)

FULL SUBTRACTOR:

![fs wave](https://github.com/monishr288/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/147474049/658d39db-0b5b-43e2-8d51-cd6f714cd404)


## Result:

Thus the half subtractor and full subtractor circuits are designed and the truth tables is verified using quartus software.
