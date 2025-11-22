# BOOLEAN_FUNCTION_MINIMIZATION
```
Developed by: S.VISANIYA

RegisterNumber: 25017540
```

*AIM:*

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

*Equipment Required:*

Hardware – PCs, Cyclone II , USB flasher

*Software – Quartus prime*

*Theory*

*Logic Diagram*

*Procedure*

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


*Program:*

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 


```
module logic_function(
    input  a, b, c, d,
    input  w, x, y, z,
    output f1, f2
);

assign f1 = (~b & ~d) |
            (a & b & ~c) |
            (~a & b & d);

assign f2 = (~y & z) |
            (w & y);

endmodule

```


## Logic symbol & Truthtable:

![TABLE 1](https://github.com/user-attachments/assets/29e25056-2bb7-4318-9fb0-bc5f8971fa73)

![TABLE 2](https://github.com/user-attachments/assets/2910d619-1b34-4093-a662-a57eb765df98)


*RTL realization*

<img width="1226" height="768" alt="Screenshot 2025-11-22 103401" src="https://github.com/user-attachments/assets/10147c62-b980-4d80-b792-7fe0e863f024" />



*Output:*
<img width="1920" height="1080" alt="Screenshot (47)" src="https://github.com/user-attachments/assets/a7345987-5e08-4363-865a-ed793e813ae8" />

*Result:*

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
