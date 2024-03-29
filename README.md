# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**

### Full Adder

![image](https://github.com/saiganesh2006/FULL_ADDER_SUBTRACTOR/assets/145742342/32675021-f935-4a0b-b4d5-88a3d7dcbb1f)

### Full Subtractor

![image](https://github.com/saiganesh2006/FULL_ADDER_SUBTRACTOR/assets/145742342/dbbf663b-d739-4d77-a0b3-1feeb67812bf)

**Procedure**

1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram.
Write the detailed procedure here

**Program:**

 Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. 
### Developed by: D.B.V. SAI GANESH
### RegisterNumber: 212223240025
```
module Full_Adder_Subtractor(a,b,c,sum,carry,D,Bo);
input a,b,c;
output sum,carry,D,Bo;
assign sum=a^b^c;
assign carry=(a&b)|(b&c) | (a&c);
assign D=a^b^c;
assign B0=(~a&b) | (b&c) | (~a&c);
endmodule
```
**RTL Schematic**

![image](https://github.com/saiganesh2006/FULL_ADDER_SUBTRACTOR/assets/145742342/698fa788-653c-45dd-8120-1d6149e69d0f)

**Output Timing Waveform**

![image](https://github.com/saiganesh2006/FULL_ADDER_SUBTRACTOR/assets/145742342/543bcd05-4a21-4cda-b9e5-63ff5d976bb5)

**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



