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

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: yuva krishna k
RegisterNumber:  212222110056
*/

1.
```
module halfadder(A,B,sum,carry);
input A,B;
output sum,carry;
assign sum= A^B;
assign carry = A&B;
endmodule

```
2.
```
module fulladder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum=a^b^c;
assign carry=((a&b)|(b&c)|(c&a));
endmodule 
```
### Output:
![Screenshot (97)](https://github.com/Yuvakrishna0/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/117915037/53b8df3f-d70a-4b1a-a5d4-8fc26e4b6f5a)

![Screenshot 2023-09-01 090708](https://github.com/Yuvakrishna0/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/117915037/349cce35-5201-4458-9523-ae40ddd047df)

### RTL:
![Screenshot (96)](https://github.com/Yuvakrishna0/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/117915037/620eea87-19e8-4ddd-9f6b-f955ec1aee89)


![Screenshot 2023-09-01 090416](https://github.com/Yuvakrishna0/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/117915037/2c12870a-1754-4391-9da5-b7b789c4cf7b)


### TRUTH TABLE 
![Screenshot 2023-09-01 091842](https://github.com/Yuvakrishna0/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/117915037/ef6e504b-7ec1-4024-9817-71d1025e7084)


![Screenshot 2023-09-01 092248](https://github.com/Yuvakrishna0/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/117915037/82f5559f-74d2-47f1-95cc-de280c617750)

### Result:
Thus the program to implement half adder and full adder is executed successfully.
