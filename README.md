# SERIAL-IN-SERIAL-OUT-SHIFTREGISTER

**AIM:**

To implement the  SISO Shift Register using Verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**SISO shift Register**

A Serial-In Serial-Out shift register is a sequential logic circuit that allows data to be shifted in and out one bit at a time in a serial manner. It consists of a cascade of flip-flops connected in series, forming a chain. The input data is applied to the first flip-flop in the chain, and as the clock pulses, the data propagates through the flip-flops, ultimately appearing at the output.

The logic circuit provided below demonstrates a serial-in serial-out (SISO) shift register. It comprises four D flip-flops that are interconnected in a sequential manner. These flip-flops operate synchronously with one another, as they all receive the same clock signal.

![image](https://github.com/naavaneetha/SERIAL-IN-SERIAL-OUT-SHIFTREGISTER/assets/154305477/e81c4072-37f9-46c6-8145-566764b74c3a)

Figure 01 4 Bit SISO Register

The synchronous nature of the flip-flops ensures that the shifting of data occurs in a coordinated manner. When the clock signal rises, the input data is sampled and stored in the first flip-flop. On subsequent clock pulses, the stored data propagates through the flip-flops, moving from one flip-flop to the next.
Each D flip-flop in the circuit has a Data (D) input, a Clock (CLK) input, and an output (Q). The D input represents the data to be loaded into the flip-flop, while the CLK input is connected to the common clock signal. The output (Q) of each flip-flop is connected to the D input of the next flip-flop, forming a cascade.

**Procedure**

1. Type the program in Quartus software.
2.	Compile and run the program.
3.	Generate the RTL schematic and save the logic diagram.
4.	Create nodes for inputs and outputs to generate the timing diagram.
5.	For different input combinations generate the timing diagram

	

![image](https://github.com/user-attachments/assets/896a210b-cf91-4224-909b-eb2c6b850803)





![image](https://github.com/user-attachments/assets/f5412d3b-21bd-4a83-873c-ea548e15fb93)



![image](https://github.com/user-attachments/assets/e2894edd-a8db-44cf-8369-202ef66cc503)




**PROGRAM**

'''module EXP10(clk, sin, q); 
input clk; input sin; 
output [3:0] q; 
reg [3:0] q; 
always @(posedge clk) begin q[0] <= sin; 
q[1] <= q[0]; 
q[2] <= q[1]; 
q[3] <= q[2]; 
end endmodule'''

**RTL LOGIC FOR SISO Shift Register**


![image](https://github.com/user-attachments/assets/699ef981-72c9-4af1-ab91-927a723b9a30)



**TIMING DIAGRAMS FOR SISO Shift Register**


![image](https://github.com/user-attachments/assets/6042c554-7eee-4fcb-b1a2-2c8b39ce421f)


**RESULT**
SISO Shift Register using Verilog and validating their functionality using their functional tables is verified.
