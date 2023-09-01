# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
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

### Procedure :

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
/*
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: JEEVAGOWTHAM S
RegisterNumber:  212222230053
*/
```
## HALF ADDER:
```
module exp33(a,b,s,c);
input a,b;
output s,c;
assign s=a^b;
assign c=a&b;
endmodule
```

## FULL ADDER:
```
module ass3(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum=a^b^c;
assign carry= ((a&b)|(b&c)|(c&a));
endmodule
```


Logic symbol & Truthtable
RTL realization

### Output:
### RTL
# HALF ADDER:
![Screenshot 2023-09-01 085510](https://github.com/JeevaGowtham-S/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118042624/084d609b-1bb0-4f47-82fe-3fb1dda94395)
# FULL ADDER:
![Screenshot 2023-09-01 091422](https://github.com/JeevaGowtham-S/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118042624/6ca1e10c-a439-49f7-b7cb-cb7ed7b5e66e)



### TIMING DIAGRAM:
# HALF ADDER:
![Screenshot (123)](https://github.com/JeevaGowtham-S/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118042624/95eccf36-94f9-4925-ad15-82c9579880aa)


# FULL ADDER:
![Screenshot (124)](https://github.com/JeevaGowtham-S/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118042624/863312c7-17df-4b4c-9958-768cbbcf34e6)




### TRUTH TABLE :
# HALF ADDER:
![TT 1](https://github.com/JeevaGowtham-S/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118042624/9cd28690-b0b2-4e1f-8f6a-dcf9a657d344)

# FULL ADDER:
![FULL ADDER](https://github.com/JeevaGowtham-S/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118042624/bb1b445a-65fa-4c1f-80fe-aca2993690f6)


### Result:
Thus the half adder and full adder are studied and the truth table for different logic gates are verified.
