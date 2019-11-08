# Integer-Sequence-Learning

## Linear Recurrence Relations

**2nd order recurrence relation**

A second order recurrence relation is of the form:

            a(n+2) = c0*a(n) + c1*a(n+1)
 
where the coefficients  `c0`  and  `c1` are constant.

For example, the Fibonacci sequence  an+2=an+an+1  is a second order recurrence sequence with coefficients  (1,1) .

**3rd order recurrence relation**

A third order recurrence relation is of the form:

            a(n+3) = c0*a(n) + c1*a(n+1) + c2*a(n+2)
 
where the coefficients  `c0`, `c1` and `c2`  are constant.

### Detect Recurrence Relations

Given a sequence  `an` , let's say we want to verify whether it's given by a 3rd order recurrence relation. In other words, we check if it's possible to find constants  `c0`, `c1`, `c2`  so that

            a(n+3) = c0*a(n) + c1*a(n+1) + c2*a(n+2)

is satified. To find possible  `c0`, `c1`, `c2`, since there are 3 unknowns, we need at least 3 equations. Let's set the equations using  `a3`, `a4`, `a5` as follows:

            a3 = c0*a0 + c1*a1 + c2*a2
            a4 = c0*a1 + c1*a2 + c2*a3
            a5 = c0*a2 + c1*a3 + c2*a4

then we solve for  (`c0`, `c1`, `c2`). Once the coefficients  (`c0`, `c1`, `c2`)  are found, we check whether the next terms  `a6`, `a7`... satisfy the recurrence relation.

___
## Polynomial Sequences

**1st order polynomial sequence**

The nth term of a 1st order polynomial sequence is given as

            an = c0*n^0 + c1*n^1

where the coefficients  `c0` and `c1`  are constant.            

**2nd order polynomial sequence**

The nth term of a 2nd order polynomial sequence is given as

            an = c0*n^0 + c1*n^1 + c2*n^2

where the coefficients  `c0`, `c1` and `c2`  are constant.

### Detect Polynomial Sequence

Given a sequence  `an` , let's say we want to verify whether it's given by a 2nd order polynomial sequence. In other words, we check if it's possible to find constants  `c0`, `c1`, `c2`  so that

            an = c0*n^0 + c1*n^1 + c2*n^2

is satified. To find possible  `c0`, `c1`, `c2`, since there are 3 unknowns, we need at least 3 equations. Let's set the equations using  `a0`, `a1`, `a2` as follows:

            a0 = c0*1 + c1*0 + c2*0
            a1 = c0*1 + c1*1 + c2*1
            a2 = c0*1 + c1*2 + c2*4

then we solve for  (`c0`, `c1`, `c2`). Once the coefficients  (`c0`, `c1`, `c2`)  are found, we check whether the next terms  `a3`, `a4`... satisfy the recurrence relation.
___
## References:
* [Recurrrence Relation | Kaggle](https://www.kaggle.com/ncchen/recurrence-relation)