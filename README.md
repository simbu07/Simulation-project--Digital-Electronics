##  logic diagram using Verilog
### AIM
Design and simulate the logic diagram using Verilog. F=(X+Y')(X'+Y)Z'

### THEORY
Product Of Sum: i.) POS stands for Product of Sums. ii.) It is a technique of defining boolean terms as a product of sum terms. iii.) It prefers maxterms. iv.) In the case of POS, the Maxterms are defined as ‘M’ v.) It gives LOW(0) output. vi.) In POS, we can get the final term by multiplying the sum terms.

### K map:
A Karnaugh map (K-map) is a visual method used to simplify the algebraic expressions in Boolean functions without having to resort to complex theorems or equation manipulations. A K-map can be thought of as a special version of a truth table that makes it easier to map out parameter values and arrive at a simplified Boolean expression.


### PROGRAM
```
Name:Silambarasan K
Reg No:212222230101
```
```
module assignment1 (x,y,z,f);
input x,y,z;
output f;
wire a,b,c,d,e;
not (a,x);
not (b,y);
not (c,z);
and (d,a,b,c);
and (e,x,y,c);
or (f,d,e);
endmodule
```
### LOGIC DIAGRAM
![M](https://user-images.githubusercontent.com/117919362/239695084-f5c3e161-e811-4e4a-9ed8-7bbdb624d2d2.png)
#### NETLIST DIAGRAM
![m](https://user-images.githubusercontent.com/117919362/239695213-46f58906-fddf-431b-b558-e9ef2a7d643d.png)
### TIMING DIAGRAM
![n](https://user-images.githubusercontent.com/117919362/239695084-f5c3e161-e811-4e4a-9ed8-7bbdb624d2d2.png)

### REFERENCE
https://www.electroniclinic.com/sop-and-pos-digital-logic-designing-with-solved-examples/
