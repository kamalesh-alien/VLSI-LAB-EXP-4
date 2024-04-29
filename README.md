
SIMULATION AND IMPLEMENTATION OF SEQUENTIAL LOGIC CIRCUITS

AIM: To simulate and synthesis SR, JK, T, D - FLIPFLOP, COUNTER DESIGN using Vivado 2023.1.

APPARATUS REQUIRED: Vivado 2023.1

Procedure:

Open Vivado: Launch Xilinx Vivado software on your computer.

Create a New Project: Click on "Create Project" from the welcome page or navigate through "File" > "Project" > "New".

Project Settings: Follow the prompts to set up your project. Specify the project name, location, and select RTL project type.

Add Design Files: Add your Verilog design files to the project. You can do this by right-clicking on "Design Sources" in the Sources window, then selecting "Add Sources". Choose your Verilog files from the file browser.

Specify Simulation Settings: Go to "Simulation" > "Simulation Settings". Choose your simulation language (Verilog in this case) and simulation tool (Vivado Simulator).

Run Simulation: Go to "Flow" > "Run Simulation" > "Run Behavioral Simulation". This will launch the Vivado Simulator and compile your design for simulation.

Set Simulation Time: In the Vivado Simulator window, set the simulation time if it's not set automatically. This determines how long the simulation will run.

Run Simulation: Start the simulation by clicking on the "Run" button in the simulation window.

View Results: After the simulation completes, you can view waveforms, debug signals, and analyze the behavior of your design.

Spartan6 FPGA

LOGIC DIAGRAM

SR FLIPFLOP

image

JK FLIPFLOP

image

T FLIPFLOP

image

D FLIPFLOP

image

COUNTER

image

VERILOG CODE
D Flip Flop
module DFlipFlop (D, clk, reset, Q) ;
input D;
input clk;
input reset; 
output reg Q; 
always @ (posedge clk)
begin
    if(reset == 1'b1)
        Q <= 1'b0;
    else
        Q <= D;
end
endmodule
JK Flip Flop
module JK_flipflop (q, q_bar, j,k, clk, reset);
  input j,k,clk, reset;
  output reg q;
  output q_bar;
  always@(posedge clk) begin
    if(!reset)�        q <= 0;
    else 
  begin
      case({j,k})
        2'b00: q <= q;  
        2'b01: q <= 1'b0; 
        2'b10: q <= 1'b1;
        2'b11: q <= ~q; 
      endcase
    end
  end
  assign q_bar = ~q;
endmodule
SR Flip Flop
module SR_flipflop (q, q_bar, s,r, clk, reset);
  input s,r,clk, reset;
  output reg q;
  output q_bar;
  always@(posedge clk) begin 
    if(!reset)�        q <= 0;
    else 
  begin
      case({s,r})
        2'b00: q <= q;    
        2'b01: q <= 1'b0; 
        2'b10: q <= 1'b1; 
        2'b11: q <= 1'bx; 
      endcase
    end
  end
  assign q_bar = ~q;
endmodule
T Flip Flop
module tff (t,clk, rstn,q);  
 input t,clk, rstn;
 output reg q;
  always @ (posedge clk) begin  
    if (!rstn)  
      q <= 0;  
    else  
        if (t)  
            q <= ~q;  
        else  
            q <= q;  
  end  
endmodule
Ripple Carry Counter
module D_FF(q, d, clk, reset);
output q;
input d, clk, reset;
reg q;
always @(posedge reset or negedge clk)
if (reset)
q = 1'b0;
else
q = d;
endmodule
module T_FF(q, clk, reset);
output q;
input clk, reset;
wire d;
D_FF dff0(q, d, clk, reset);
not n1(d, q); 
endmodule
module ripple_carry_counter(q, clk, reset);
output [3:0] q;
input clk, reset;
T_FF tffo(q[0], clk, reset);
T_FF tff1(q[1], q[0], reset);
T_FF tff2(q[2], q[1], reset);
T_FF tff3(q[3], q[2], reset);
endmodule
MOD 10 Counter
module counter(
input clk,rst,enable,
output reg [3:0]counter_output
);
always@ (posedge clk)
begin 
if( rst | counter_output==4'b1001)
counter_output <= 4'b0000;
else if(enable)
counter_output <= counter_output + 1;
else
counter_output <= 0;
end
endmodule
UP-DOWN COUNTER

VERILOG CODE:

module updown_counter(clk,rst,updown,out);
input clk,rst,updown;
output reg [3:0]out;
always@(posedge clk)
begin
if (rst==1)
out=4'b0000;
else if(updown==1)
out=out+1;
else
out=out-1;
end
endmodule
OUTPUT WAVEFORM

D Flip Flop
324338612-16eaae0c-044c-4e5b-a12c-d819fcd455f4

324343987-72ae525c-06de-47e7-bc16-6975cee06f25
JK Flip flop
324338647-b91e64d4-589d-42c8-98f8-e0defd8d8167

324343845-4e699ef4-69e7-48cf-96ed-c19502876284
SR Flip Flop
324338686-ac45a8ed-2c8a-4688-ad43-2cac9b51106e

324343676-d2d32841-0693-4964-881d-08f9ec15fb7b
T Flip FLop
324338729-883e3448-3fcb-4cb6-b2d8-843afe8704fd

324343615-05ca7d14-49d2-4b53-b97f-2b8464ffb28b
MOD-10 COUNTER
324344088-68ca3a3d-432a-4acd-bca7-8e566b06f98f 324344112-96a0dae3-a178-4ef5-8af1-056c7effd627
RIPPLE CARRY COUNTER
324344223-66cfbd77-8a37-413a-8f55-1e034eb051bf 324344265-34cd41d4-b988-4cb4-b548-0a269e53c100
UP DOWN COUNTER
324343532-4093e481-68ab-4d30-8cd5-a91b2933dcdc 324343572-10b19508-5408-46d8-a279-81fdaf7eb2d5
RESULT: Thus the simulation and implementation of sequential logic gates is done and verified.

