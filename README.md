```
Name : ABINAYA S
REG NO : 212222230002
```
## Exp 03 Implementation of Half Adder and Full Adder circuit


### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Components Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
## Theory:
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure :
1. Create a New Project:
   - Open Quartus and create a new project by selecting "File" > "New Project Wizard."
   - Follow the wizard's instructions to set up your project, including specifying the project name, location, and target device (FPGA).

2. Create a New Design File:
   - Once the project is created, right-click on the project name in the Project Navigator and select "Add New File."
   - Choose "Verilog HDL File" or "VHDL File," depending on your chosen hardware description language.

3. Write the Combinational Logic Code:
   - Open the newly created Verilog or VHDL file and write the code for your combinational logic.
     
4. Compile the Project:
   - To compile the project, click on "Processing" > "Start Compilation" in the menu.
   - Quartus will analyze your code, synthesize it into a netlist, and perform optimizations based on your target FPGA device.

5. Analyze and Fix Errors:
   - If there are any errors or warnings during the compilation process, Quartus will display them in the Messages window.
   - Review and fix any issues in your code if necessary.
   - View the RTL diagram.

6. Verification:
   - Click on "File" > "New" > "Verification/Debugging Files" > "University Program VWF".
   - Once Waveform is created Right Click on the Input/Output Panel > " Insert Node or Bus" > Click on Node Finder > Click On "List" > Select All.
   - Give the Input Combinations according to the Truth Table amd then simulate the Output Waveform.

### Program:
```
Developed by: ABINAYA S
RegisterNumber:  212222230002
```
## Half Adder:
```
module EX03(a,b,c,s);
input a,b;
output s,c;
assign s=a^b;
assign c=a&b;
endmodule
```
## Full Adder:
```
module ex3(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum=a^b^c;
assign carry=((a&b)|(b&c)|(c&a));
endmodule
```
### RTL Diagram:
## Half Adder:
![RTLVIEW3](https://github.com/abinayasangeetha/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119393675/0e8afff2-ab8d-4302-8443-f3ade699b902)

## Full Adder:
![fullRtl3](https://github.com/abinayasangeetha/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119393675/2b14603c-f445-4688-a435-46a606c05139)
### TRUTH TABLE :
## Half Adder:
![half TT3](https://github.com/abinayasangeetha/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119393675/19f9558e-c5a9-4aa1-acdc-abd46ded8764)

## Full Adder:
![FULLTT3](https://github.com/abinayasangeetha/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119393675/255a5ea9-22ff-44b5-8889-5f79d24691fa)

## Output Waveform:
## Half Adder:
![half wf3](https://github.com/abinayasangeetha/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119393675/3050e0a3-3e19-4688-9ea9-371a37e6fe61)

## Full Adder:
![FULLWF3](https://github.com/abinayasangeetha/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119393675/5fabee84-d3be-4097-b80c-ce2064a8cf25)
 


### Result:
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
