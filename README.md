# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

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
Connect the supply (+5V) to the circuit Switch ON the main switch If the output is 1, then the led glows.

### 
Program:

```Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by:Gokul J 
RegisterNumber:212222230038
```

## HALF ADDER

```module half_adder(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum = (a^b);
assign carry = (a&b);
endmodule
```
## FULL ADDER

```module full_adder (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = (a^b^c);
assign carry = ((a&b)|(a^b)&c);
endmodule
```
## output

## Logic symbol & Truthtable

RTL realization

## HALF ADDER
![Screenshot 2023-04-23 210816](https://user-images.githubusercontent.com/121165938/233849608-4d7eb01a-ff29-4a04-afdf-2472580a101e.png)

## FULL ADDER
![Screenshot 2023-04-23 210843](https://user-images.githubusercontent.com/121165938/233849687-21bafe82-a379-471b-bce3-3faa9877050d.png)


### Output:

### RTL

## HALF ADDER
![Screenshot 2023-04-23 210858](https://user-images.githubusercontent.com/121165938/233849742-677c7268-c0f3-4a03-9fc6-07b04449c4db.png)

## FULL ADDER
![Screenshot 2023-04-23 210908](https://user-images.githubusercontent.com/121165938/233849868-e1bb2742-7072-48d1-83c4-bda0ad53aad5.png)

RTL

### TIMING DIAGRAM

## HALF ADDER
![Screenshot 2023-04-23 210920](https://user-images.githubusercontent.com/121165938/233850006-a181a137-7ae4-4146-a0c6-92de7ae2298d.png)

## FULL ADDER
![Screenshot 2023-04-23 210938](https://user-images.githubusercontent.com/121165938/233850227-d7442647-1d5a-4150-87ab-870b1911ff50.png)



### Result:
Thus,the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
