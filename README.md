# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit
## Name: DURGADEVI P
## Reg no: 212223100006
## AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.
## Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
## Theory:
Adders are digital circuits that carry out addition of numbers.
## Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB
## Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

#### Figure -01 HALF ADDER
 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -02 FULL ADDER  
![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

## Procedure:

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
## Program:

```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: DURGADEVI P 
Register Number: 212223100006
```
### Half adder:
```
module halfadder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b)
endmodule
```
### Full adder:
```
module halfadder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
xor(sum,a,b,c);
assign carry=a&b | b&c | a&c
endmodule
```
## Truthtable:
### Half adder circiut:
![image](https://github.com/durgadevi22d/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149987216/4f13c8b8-65b2-4043-88c4-3fd2edd2dd5c)
### Full adder circuit:
![image](https://github.com/durgadevi22d/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149987216/ceef0a26-bcbe-4c13-8d4d-50b288b9c344)

## RTL realization:
### Half adder circuit:
![image](https://github.com/durgadevi22d/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149987216/aec5871d-4e9c-48e1-a42d-84e1a5bc2fb0)
### Full adder circuit:
![image](https://github.com/durgadevi22d/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149987216/bd3e68c0-8ab3-4c30-932f-bc8ebe9c11c4)
## Output:
### Half adder:
![image](https://github.com/durgadevi22d/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149987216/4881d068-92f9-4041-a99e-a24da6cee988)

### Full adder:
![image](https://github.com/durgadevi22d/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149987216/7ca5e96e-7d58-4663-8c22-225eb554e668)
## Result:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming
