# assingnment

## AIM

To aim for f(A, B, C) = A'B + B'C + BC + AB'C', you would need to design or find a circuit
that implements this Boolean function. This could be done using various logic gates
such as AND, OR, NOT, NAND, NOR, etc.

## EQUIPMENT REQUIRED

Hardware-PCs,cycloneII,USBflasher

software-Quartus prime

## PROCEDURE

connect the supply (+5) to the circuit Switch ON the main switch Press the switches for inputs "A" & "B". Th eswitch is On 
stae when 1 is pressed. The switch is OFF state when 0 is pressed. If the output is 1,then the bulb glows.Check all gates using
Verilog programming.

## EXPLANATION:

The function f(A,B,C) is a Boolean function that takes three binary inputs, A, B, and C, and 
returns a binary output. The function is constructed using logical operations such as AND 
(represented by a dot, '.'), OR (represented by a plus, '+'), and NOT (represented by a prime, ''').

The NOT operator (') inverts the value of the variable.

A' means NOT A.

The AND operator ('.') returns 1 if and only if both inputs are 1.

The OR operator ('+') returns 1 if either or both inputs are 1.

So the function f(A,B,C) = A'B + B'C + BC + AB'C'
can be read as
f(A,B,C) = (NOT A AND B) OR (NOT B AND C) OR (B AND C) OR (A AND NOT B AND NOT C)

The function is a sum-of-products form, where each term in the sum is the product of one or more variables or their complements.

It returns 1 if any of the four logical conditions are true. Otherwise, it returns 0.

## PROGRAM:
 module logic_function(input a, b, c, output f);
 assign f = (!a & b) | (!b & !c) | (b & c) | (a & !b & !c);
endmodule
 

## OUTPUT:  
 
## RTL:
![image](https://user-images.githubusercontent.com/119394582/215339306-529e51ae-9952-47d4-9a7e-8b09f14a69cd.png)



## TIMING DIAGRAM:

![image](https://user-images.githubusercontent.com/119394582/215339324-6975a43c-a03d-4780-8e3a-13adbbfc2a8d.png)


## TRUTH TABLE:

![image](https://user-images.githubusercontent.com/119394582/215339373-7fad8d80-757e-4019-b17e-d747a5285cec.png)


## RESULT:

The program is executed by verilog code successfully.
