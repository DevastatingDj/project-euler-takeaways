# project-euler-takeaways
Takeaways from the first 75 problems of Project Euler (Target is yet to be achieved)

## Problem 1
Find the sum of all the multiples of 3 or 5 below 1000.

Sum of numbers 1-n = n*(n+1)/2

## Problem 2
By considering the terms in the Fibonacci sequence whose values do not exceed four million, find the sum of the even-valued terms.

2 8 34 144...
it seems that they obey the following recursive relation

F(n)=4*F(n-3)+F(n-6)

## Problem 3
Find the largest prime factor of a composite number

Let the given number be n and let k = 2, 3, 4, 5, ... . For each k, if it is a factor of n then we
divide n by k and completely divide out each k before moving to the next k. It can be seen that
when k is a factor it will necessarily be prime, as all smaller factors have been removed, and
the final result of this process will be n = 1.

## Problem 4
Find the largest palindrome made from the product of two 3-digit
numbers.

Consider the digits
of P – let them be x, y and z. P must be at least 6 digits long since the
palindrome 111111 = 143×777 – the product of two 3-digit integers. Since P is
palindromic:
P=100000x10000y1000z100z10yx
P=100001x10010y1100z
P=119091x910y100z
Since 11 is prime, at least one of the integers a or b must have a factor of 11.
So if a is not divisible by 11 then we know b must be

## Problem 5
What is the smallest number divisible by each of the numbers 1 to 20? 

The smallest number n that is evenly divisible by every number in a set {k1, k2, ..., k_m}
is also known as the lowest common multiple (LCM) of the set of numbers.
The LCM of two natural numbers x and y is given by LCM(x, y) = x * y / GCD(x, y).
When LCM is applied to a collection of numbers, it is commutative, associative, and idempotent.
Hence LCM(k1, k2, ..., k_m) = LCM(...(LCM(LCM(k1, k2), k3)...), k_m).
