# 4-BIT-RIPPLE-COUNTER

Developed by:P.Dharshini

Register number:25010127


**AIM:**

To implement  4 Bit Ripple Counter using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 Bit Ripple Counter**

A binary ripple counter consists of a series connection of complementing flip-flops (T or JK type), with the output of each flip-flop connected to the Clock Pulse input of the next higher-order flip-flop. The flip-flop holding the least significant bit receives the incoming count pulses. The diagram of a 4-bit binary ripple counter is shown in Fig. below.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/cb4b74d4-31ab-4359-95d0-d22e67daba13)

In timing diagram Q0 is changing as soon as the negative edge of clock pulse is encountered, Q1 is changing when negative edge of Q0 is encountered(because Q0 is like clock pulse for second flip flop) and so on.

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/a573a7d6-014e-4e54-93e6-e2ac9530960b)

![image](https://github.com/naavaneetha/4-BIT-RIPPLE-COUNTER/assets/154305477/85e1958a-2fc1-49bb-9a9f-d58ccbf3663c)

**Procedure**

1.Start the simulation tool (such as ModelSim).

2.Create a new project and add a new Verilog source file.

3.Write the Verilog code for the 4-bit ripple counter module.

4.The counter consists of 4 flip-flops, where:

5.The first flip-flop receives the clock input.

6.The output of each flip-flop acts as the clock for the next flip-flop.

7.Add a reset signal (rst) to initialize the counter output to 0000.

8.Create a testbench module to generate the clock and reset signals.

9.Compile the design and check for errors.

10.Run the simulation.

**PROGRAM**

/* Program for 4 Bit Ripple Counter and verify its truth table in quartus using Verilog programming.

 Developed by:P.DHARSHINI
 
 RegisterNumber:25010127
*/
```
module exp_6(out,clk,rst); 
 input clk,rst; 
 output reg [3:0]out; 
 always @ (posedge clk)
 begin 
 if(rst) 
 out<=0; 
 else 
 out <= out-1; 
 end endmodule
```

**RTL LOGIC FOR 4 Bit Ripple Counter**
<img width="1920" height="1080" alt="Screenshot (590)" src="https://github.com/user-attachments/assets/b12a48ae-353c-47f6-806b-9250faf4550e" />


**TIMING DIGRAMS FOR 4 Bit Ripple Counter**
<img width="1920" height="1080" alt="Screenshot (591)" src="https://github.com/user-attachments/assets/f5164d1a-acf6-4c46-ab64-b2b6c1608d22" />


**RESULTS**
Thus,4-bit ripples counter executed successfully.
