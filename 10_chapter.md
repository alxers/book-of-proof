Mathematical Induction.     

Outline for Proof by Induction.     
Proposition The statements S_1, S_2, S_3, ... are all true.     

Proof. (Induction)     
(1) Prove that the first statement S_1 is true.     
(2) Given any integer k >= 1, prove that the statement S_k => S_k+1 is true.     
It follows by mathematical induction that every S_n is true.     


Example:     
Proposition. If n in N, then 1+3+5+7+...+(2n-1) = n^2.     
Proof.     
(1) Observe that if n = 1, this statement is 1 = 1^2, which is true.     
(2) We must prove S_k => S_k+1 for any k >= 1.     
That is if 1+3+5+7+...+(2k - 1) = k^2, then 1+3+5+7+...+(2(k+1) - 1) = (k + 1)^2.     
Direct proof. Suppose 1+3+5+7+...+(2k - 1) = k^2.     
Then 1 + 3 + 5 + 7 + ... + (2 (k + 1) - 1) =       
1 + 3 + 5 + 7 + ... + (2k - 1) + (2 (k + 1) - 1) =     
(1 + 3 + 5 + 7 + ... + (2k - 1)) + (2 (k + 1) - 1) =      
k^2 + (2 (k + 1) - 1) = k^2 + 2k + 1 = (k + 1)^2      
This proves that S_k => S_k+1.     
It follows by induction that 1 + 3 + 5 + 7 + ... + (2n - 1) = n^2 for every n in N.     


Proposition If n is a non-negative integer, then 5 | (n^2 - n).     
(1) If n = 0, 0 = 5x.    
(2) Let k >= 0, we need to prove that if 5 | (k^5 - k), then 5 | ((k+1)^5 - (k+1)).     
k^5 - k = 5x.     
(k + 1)^5 - (k + 1) = k^5 + 5k^4 + 10k^3 + 10k^2 + 5k + 1 - k - 1 =      
= (k^5 - k) + 5(k^4 + 2k^3 + 2k^2 + k) =       
= 5x + 5(...) = 5(x + ...).     
It follows by induction that 5 | (n^5 - n) for all non-negative integers n.     


Proposition For each n in N, it follows that 2^n <= 2^(n+1) - 2^(n-1) - 1.     
(1) If n = 1, then 2 <= 4 - 1 - 1      
(2) Suppose k >= 1. We need to show that 2^k <= 2^(k+1) - 2^(k-1) - 1 implies 2^(k+1) <= 2^(k+2) - 2^k - 1      
2^k <= 2^(k+1) - 2^(k-1) - 1.     
Multiply both sides by 2.     
2^(k+1) <= 2^(k+2) - 2^k - 2.      
Add 1 to the right side (it doesn't change inequation).      
2^(k+1) <= 2^(k+2) - 2^k - 1.     
It follows by induction that 2^n <= 2^(n+1) - 2^(n-1) - 1 for each n in N.     
