# TITTLE

Design a 4 bit binary to BCD converter using verilog.


# THEORY

BCD code plays an important role in digital circuits. The BCD stands for Binary Coded Decimal Number. In BCD code, each digit of the decimal number is represented as its equivalent binary number. So, the LSB and MSB of the decimal numbers are represented as its binary numbers.ln the 4 bit binary to BCD code converter, the input is 4- bit binary so there is 16 possible combinations. From 10 to 15 decimal numbers, since we cannot represent these numbers by 4 bit BCD code, so we need 8 bit to represent such 2 digit decimal number.But the first 3 bits are zero. Therefore, we can ignore the first 3 bit and we are going to use remaining 5 bits to represent such number in BCD code.

# PROGRAM

```
Program to design a half adder and full adder circuit and verify its truth table in quartus

using Verilog programming.

Developed by: ALFRED AB

registerNumber: 212222110002


module bcd(input [3:0] bin_in, output reg [3:0] bcd_out);

always @* begin

case (bin_in) 4'be000: bcd_out = 4'b0000;

4'b0001: bcd_out = 4'b0001;

4'be010: bcd_out = 4'b9910;

4'b0011: bcd_out = 4'b0011;

4'b0100: bcd_out = 4'b0100;

4'b0101: bcd_out = 4'b0101;

4'b0110bcd_out = 4'b0110;

4'b0111: bcd_out = 4'b0111;

4'b1000: bcd_out = 4'b1000;

4'b1001: bcd_out = 4'b1001;

default: bcd_out = 4'bxxxx;


endmodule
```

# LOGIC DIAGRAM

![image](https://github.com/Alfredsec/Simulation-project--Digital-Electronics/assets/120621608/5a7efd50-27a8-4801-84ed-464b348e006f)


# TRUTH TABLE:

![image](https://github.com/Alfredsec/Simulation-project--Digital-Electronics/assets/120621608/91343bc2-a142-49e3-b5ba-b49bd9991f82)


# TIMING DIAGRAM

![image](https://github.com/Alfredsec/Simulation-project--Digital-Electronics/assets/120621608/70e9f247-0c12-4f25-9b34-d71590b25c7d)


# RESULT

Thus,to design a 4 bit binary to BCD converter is implemented successfully in Quartus using Verilog programming.


