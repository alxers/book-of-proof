Part II
Chapter 4

Definition 4.3 Two integers have the same parity if they are both even or they are both odd. Otherwise they have opposite parity

Definition 4.4 Suppose a and b are integers. We say that a divides b, written a | b, if b = ac for some c in Z. In this case we also say that a is a divisor of b, and that b is a multiple of a.

4.3 Direct Proof
(proposition is a statement that, although true, is not as significant as a theorem.)

Suppose we have:
Proposition If P, then Q.

The goal is to show that this statement is true.
1. When P is false, P => Q is always true, so we don't have to worry about this case.
2. When P is true we must show that Q is also true



*Outline of Direct Proof*

Proposition If P, then Q.

Proof. Suppose P.
...
Therefore Q.

Example:

1) Proposition If x is odd, then x^2 is odd.
Proof. Suppose x is odd.

Therefore x^2 is odd.

2) Proposition If x is odd, then x^2 is odd.    
Proof. Suppose x is odd.    
x = 2b + 1 by definition of an odd number.    
...    
Therefore x^2 is odd.    


3) Proposition If x is odd, then x^2 is odd.    
Proof. Suppose x is odd.    
x = 2a + 1 by definition of an odd number.    
...    
x^2 = 2b + 1    
Therefore x^2 is odd.    


4) Proposition If x is odd, then x^2 is odd.    
Proof. Suppose x is odd.    
x = 2a + 1 by definition of an odd number.    
Then x^2 = (2a + 1)^2 = 4a^2 + 4a + 1 = 2a(2a + 1) + 1    
...    
x^2 = 2b + 1    
Therefore x^2 is odd.    

5) Proposition If x is odd, then x^2 is odd.    
Proof. Suppose x is odd.    
x = 2a + 1 by definition of an odd number.    
Then x^2 = (2a + 1)^2 = 4a^2 + 4a + 1 = 2(2a^2 + 2a) + 1    
So x^2 = 2b + 1 where b = (2a^2 + 2a)    
Therefore x^2 is odd.    


Example:    

Proposition Let a, b and c be integers. If a | b and b | c, then a | c.    

1) Proposition Let a, b and c be integers. If a | b and b | c, then a | c.    
...    
Therefore a | c    

2) Proposition Let a, b and c be integers. If a | b and b | c, then a | c.  
By definition a | b means b = ax, b | c means c = by    
...    
Therefore a | c  

3) Proposition Let a, b and c be integers. If a | b and b | c, then a | c.  
By definition a | b means b = ax, b | c means c = by    
a | c means c = az
Therefore a | c  


Example:    

Proposition If a, b, c ∈ N , then lcm ( ca, cb ) = c · lcm ( a, b ).    

Let m = lcm(ca, cb), n = c * lcm(a, b)    
By definition lcm(a, b) is an integer divisible by a and b, then lcm(a, b) = ax = by    
So n = c * ax = c * by, but m is the *smallest* multiple of ca and cb (by definition). Thus m <= n.    
On the other hand m = lcm(ca, cb) = cax = cby by definition of lcm.    
Then 1/c * m = ax = by is a multiple of a and b. lcm(a, b) <= 1/c * m.    
But c * lcm(a, b) <= m, n <= m.    
Since m <= n and n <=m, must be that n = m.    


Example:

Proposition If x and y are positive and x <= y, then sqrt(x) <= sqrt(y).    
Subtrackt y from both sides x - y <= 0    
sqrt(x)^2 - sqrt(y)^2 <= 0    
(sqrt(x) + sqrt(y))(sqrt(x) - sqrt(y)) <= 0    
Divide both sides by positive (sqrt(x) + sqrt(y))    
sqrt(x) - sqrt(y) <= 0    
Add sqrt(y) to both sides    
sqrt(x) <= sqrt(y)    


Example:

To show that If x and y are positive real numbers, then 2 * sqrt(xy) <= x + y we can start backwards.    
Since we proved that x <= y, then sqrt(x) <= sqrt(y) we can use this property    
4xy <= (x + y)^2    
4xy <= x^2 + 2xy + y^2    
Subtrackt 4xy from both sides    
0 <= x^2 - 2xy + y^2    
0 <= (x - y)^2 which is true, because (x - y)^2 can't be negative    

Proposition If x and y are positive real numbers, then 2 * sqrt(xy) <= x + y.    
Since 0 <= (x - y)^2 holds for all x,y in Z.    
Then 0 <= x^2 - 2xy + y^2      
4xy <= x^2 + 2xy + y^2    
4xy <= (x + y)^2      
Because for all positive x, y in Z it's true that x <= y, then sqrt(x) <= sqrt(y).    
2 * sqrt(xy) <= x + y.    

Example:

Proposition If n in N , then 1 + (-1)^n * (2n - 1) is a multiple of 4.    
There are two cases:    
1) when n is even, n = 2k, k in N.   
2) when n is odd, n = 2k + 1, k in N.    

For the first case we have 1 + 1 * (2 * 2k - 1) = 1 + 4k - 1 = 4k.   
4k is a multiple of 4.   

For the second case we have 1 + ((-1)^(2k + 1)) * (2 * (2k + 1) - 1) = 1 + (-1) * (4k + 2 - 1) = -4k   
-4k is a multiple of 4.     


Example:

Proposition Every multiple of 4 equals 1 + (-1)^n * (2n - 1) for some n in N.    

Exercises for Chapter 4
Use the method of direct proof to prove the following statements.
1. If x is an even integer, then x^2 is even.  
