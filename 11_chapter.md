Relations

Definition 11.1 A relation on a set A is a subset R set_in A x A. Abbreviated as (x, y) in R as xRy.     

Example 11.1 Let A = { 1, 2, 3, 4 }.     
R = { (1, 1), (2, 1), (2, 2), (3, 3), (3, 2), (3, 1), (4, 4), (4, 3), (4, 2), (4, 1) } set_in A x A.     
1R1, 2R1, ... etc.     
R is greater-then-or-equal set.     


Exercises for Section 11.1.     
.1. Let A = { 0, 1, 2, 3, 4, 5 }. Write out the relation R that express > on A.     
R = {     
    (1, 0), (2, 0), (3, 0), (4, 0), (5, 0),     
    (2, 1), (3, 1), (4, 1), (5, 1),     
    (3, 2), (4, 2), (5, 2),          
    (4, 3), (5, 3),               
    (5, 4)                    
}      


.2. Let A = { 1, 2, 3, 4, 5, 6 }. Write out the relation R that express | (divides) on A.     
R = {     
    (1, 1), (1, 2), (1, 3), (1, 4), (1, 5), (1, 6),      
    (2, 2), (2, 4), (2, 6),           
    (3, 3), (3, 6),                
    (4, 4),                
    (5, 5),                
    (6, 6)                
}   


.3. Let A = { 0, 1, 2, 3, 4, 5 }. Write out the relation R that express >= on A.     
R = {     
    (0, 0), (1, 0), (2, 0), (3, 0), (4, 0), (5, 0),     
    (1, 1), (2, 1), (3, 1), (4, 1), (5, 1),     
    (2, 2), (3, 2), (4, 2), (5, 2),          
    (4, 4), (4, 3), (5, 3),               
    (5, 5), (5, 4)                    
}      


.4.         
A = { 1, 2, 3, 4, 5 }     
R = {     
    (0, 0), (0, 4), (4, 0),     
    (1, 1), (1, 3), (3, 1), (1, 5), (5, 1),      
    (2, 2), (2, 4), (4, 2),      
    (3, 3),     
    (5, 5)                
}     


.5. 
A = { 0, 1, 2, 3, 4, 5 }      
R = { (1, 2), (2, 5), (3, 3), (4, 3), (4, 2), (5, 0) }



.6. Congruence modulo5 is a relation on the set A = Z. In this relation xRy means x ≡ y(mod5). Write out the set R in set-builder notation.      
R = { (x, y) in Z : 5 | x - y }       



.7. Write the relation < on the set A = Z as a subset R of Z x Z. This is an infinite set, so you will have to use set-builder notation.      
R = { (x, y) in Z x Z : y - x in N } set_in Z x Z.      


.9. Let A = { 1, 2, 3, 4, 5, 6 }. How many different relations are there on the set A ?       
There are 2^|A| = 2^6 subsets of A.      
There are 36 ordered pairs in A.       
So 2^36 many different relations.     

.10. Consider the subset R = (R x R) - { (x,x) : x in R } set_in R x R. What familiar relation onRis this? Explain.        
(R x R) is 2D plane, { (x,x) : x in R } is an equal coordinates.     
Remove all equal coordinates from 2D plane, you get all non-equal coordinates.          


.11. Given a finite set A, how many different relations are there on A ?     
There are 2^|A| subsets of A.      
There are |A| * |A| = |A|^2 ordered pairs in A.       
So 2^(|A|^2) many different relations.     

In the following exercises, R of R^2 = R x R or Z^2 = Z x Z indicated by gray shading. In each case, R is a familiar relation on R or Z. State it.      
.12.     




11.2 Properties of Relations
Definition 11.2 Suppose R is a relation on a set A.     

.1. Relation R is reflexive if xRx for every x in A.     
That is, R is reflexive if all x in A, xRx.     

.2. Relation R is symmetric if xRy implies yRx for all x,y in A.    
That is, R is symmetric if all x, y in A, xRy => yRx.       

.3. Relation R is transitive if whenever xRy and yRz, then also xRz.     
That is, R is transitive if for all x, y, z in A, ((xRy) ^ (yRz)) => xRz.     


Example 11.7. A = { b, c, d, e }, and R is the following relation on A: R { (b, b), (b, c), (c, b), (c, c), (d, d), (b, d), (d, b), (c, d), (d, c) }.      
.1. It's not reflexive, because it's not true that eRe. (should be true for all x in A).      
.2. It's symmetric, whenever we have xRy, it follows yRx too.      
.3. It's transitive.     


Example 11.8 Prove the following proposition.     
Proposition. Let n in N. The relation ≡ (mod n) on the set Z is reflexive, symmetric and transitive.     
1) Show that it's reflexive.     
For all integers in Z it's true that n | 0.     
n | (x - x), which is x ≡ x (mod n) by definition.     
So it's reflexive.     
2) Show that it's symmetric.      
For all x, y in Z it must be true that if x ≡ y (mod n) then y ≡ x (mod n).     
Suppose x ≡ y (mod n). Then n | (x - y).     
Then x - y = na for some a.      
Multiply by (-1) both sides, y - x = n(-a).     
Then n | (y - x), y ≡ x (mod n).     
3) Show that it's transitive.     
Show that if x ≡ y (mod n) and y ≡ z (mod n), then x ≡ z (mod n).      
n | (x - y) and n | (y - z), then x - y = na, y - z = nb.      
x - y + y - z = na + nb.     
x - z = n(a + b).     
n | (x - z).     
x ≡ z (mod n).     



Exercises for Section 11.2     

.1.Consider the relation R = { (a,a), (b,b), (c,c), (d,d), (a,b), (b,a) } on set A = { a, b, c, d }. Is R reflexive? Symmetric? Transitive? If a property does not hold, say why.       
1) R is reflexive, it's true that for all x in R, xRx.      
2) R is symmetric, for all x, y it's true that xRy => yRx.      
3) ?

.2. Consider the relation R = { (a,b), (a,c), (c,c), (b,b), (c,b), (b,c) } on the set A = { a, b, c }. Is R reflexive? Symmetric? Transitive? If a property does not hold, say why.     
1) R is not reflexive, it's not true that aRa.     
2) R is not symmetric, it's not true that bRa.     


.3. Consider the relation R = { (a,b), (a,c), (c,b), (b,c) } on the set A = { a, b, c }. Is R reflexive? Symmetric? Transitive? If a property does not hold, say why.      
1) R is not reflexive, it's not true that xRx for all x in R.      
2) R is not symmetric, it's not true that f.e. aRb => bRa.      
3) R is transitive.     


.4. Let A = { a, b, c, d }. Suppose R is the relation    
R = { (a,a), (b,b), (c,c), (d,d),     
      (a,b), (b,a), (a,c), (c,a),     
      (a,d), (d,a), (b,c), (c,b),     
      (b,d), (d,b), (c,d), (d,c) 
    }.      
Is R reflexive? Symmetric? Transitive? If a property does not hold, say why.      
1) R is reflexive.     
2) R is symmetric.     
3) R is transitive (?).      


.5. Consider the relation R = { (0, 0), (sqrt(2), 0), (0, sqrt(2)), (sqrt(2), sqrt(2)) } on R. Is R reflexive? Symmetric? Transitive? If a property does not hold, say why.      
1) R is reflexive.     
2) R is symmetric.      
?

.6. Consider the relation R = { (x,x) : x in Z } on Z. Is this R reflexive? Symmetric? Transitive? If a property does not hold, say why. What familiar relation is this?      
1) R is reflexive.     
2) R is symmetric.     
3) R is transitive.     
This relation is 2D plain.      (?)

.7. There are 16 possible different relations R on the set A = { a, b }. Describe all ofthem. (A picture for each one will suffice, but don't forget to label the nodes.) Which ones are reflexive? Symmetric? Transitive?     


.8. Define a relation on Z as xRy if |x−y| < 1. Is R reflexive? Symmetric? Transitive? If a property does not hold, say why. What familiar relation is this?      
R = { (x, y) in Z x Z : |x - y| < 1 }     
1) R is reflexive, |x - x| < 1 for all x in R.     
???


.9. Define a relation on Z by declaring xRy if and only if x and y have the same parity. Is R reflexive? Symmetric? Transitive? If a property does not hold, say why. What familiar relation is this?     
1) R is reflexive, xRx for all x in R since x have the same parity.     
2) R is symmetric, xRy => yRx, x and y have the same parity.     
3) R is transitive, if xRy and xRz, then xRz.     


.10. Suppose A != empty_set. Since empty_set set_in A x A, the set R = empty_set is a relation on A. Is R reflexive? Symmetric? Transitive? If a property does not hold, say why.       
1) R is not reflexive, it's not true that for all x in A, xRx. (?)     
2) R is symmetric.     
3) R is transitive.     


.11. Let A = { a, b, c, d } and R = { (a,a), (b,b), (c,c), (d,d) }. Is R reflexive? Symmetric? Transitive? If a property does not hold, say why.      
1) R is reflexive.      
2) R is symmetric, there are no such x, y for which (y, x) not in R if (x, y) in R.     
3) R is transitive, f.e. (aRa ^ aRa) => aRa.            

.12. Prove that the relation | (divides) on the set Z is reflexive and transitive.     
1) Show that | is reflexive.     
For any integer x in Z, it's true that x | x.      
2) Show that | is transitive.     
We must show that if x | y and y | z then x | z.     
Direct proof. Suppose that x | y and y | z, then y = x * a (for some a in Z) and z = y * b (for some b in Z).     
Then z = x * a * b = x (ab).     
By definition x | z.      

.13. Consider the relation R = { (x, y) in R x R : x - y  in Z } on R. Prove that this relation is reflexive, symmetric and transitive.      
1) Show that R is reflexive.     
For any (x, x) in R it's true that x - x in Z.     
2) Show that R is symmetric.     
If x - y in Z, then -(x - y) in Z, but -(x - y) = y - x.     
Which means xRy => yRx for all x, y in R.      
3) Show that R is transitive.     
Show that if x - y in Z and y - z in Z, then x - z in Z.     
Suppose x - y in Z and y - z in Z, then      
x - y = a, y - z = b for some a, b in Z,     
x - b - z = a, x - z = a + b, a + b in Z.     

.14. Suppose R is a symmetric and transitive relation on a set A, and there is an element a in A for which aRx for every x in A. Prove that R is reflexive.      
Since R is symmetric it follows that aRx => xRa.     
R is also transitive, so aRx ^ xRa => aRa.    

.15. Prove or disprove: If a relation is symmetric and transitive, then it is also reflexive.     
It's false (see Example 11.7, page 180).    
Disprove by counterexample.     
Consider A = { b, c, d }, and R is the following relation on A:     
R = { (b, b), (b, c), (c, b), (c, c), (b, d), (d, b), (c, d), (d, c) }      
R is symmetric, whenever we have xRy, it follows that yRx.     
R is transitive, but not reflexive, it's not true that dRd.      

.16. Define a relation R on Z by declaring that xRy if and only if x^2 === y^2(mod 4). Prove that R is reflexive, symmetric and transitive.     
R = { (x, y) in Z x Z : 4 | x^2 - y^2 }.     
Prove that R is reflexive.     
Observe that 4 | 0, so 4 | (x^2 - x^2) => x^2 === x^2 (mod 4).     
Prove that R is symmetric.     
Suppose x^2 === y^2 (mod 4), then by definition 4 | x^2 - y^2, then x^2 - y^2 = 4a, for some a in Z.     
Multiply by -1 we get y^2 - x^2 = 4(-a).     
Then 4 | y^2 - x^2 => y^2 === x^2 (mod 4).     
Prove that R is transitive.     
Suppose that 4 | x^2 - y^2 and 4 | y^2 - z^2.     
x^2 - y^2 = 4a, y^2 - z^2 = 4b.     
Add those two together we get x^2 - y^2 + y^2 - z^2 = 4a + 4b.     
x^2 - z^2 = 4(ab) => 4 | x^2 - z^2 => x^2 === z^2 (mod 4).     


.17. Modifying the above Exercise 8 (above) slightly, define a relation ~ on Z as x ∼ y if and only if |x-y|<=1. Say whether ∼ is reflexive. Is it symmetric? Transitive?
1) R is reflexive, |x - x| < 1 for all x in R.     
???


11.3 Equivalence Relations.     

Definition 11.3 A relation R is called equivalence relation on a set A if it's reflexive, symmetric and transitive.     


Definition 11.4 Suppose R is an equivalence relation on a set A. Given any element a, an equivalence class containing a is a subset of A [a] = { x in A : xRa }.     


R_1 = { (-1, -1), (1, 1), (2, 2), (3, 3), (4, 4) }

Example 11.9 Consider relation R_1 (equal to, "="), the equivalence class containing 2 is [2] = { x in A : x(R_1)2 } = { 2 }.     


Exercises for Section 11.3.      

.1. Let A = { 1, 2, 3, 4, 5, 6 }, and consider the following equivalence relation on A: R = { (1, 1), (2, 2), (3, 3), (4, 4), (5, 5), (6, 6), (2, 3), (3, 2), (4, 5), (5, 4), (4, 6), (6, 4), (5, 6), (6, 5) }. List the equivalence classes of R.     
[1] = { x in A : xR1 } = { 1 }     
[2] = { x in A : xR2 } = { 2, 3 }     
[3] = { x in A : xR3 } = { 3, 2 }     
[4] = { x in A : xR4 } = { 4, 5, 6 }     
[5] = { x in A : xR5 } = { 5, 4, 6 }     
[6] = { x in A : xR6 } = { 6, 4, 5 }     
{ 1 }, { 2, 3 }, { 4, 5, 6 }     
There are 3 equivalence classes.     


.2. Let A = { a, b, c, d, e }. Suppose R is an equivalence relation on A. Suppose R has two equivalence classes. Also aRd, bRc and eRd. Write out R as a set.     
If aRd,bRc and eRd, then R contains (a, d), (b, c), (e, d).     
R is symmetric, so R contains (d, a), (c, b), (d, e).     
R is reflexive, R contains (a, a), (b, b), (c, c), (d, d), (e, e).     
aRd and eRd means there should be (a, e), (e, a)
R has two equivalence classes, they are:     
[a] = { a, d, e }.     
[b] = { c, b }.     
[c] = { b, c }.     
[d] = { a, d, e }.     
[e] = { d, e, a }.     
[a] = [d] = [e], [b] = [c].         
R = { (a, d), (b, c), (e, d), (d, a), (c, b), (d, e), (a, a), (b, b), (c, c), (d, d), (e, e), (a, e), (e, a) }
Solution_2.      
aRd and eRd means that a, e, d in the same equivalence class.     
bRc means b, c in the same equivalence class.     
There are two equivalence classes - { a, e, d }, { b, c }.          
For R to be an equivalence relation, it needs to include all possible pairs of elements in the same equivalence class and no others (!!!).     


.3. Let A = { a, b, c, d, e }. Suppose R is an equivalence relation on A. Suppose R has three equivalence classes. Also aRd and bRc. Write out R as a set.      
If aRd, bRc, then R contains (a, d), (b, c).     
R is symmetric, R contains (d, a), (c, b).     
R is reflexive, R contains (a, a), (b, b), (c, c), (d, d), (e, e).     
R has three equivalence classes:
[a] = { d, a }.      
[b] = { c, b }.     
[c] = { b, c }.     
[d] = { c, b }.     
[e] = { e }.     
[a] = [d], [b] = [c], [e] - three classes.     
R = { (a, d), (b, c), (d, a), (c, b), (a, a), (b, b), (c, c), (d, d), (e, e) }     

.4.Let A = { a, b, c, d, e }. Suppose R is an equivalence relation on A. Suppose also that aRd and bRc, eRa and cRe. How many equivalence classes does R have?      
aRd => a, and d in the same equivalence class, [a] = [d]     
bRc => [b] = [c]     
eRa => [e] = [a]     
cRe => [c] = [e]     
[a] = [d] = [e] = [c] = [b].     
There is one equivalence class.     
