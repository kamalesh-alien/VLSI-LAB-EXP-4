
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


https://private-user-images.githubusercontent.com/6987778/301740946-77fb7f38-5649-4778-a987-8468df9ea3c3.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTQzNjg4NzYsIm5iZiI6MTcxNDM2ODU3NiwicGF0aCI6Ii82OTg3Nzc4LzMwMTc0MDk0Ni03N2ZiN2YzOC01NjQ5LTQ3NzgtYTk4Ny04NDY4ZGY5ZWEzYzMucG5nP1gtQW16LUFsZ29yaXRobT1BV1M0LUhNQUMtU0hBMjU2JlgtQW16LUNyZWRlbnRpYWw9QUtJQVZDT0RZTFNBNTNQUUs0WkElMkYyMDI0MDQyOSUyRnVzLWVhc3QtMSUyRnMzJTJGYXdzNF9yZXF1ZXN0JlgtQW16LURhdGU9MjAyNDA0MjlUMDUyOTM2WiZYLUFtei1FeHBpcmVzPTMwMCZYLUFtei1TaWduYXR1cmU9OTU1ZTIxMTlmMjMzMjJkNDE3NzFjMzRhNmI4M2RiN2Y5MzczZjNmNDdmNTc3OWI2Yzc1YTIzZGJiN2VhOWI0MCZYLUFtei1TaWduZWRIZWFkZXJzPWhvc3QmYWN0b3JfaWQ9MCZrZXlfaWQ9MCZyZXBvX2lkPTAifQ.3kBLPkuXTieOFzFLhvlZ3rzSvsHxSTM37v7jyR0DNps

JK FLIPFLOP

https://private-user-images.githubusercontent.com/6987778/301743103-1510e030-4ddc-42b1-88ce-d00f6f0dc7e6.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTQzNjg4NzYsIm5iZiI6MTcxNDM2ODU3NiwicGF0aCI6Ii82OTg3Nzc4LzMwMTc0MzEwMy0xNTEwZTAzMC00ZGRjLTQyYjEtODhjZS1kMDBmNmYwZGM3ZTYucG5nP1gtQW16LUFsZ29yaXRobT1BV1M0LUhNQUMtU0hBMjU2JlgtQW16LUNyZWRlbnRpYWw9QUtJQVZDT0RZTFNBNTNQUUs0WkElMkYyMDI0MDQyOSUyRnVzLWVhc3QtMSUyRnMzJTJGYXdzNF9yZXF1ZXN0JlgtQW16LURhdGU9MjAyNDA0MjlUMDUyOTM2WiZYLUFtei1FeHBpcmVzPTMwMCZYLUFtei1TaWduYXR1cmU9MjUzNzMyNTZkYTdhYTEyMjM4NmFlMGQwY2VjNzdlYmFhOGNlNjZkMWM1YjJjZmQ3MjkwNTQyZjQ1YjBmN2M4YSZYLUFtei1TaWduZWRIZWFkZXJzPWhvc3QmYWN0b3JfaWQ9MCZrZXlfaWQ9MCZyZXBvX2lkPTAifQ.amTsZZ0u_QVnbdaX5TRt8qngEdE31MfPoTK6BTS4Z-Y

T FLIPFLOP

https://private-user-images.githubusercontent.com/6987778/301743290-7a020379-efb1-4104-85ee-439d660baa08.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTQzNjg4NzYsIm5iZiI6MTcxNDM2ODU3NiwicGF0aCI6Ii82OTg3Nzc4LzMwMTc0MzI5MC03YTAyMDM3OS1lZmIxLTQxMDQtODVlZS00MzlkNjYwYmFhMDgucG5nP1gtQW16LUFsZ29yaXRobT1BV1M0LUhNQUMtU0hBMjU2JlgtQW16LUNyZWRlbnRpYWw9QUtJQVZDT0RZTFNBNTNQUUs0WkElMkYyMDI0MDQyOSUyRnVzLWVhc3QtMSUyRnMzJTJGYXdzNF9yZXF1ZXN0JlgtQW16LURhdGU9MjAyNDA0MjlUMDUyOTM2WiZYLUFtei1FeHBpcmVzPTMwMCZYLUFtei1TaWduYXR1cmU9YWRmMjk1MTFjNWI1ZmZkODQ1MDNiZWNlZTQ1MmI4NTY3NjQ4OWYyMDFkOGQwOTZmZWExMjVkZDNlNzIxZDBlMCZYLUFtei1TaWduZWRIZWFkZXJzPWhvc3QmYWN0b3JfaWQ9MCZrZXlfaWQ9MCZyZXBvX2lkPTAifQ.1bpjGw39KDQDnMJf6lji3SYBf9YHI0rFzScbBOdyKNA

D FLIPFLOP

https://private-user-images.githubusercontent.com/6987778/301743389-dda843c5-f0a0-4b51-93a2-eaa4b7fa8aa0.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTQzNjg4NzYsIm5iZiI6MTcxNDM2ODU3NiwicGF0aCI6Ii82OTg3Nzc4LzMwMTc0MzM4OS1kZGE4NDNjNS1mMGEwLTRiNTEtOTNhMi1lYWE0YjdmYThhYTAucG5nP1gtQW16LUFsZ29yaXRobT1BV1M0LUhNQUMtU0hBMjU2JlgtQW16LUNyZWRlbnRpYWw9QUtJQVZDT0RZTFNBNTNQUUs0WkElMkYyMDI0MDQyOSUyRnVzLWVhc3QtMSUyRnMzJTJGYXdzNF9yZXF1ZXN0JlgtQW16LURhdGU9MjAyNDA0MjlUMDUyOTM2WiZYLUFtei1FeHBpcmVzPTMwMCZYLUFtei1TaWduYXR1cmU9OGZlNjc5YzZiNmM1YWRhM2NkNWZjMjE0NjNmNmFiZWQ0MTJmOTgzMTYwZjcxYTEwNWViZDk4OTg1ZGNhYjVmOCZYLUFtei1TaWduZWRIZWFkZXJzPWhvc3QmYWN0b3JfaWQ9MCZrZXlfaWQ9MCZyZXBvX2lkPTAifQ.v7dy7UNQUS43CY_K541sZc0IPBBK1lPjNOOQIFOwQJU

COUNTER
https://private-user-images.githubusercontent.com/6987778/301743514-a1fc5f68-aafb-49a1-93d2-779529f525fa.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTQzNjg4NzYsIm5iZiI6MTcxNDM2ODU3NiwicGF0aCI6Ii82OTg3Nzc4LzMwMTc0MzUxNC1hMWZjNWY2OC1hYWZiLTQ5YTEtOTNkMi03Nzk1MjlmNTI1ZmEucG5nP1gtQW16LUFsZ29yaXRobT1BV1M0LUhNQUMtU0hBMjU2JlgtQW16LUNyZWRlbnRpYWw9QUtJQVZDT0RZTFNBNTNQUUs0WkElMkYyMDI0MDQyOSUyRnVzLWVhc3QtMSUyRnMzJTJGYXdzNF9yZXF1ZXN0JlgtQW16LURhdGU9MjAyNDA0MjlUMDUyOTM2WiZYLUFtei1FeHBpcmVzPTMwMCZYLUFtei1TaWduYXR1cmU9MzljZmM0ZmM4NDE0ODM1MTAyM2NiNDkxMjM5ZDJjNjk2NDk5OWI5YTU2NGMzOWYyYTM5MzY3MDA5YzgwNjFhYiZYLUFtei1TaWduZWRIZWFkZXJzPWhvc3QmYWN0b3JfaWQ9MCZrZXlfaWQ9MCZyZXBvX2lkPTAifQ.xaM2NTFw25G-rPkbLoJr6K2C52SNkTUtVvWZBP5ytYw


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
https://private-user-images.githubusercontent.com/160568583/326332237-b9f321af-c3a5-4188-9622-b3558baf683b.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTQzNjg4NzYsIm5iZiI6MTcxNDM2ODU3NiwicGF0aCI6Ii8xNjA1Njg1ODMvMzI2MzMyMjM3LWI5ZjMyMWFmLWMzYTUtNDE4OC05NjIyLWIzNTU4YmFmNjgzYi5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNDI5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDQyOVQwNTI5MzZaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1mNDE3ZDA3ZmExODRhMTUyYzNiZTc0MDkyNDA0MzY2ZmUwODgwNjIyYjQwZjg1NGM0YTkxYzQ5NWMyMzdhZDBkJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.Dx7p3rIWYv42ZISsnV-mFLbnRRX4qi952KkzDINzLMs

https://private-user-images.githubusercontent.com/160568583/326332264-a25bf3f2-cd76-4299-b77e-996da33e3835.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTQzNjg4NzYsIm5iZiI6MTcxNDM2ODU3NiwicGF0aCI6Ii8xNjA1Njg1ODMvMzI2MzMyMjY0LWEyNWJmM2YyLWNkNzYtNDI5OS1iNzdlLTk5NmRhMzNlMzgzNS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNDI5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDQyOVQwNTI5MzZaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1mYzE3N2U3MmZiNDlhOGI3ZjIxNGNjNmVkYzc0OTlkZjdmYWE3NjQ2OThjOWJmMzM4OTRhNzlmYWI5ZTFjNDhmJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.8wawHd6SsZxOjLsevIyrytFvAgD9lJIxviiABSvuZQQ
JK Flip flop
https://private-user-images.githubusercontent.com/160568583/326332302-09257289-827d-46b6-98f4-5f70b562f62c.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTQzNjg4NzYsIm5iZiI6MTcxNDM2ODU3NiwicGF0aCI6Ii8xNjA1Njg1ODMvMzI2MzMyMzAyLTA5MjU3Mjg5LTgyN2QtNDZiNi05OGY0LTVmNzBiNTYyZjYyYy5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNDI5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDQyOVQwNTI5MzZaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT0zMDBmNmQ2YTZlMzk5M2E2ZWYzNzUzYWY4MDllZmIxMmJlZWFlNzliYzg3Y2E5MjJlMjgyNGNmZDE0M2YzZDlhJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.pmnxf6ZzyK9Vtbt8IFbnYrILWr7lJOSsHWtZBBHN9HE

https://private-user-images.githubusercontent.com/160568583/326332331-f3e56281-727e-4fa2-b119-9117bda83d38.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTQzNjg4NzYsIm5iZiI6MTcxNDM2ODU3NiwicGF0aCI6Ii8xNjA1Njg1ODMvMzI2MzMyMzMxLWYzZTU2MjgxLTcyN2UtNGZhMi1iMTE5LTkxMTdiZGE4M2QzOC5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNDI5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDQyOVQwNTI5MzZaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT01MTM1NTI0ODg4NzRjOWM5Yzk3Njk3MDZiYTc4YzY1YzY2OWEyMGNlYTAyODJjZjg4MDY3OTA0NWMzZmQ2NzBmJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.xHWCvPSbjoyzpfUijur9N6YBEfrmOgISl1R5Nj0YDiU

SR Flip Flop
https://private-user-images.githubusercontent.com/160568583/326332351-4077a870-f8c0-4f94-8633-9a25f7e2f30c.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTQzNjg4NzYsIm5iZiI6MTcxNDM2ODU3NiwicGF0aCI6Ii8xNjA1Njg1ODMvMzI2MzMyMzUxLTQwNzdhODcwLWY4YzAtNGY5NC04NjMzLTlhMjVmN2UyZjMwYy5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNDI5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDQyOVQwNTI5MzZaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT0zYTVkODRjYjIyZTY0MzkyYTk3YjdhOTdmOGJiY2I3MmM1MDVjYzg2NGU3Yzc2MWRhM2I4YzI5MTJkZGQ1MDExJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.jUkqMlThlkKQkP4THsvego445VbdYFltSBhUMlyw_gM
https://private-user-images.githubusercontent.com/160568583/326332364-47e513d6-f813-47df-a836-a9c59cfa5171.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTQzNjg4NzYsIm5iZiI6MTcxNDM2ODU3NiwicGF0aCI6Ii8xNjA1Njg1ODMvMzI2MzMyMzY0LTQ3ZTUxM2Q2LWY4MTMtNDdkZi1hODM2LWE5YzU5Y2ZhNTE3MS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNDI5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDQyOVQwNTI5MzZaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT03MGM1MjQyNzBkYTkwM2E2YzdmNjVlMjI2MTcxM2I1NzdmM2ZjMDc4ZTJiYzFlZjE4ZDY5YjE2ZDlmODYyMDI5JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.SRJyJZUn1YQEGWR1W11l8rsjH44ZGwyGkWNke_kFI5k
T Flip FLop
https://private-user-images.githubusercontent.com/160568583/326332398-b0e8a2bf-fd39-4938-bc69-01ace61b6ffa.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTQzNjg4NzYsIm5iZiI6MTcxNDM2ODU3NiwicGF0aCI6Ii8xNjA1Njg1ODMvMzI2MzMyMzk4LWIwZThhMmJmLWZkMzktNDkzOC1iYzY5LTAxYWNlNjFiNmZmYS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNDI5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDQyOVQwNTI5MzZaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT03OGUwY2Y2ZDNhNmRlNDQ4NzAxODBhN2I2NmI1ODRmNDU3OWUzMzY3YmExZGFlZjU0Y2I4ZDdlZTZjOTUyM2UwJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.MQRWiIgTIK3dmmbeLwG1ZCQDbSauAdOaHGFzGcGlUY8
https://private-user-images.githubusercontent.com/160568583/326332404-ee6e187c-6632-417e-adc4-baa9f6c5ae21.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTQzNjg4NzYsIm5iZiI6MTcxNDM2ODU3NiwicGF0aCI6Ii8xNjA1Njg1ODMvMzI2MzMyNDA0LWVlNmUxODdjLTY2MzItNDE3ZS1hZGM0LWJhYTlmNmM1YWUyMS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNDI5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDQyOVQwNTI5MzZaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT0xYzY1MTNiOGIyNmM5ZmY2Y2EzMWRkZWJiNDc0NDAzNzdjZjA2MTBiM2JlNWRiNGUxYTAxMWQ4YTk5YTNlYWY0JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.kEH5aQIU2MN3UFtITN56NtcNlLdK17AzeWsoDX65GPM

MOD-10 COUNTER
https://private-user-images.githubusercontent.com/160568583/326332435-b7fdb83e-6c45-4404-89df-fdc217824ecd.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTQzNjg4NzYsIm5iZiI6MTcxNDM2ODU3NiwicGF0aCI6Ii8xNjA1Njg1ODMvMzI2MzMyNDM1LWI3ZmRiODNlLTZjNDUtNDQwNC04OWRmLWZkYzIxNzgyNGVjZC5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNDI5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDQyOVQwNTI5MzZaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT01ZjJlYmU2ODEzYmY3NzA3NGFiMTQwOTIwYTUxNmFhOWQ0ZjBlYjU3MTYxNjg2MjZmYTczOGI4MTQ1MjY5OTk2JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJ

https://private-user-images.githubusercontent.com/160568583/326332446-74e494dd-a3c9-465e-b5a8-3da59877a545.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTQzNjg4NzYsIm5iZiI6MTcxNDM2ODU3NiwicGF0aCI6Ii8xNjA1Njg1ODMvMzI2MzMyNDQ2LTc0ZTQ5NGRkLWEzYzktNDY1ZS1iNWE4LTNkYTU5ODc3YTU0NS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNDI5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDQyOVQwNTI5MzZaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT0yOGJhZjY5OWE1YzdjZThmYjY1YWFkYTQ0MzNiYTYzYTdjMWRkNGUyY2ZkMzY5NmE4ZDRiZDY5OTIyNGVlNGI3JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.SbgXGXgl325euOWn0OFG8q3wcxHAhwfSiCdy5xIvqkUmtleV9pZD0wJnJlcG9faWQ9MCJ9.vmeuTgl5PCJg6P_sOGHI_6oc2-LmkkDsrJheJnw0aT0

RIPPLE CARRY COUNTER
https://private-user-images.githubusercontent.com/160568583/326332470-fa1d7d09-667c-4b17-a07c-830fcf352ae9.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTQzNjg4NzYsIm5iZiI6MTcxNDM2ODU3NiwicGF0aCI6Ii8xNjA1Njg1ODMvMzI2MzMyNDcwLWZhMWQ3ZDA5LTY2N2MtNGIxNy1hMDdjLTgzMGZjZjM1MmFlOS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNDI5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDQyOVQwNTI5MzZaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT03ZThlNGViYWQ0NTQ1MzM4OWUzZDM0YzgyNWRjNjViMjRmNWFlMzlkYjMzZGMwNWZiODJhYjY3YjIxNTdmOTEzJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.wEJACA3vNeq9gXE6DebbuiKaA_w35wLNccEhXhIoyCc 
https://private-user-images.githubusercontent.com/160568583/326332477-f842d2db-6535-4935-ad18-ddfaf57dc1e6.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTQzNjg4NzYsIm5iZiI6MTcxNDM2ODU3NiwicGF0aCI6Ii8xNjA1Njg1ODMvMzI2MzMyNDc3LWY4NDJkMmRiLTY1MzUtNDkzNS1hZDE4LWRkZmFmNTdkYzFlNi5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNDI5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDQyOVQwNTI5MzZaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT01Y2E4YTBmOWU1ZWYxMWVlY2I0MTlmYjAwZjE5OTIwZDUwMDkyNWJlNjQ4OTJlODRlNjI4MTZkYjBkNzM4NWYzJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.qC-BKACiQECJyf3HaM2DxlKn_uQE8qfs5IwrHCXqusM

UP DOWN COUNTER
https://private-user-images.githubusercontent.com/160568583/326332470-fa1d7d09-667c-4b17-a07c-830fcf352ae9.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTQzNjg4NzYsIm5iZiI6MTcxNDM2ODU3NiwicGF0aCI6Ii8xNjA1Njg1ODMvMzI2MzMyNDcwLWZhMWQ3ZDA5LTY2N2MtNGIxNy1hMDdjLTgzMGZjZjM1MmFlOS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNDI5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDQyOVQwNTI5MzZaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT03ZThlNGViYWQ0NTQ1MzM4OWUzZDM0YzgyNWRjNjViMjRmNWFlMzlkYjMzZGMwNWZiODJhYjY3YjIxNTdmOTEzJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.wEJACA3vNeq9gXE6DebbuiKaA_w35wLNccEhXhIoyCc

https://private-user-images.githubusercontent.com/160568583/326332477-f842d2db-6535-4935-ad18-ddfaf57dc1e6.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTQzNjg4NzYsIm5iZiI6MTcxNDM2ODU3NiwicGF0aCI6Ii8xNjA1Njg1ODMvMzI2MzMyNDc3LWY4NDJkMmRiLTY1MzUtNDkzNS1hZDE4LWRkZmFmNTdkYzFlNi5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNDI5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDQyOVQwNTI5MzZaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT01Y2E4YTBmOWU1ZWYxMWVlY2I0MTlmYjAwZjE5OTIwZDUwMDkyNWJlNjQ4OTJlODRlNjI4MTZkYjBkNzM4NWYzJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.qC-BKACiQECJyf3HaM2DxlKn_uQE8qfs5IwrHCXqusM
RESULT: Thus the simulation and implementation of sequential logic gates is done and verified.

