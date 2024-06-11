
# Calculating NOD of a number in $O(n^{1/3})$
To find NOD(N), first we wrtie N as a product of two number X*Y. Here all the prime factors of x are less than equal $n^{1/3}$. Therefore, rest of the prime factors are in Y; Hence the GCD(X,Y) = 1. 

We can easily proof that $NOD(X * Y) = NOD(X) * NOD(Y)$ when gcd(x,y) = 1

## calculating NOD of X
We can calculate the NOD(X) using the nieve prime factorisation of N up to the primes under $N^{1/3}$ 

if $X = {p_1}^{n_1}*{p_2}^{n_2}{p_3}^{n_3}...$

Then $NOD(X) = ({n_1+1})*({n_2+1})*({n_3+1})....$

## calculating NOD of Y
Now in case of Y, as all the prime factors are greater than $N^{1/3}$ so Y is at most multiple of two prime numbers.
So we can see there are only four cases which will cover all the possibilities.
* if Y is 1 NOD = 1
* if Y in a prime NOD(Y) = 2;
* if Y is square of a prime NOD(Y) = 3
* if Y is multiple of two primes NOD(Y) = 4

For primality test we will use efficient Miller Rabin primality test algorith

[code in C++](https://github.com/srlabib/Competitve-programming-equipments/blob/main/Number%20Theory/Optimized_NOD.cpp) 
