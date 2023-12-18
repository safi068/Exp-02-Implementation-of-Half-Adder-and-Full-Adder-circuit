```
name:H.kamsa safi
reg no:23013651
```
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

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### Program:
## Half Adder
```
module halfadder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b)
endmodule
```
## Full Adder
```
module halfadder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
xor(sum,a,b,c);
assign carry=a&b | b&c | a&c
endmodule
```
### TRUTH TABLE 
 
 Half adder circuit

 ![WhatsApp Image 2023-12-18 at 10 32 40_2107160b](https://github.com/safi068/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152167833/abe7b896-d58d-4ffd-b4d8-4b3a8a3b8a78)


Full Adder circuit


![WhatsApp Image 2023-12-18 at 10 32 41_d82a7140](https://github.com/safi068/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152167833/da1a7685-2f97-4781-869a-025a4cf845bc)




### RTL

Half adder circuit


![WhatsApp Image 2023-12-18 at 10 32 39_a96f6f3c](https://github.com/safi068/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152167833/421dc8a8-11e9-417d-b2bd-1e60d57c0969)


Full Adder circuit

![WhatsApp Image 2023-12-18 at 10 32 40_f28471a5](https://github.com/safi068/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152167833/0d8e2639-3193-49d5-b3d5-a70b85c06644)



### TIMING DIAGRAM

Half adder circuit


![WhatsApp Image 2023-12-18 at 10 32 40_a11c8144](https://github.com/safi068/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152167833/c3e0eb3a-0d61-4563-b268-c79d49af5664)


Full Adder circuit

![WhatsApp Image 2023-12-18 at 10 32 41_e072e15d](https://github.com/safi068/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152167833/88dcfb1e-774f-4036-8431-20310366bac3)

### Result:

To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.
