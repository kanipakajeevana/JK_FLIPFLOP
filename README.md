# JK_FLIPFLOP
# AIM
To simulate and synthesis JK flipflop using vivado.
# APPARATUS REQUIRE
Vivado 2023.2 software
# PROCEDURE
STEP:1 Start the vivado software, Select and Name the New project.

STEP:2 Select the device family, device, package and speed.

STEP:3 Select new source in the New Project and select Verilog Module as the Source type.

STEP:4 Type the File Name and module name and Click Next and then finish button. Type the code and save it.

STEP:5 Select the run simulation and then run Behavioral Simulation in the Source Window and click the check syntax.

STEP:6 Click the simulation to simulate the program and give the inputs and verify the outputs as per the truth table.

STEP:7 compare the output with truth table.
# Circuit Diagram
![image](https://github.com/kanipakajeevana/JK_FLIPFLOP/assets/170450203/b5bce14e-4ce1-4f5f-adfe-e197f6e3d0e7)
![image](https://github.com/kanipakajeevana/JK_FLIPFLOP/assets/170450203/976204c8-3774-496a-b0d5-eaa6753d530b)


# Truth Table
![image](https://github.com/kanipakajeevana/JK_FLIPFLOP/assets/170450203/2736fb47-a79f-4b8c-b607-eb6561fe9f3d)
# PROGRAM
module jkff(clk,j,k,rst,q );
input j,k,clk,rst;
output reg q;
always@(posedge clk)
begin
if(rst==1)
q=1'b0;
else
begin
case({j,k})
2'b00: q=q;
2'b01:q=1'b0;
2'b10:q=1'b1;
2'b11:q=~q;
endcase
end
end
endmodule
# OUTPUT
![image](https://github.com/kanipakajeevana/JK_FLIPFLOP/assets/170450203/2c5eac16-0c21-48e8-8f26-c5ca8219a4a3)
# RESULT
Thus the verilog program for JK flipflop has been simulated and verified successfully.



