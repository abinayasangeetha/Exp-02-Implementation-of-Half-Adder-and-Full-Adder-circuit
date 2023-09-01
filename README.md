```
Name : ABINAYA S
REG NO : 212222230002
```
## Implementation of Half Adder and Full Adder circuit


### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
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

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
```
Developed by: ABINAYA S
RegisterNumber:  212222230003
```
## Half Adder:
module EX03(a,b,c,s);
input a,b;
output s,c;
assign s=a^b;
assign c=a&b;
endmodule
## Full Adder:
module ex3(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum=a^b^c;
assign carry=((a&b)|(b&c)|(c&a));
endmodule

### RTL Diagram:
## Half Adder:
![RTLVIEW3](https://github.com/abinayasangeetha/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119393675/0e8afff2-ab8d-4302-8443-f3ade699b902)

## Full Adder:
![fullRtl3](https://github.com/abinayasangeetha/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119393675/2b14603c-f445-4688-a435-46a606c05139)

## Waveform:
## Half Adder:
![half wf3](https://github.com/abinayasangeetha/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119393675/3050e0a3-3e19-4688-9ea9-371a37e6fe61)

## Full Adder:
![FULLWF3](https://github.com/abinayasangeetha/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119393675/5fabee84-d3be-4097-b80c-ce2064a8cf25)
 


### TRUTH TABLE :
## Half Adder:
![half TT3](https://github.com/abinayasangeetha/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119393675/19f9558e-c5a9-4aa1-acdc-abd46ded8764)

## Full Adder:
![FULLTT3](https://github.com/abinayasangeetha/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119393675/255a5ea9-22ff-44b5-8889-5f79d24691fa)

### Result:
