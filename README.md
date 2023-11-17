# TITLE
Minimise the function using K map F(A,B,C)=ABC+B'C'+BC+AB' and simulate the logic diagram using verilog.

# THEORY

K-Map:
    
    The K-map is a systematic way of simplifying Boolean expressions.With the help of the K-map method, we can find the simplest POS and SOP expression, which is known as the minimum expression. The K-map provides a cookbook for simplification.The 3-variable K-map is represented as an array of eight cells. In this case, we used A, B, and C for the variable. We can use any letter for the names of the variables. The binary values of variables A and B are along the left side, and the values of C are across the top. The value of the given cell is the binary values of A and B at left side in the same row combined with the value of C at the top in the same column. For example, the cell in the upper left corner has a binary value of 000, and the cell in the lower right corner has a binary value of 101.

![Simulation-project--Digital-Electronics](simu3.png)

# PROCEDURE

1.Simplify and Minimise the given function.

2.Draw the K-map for the same.

3.Obtain the minimised function.

4.Open the Quartus software and create a new file.

5.Feed and run the program .

6.The RTL viewer and the timing diagram will be displayed.


# PROGRAM

```
module logic(a,b,c,F);
input a,b,c;
output F;
assign F=(((~b&~c)|(a&c))|(b&c));
endmodule
```

# RTL VIEWER
![Simulation-project--Digital-Electronics](simu1.png)

# TIMING DIAGRAM
![Simulation-project--Digital-Electronics](simu2.png)

# RESULT
    Thus the program to minimise the function using K map is implemented and executed successfully.
