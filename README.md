### ENCODER 8TO3 DATAFLOW Modelling

**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/0bc242c1-eb9e-4c47-afe5-30428470efc3)

Figure 01  Block Diagram of Encoder 8 * 3

**Truth Table**

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/35496b14-ae6e-4cd1-9abd-d6736b576575)

The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/95acaee6-c873-4c75-89eb-ef09fb158053)

Figure 02  Encoder 8 * 3

**Procedure**
```
1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram.
```
**PROGRAM**

```
Developed by: SENTHIL KUMARAN C
RegisterNumber:212223220103

module encoder_4to2(A0, A1, YO, Y1, Y2, Y3);

input YO, Y1, Y2, Y3;

output A0, A1;

assign A1 = Y3 + Y2;

assign AO = Y3 + ((~Y2)&Y1);

endmodule
```

**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**
![image](https://github.com/gowthamsec/ENCODER8TO3DATAFLOW/assets/147933945/ff7309a6-b4f1-4985-9fa0-4d612a1c2153)



**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**
![image](https://github.com/gowthamsec/ENCODER8TO3DATAFLOW/assets/147933945/38ff12ec-d593-44d1-8a4b-ef1edc8d6549)



**RESULTS**
Implementing Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables executed succesfully.




