# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**
![Half Adder](https://github.com/user-attachments/assets/4b27b166-b1a6-43be-9efd-4b10cf21e8ad)


![Half subtracter](https://github.com/user-attachments/assets/d403ac9e-42fd-4749-bb3d-752691648a76)




**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

i)HALF ADDER
module ha(a,b,sum,carry);


input a,b;


output sum,carry;


assign sum= (a ^ b);


assign carry= ( a & b);


endmodule





ii)HALF SUBTRACTOR
module hs(a,b,difference,borrow);


input a,b;


output difference,borrow;


assign difference= (a ^ b);


assign borrow= ( ~a & b);


endmodule

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by:YUGESH M
RegisterNumber:24900164*/

**RTL Schematic**


i)HALF ADDER
![logi diagram](https://github.com/user-attachments/assets/265aaf7f-880c-4373-8576-1e373b55d21e)


ii)HALF SUBTRACTOR
![logic diagram](https://github.com/user-attachments/assets/fbd43f4c-8dbc-4e28-b077-a45c545d13ef)



**Output/TIMING Waveform**

i)HALF ADDER
![output](https://github.com/user-attachments/assets/2e42b844-3a64-4298-ae99-2f9d0c927c58)

ii)HALF SUBTRACTOR
![output 2](https://github.com/user-attachments/assets/9f852368-2489-4c2c-8127-84e755ee3f4d)



**Result:**
Thus the Half adder and half subtractor are verified by using verilog programm.
