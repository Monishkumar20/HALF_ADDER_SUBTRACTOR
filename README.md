![image](https://github.com/user-attachments/assets/b616ca0e-85e0-4938-baf8-b1c799a9f5a0)# HALF_ADDER_SUBTRACTOR

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

1.HALF SUBTRACTOR

![WhatsApp Image 2024-12-21 at 09 36 53_6fc84887](https://github.com/user-attachments/assets/949f894a-27b0-44cf-9958-4718c9ad0fde)

2.HALF ADDER

![WhatsApp Image 2024-12-21 at 09 37 48_51ee18a7](https://github.com/user-attachments/assets/a8224682-edea-44b9-a23d-c7f2e10c34ec)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

```
module ha(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum= (a ^ b);
assign carry= ( a & b);
endmodule


module hs(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign difference= (a ^ b);
assign borrow= ( ~a & b);
endmodule
```

**RTL Schematic**

1.HALF ADDER

![image](https://github.com/user-attachments/assets/354189a4-d973-4a3c-9834-bb8af143578b)

2.HALF SUBTRACTOR

![image](https://github.com/user-attachments/assets/c8971e1d-840a-4cda-b1eb-80761aca0e3c)



**Output/TIMING Waveform**
1.HALF ADDER

![image](https://github.com/user-attachments/assets/2e546267-5e02-437e-b0be-c3a08683ab5b)

2.HALF SUBTRACTOR

![image](https://github.com/user-attachments/assets/30b80242-00f5-40f9-9807-ba97d86c19b2)





**Result:**
The code is excecuted successfully.
