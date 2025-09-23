---
layout: default
title: "The Fibonacci Toolbox"
tags: [ "maths" ]
---

These are some facts and theorems on fibonacci numbers that are often useful for various problems.

Wiki Link: [Fibonacci Number](https://en.wikipedia.org/wiki/Fibonacci_number)

----

# Definitions

Fibonacci Sequence : A sequence of integers $F_0, F_1, \cdots$ such that $F_{n} = F_{n-1} + F_{n - 2}$ for all $n \geqslant 1$, with, $F_0 = 0$ and $F_1 = 1$. 

Lucas Sequence: $L_n = F_{n-1} + F_{n + 1}$

Golden Ratio: $\phi =	\frac{1+\sqrt{5}}{2}$

Binet's Formula:

$$F_{n}=\frac{1}{\sqrt{5}}\left(\frac{\sqrt{5}+1}{2}\right)^{n}-\frac{(-1)^{n}}{\sqrt{5}}\left(\frac{\sqrt{5}-1}{2}\right)^{n}$$

for $n \geq 0$.
---

# Properties


1. (Strong Divisibility) $$\operatorname{gcd}(F_n,F_m)= F_{\operatorname{gcd}(n,m)}$$
   (GCD Rule) $$\operatorname{gcd}\left(F_{n}, F_{n-1}\right)=1$$
2. (Divisibility Sequence) $$m \mid n \implies F_m \mid F_n$$
3. (Cassini's Identity) $$F_{n-1}F_{n+1} - {F_n}^2 = (-1)^n$$
4. (Matrix Power Form) $$
\begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix}^n =
\begin{pmatrix} F_{n+1} & F_n \\ F_n & F_{n-1} \end{pmatrix}
$$
5. (Parity) If $F_n$ is even if and only if $n$ is divisible by $3$
6. (Lucas Identity) $$F_n^2+F_{n+1}^2 = F_{2n+1}  $$
7. (Fibonacci Generating Function) $$\sum_{n=1}^{\infty} F_{n} x^{n}=\frac{x}{1-x-x^{2}}$$
8. (Finite Sum) $$F_1 + F_2 + F_3 + F_4 + \cdots + F_n = F_{n+2} - 1$$
9. (Balls and Urns Formulation) $$F_n=\sum\limits_{k=0}^{n-1} \binom{n-k-1}{k} \text{ or, } 	\sum\limits_{k=1}^{n}\binom{n-k}{k-1} $$ 
10. (Fibonacci Limit Theorem) $$\lim\limits_{n \to \infty} \frac{F_{n+1}}{F_n} = \phi$$ 
11. (Gap Telescope) $$\frac 1{F_{n-1}F_{n+1}}=\frac 1{F_{n-1}F_n}-\frac 1{F_nF_{n+1}}$$
12. (Difference Rule) $$F_nF_{n+1}=F_n^2+F_{n-1}F_n$$
13. (Square Sum) $$\sum_{k=1}^{n}F_{k}^{2}=F_{n}F_{n+1}$$
14. (Double Sum)$$F_{m}F_{n+1} + F_{m-1}F_{n} = F_{n+m}$$
15. (Triple Sum) $$F_a F_{a+b+c}-F_{a+b}F_{a+c}=(-1)^{a+1} F_b F_c$$
16. (First Form Inequality) $$F_k > F_{k-2}+F_{k-3}+\ldots+F_2$$
17. (Sum of the First $n$ Odd-Indexed) $$\sum_{i=1}^n F_{2i-1} = F_{2n}$$
18. (Sum of the First $n$ Even-Indexed) $$\sum_{i=1}^n F_{2i} = F_{2n+1} - 1$$
18. (Gelin-Cesàro Identity) $$F_{n}^{4}-F_{n-2} F_{n-1} F_{n+1} F_{n+2}=1, \quad n \geq 3$$  

--- 

# Fact File

Fact 1: The only Fibonacci numbers that are squares are $0, 1, 144.$ 

// Proof: https://math.la.asu.edu/~checkman/SquareFibonacci.html#intro

Fact 2: Every positive integer $m$, there is a Fibonacci number divisible by $m$.

// Proof: https://math.stackexchange.com/questions/1523198/proving-that-every-integer-has-a-fibonacci-number-multiple (also see, https://artofproblemsolving.com/community/c6h2231614p17047441)

Fact 3: A number x is fibonacci if $5x^2 \pm 4$ is a square. Another way to test if a number is fibonacci is to invert binet's formula.

Fact 4: $G_n$: The ratio of two successive term in the Fibonacci Sequence, i.e, $\displaystyle G_n = \frac{F_{n+1}}{F_n}$

---

# Theorems

* Theorem[Zeckendorf]: Every positive integer can be represented `uniquely` as the sum of one or more Fibonacci numbers in such a way that the sum does not include any two consecutive Fibonacci numbers.

* Theorem[Counting]: 

   + $F_{n}$ is the number of binary sequences of length $n-2$ with no consecutive 0 s.
   + $F_{n}$ is the number of subsets of ${1,2, \ldots, n-2}$ that do not contain any pair of consecutive numbers.

*  Theorem: All the odd divisors of Fibonacci numbers with odd subscripts are of
the form $4t + 1$

 * Theorem: Let $r \in \mathbb{N}$. The Fibonacci numbers modulo $r$ form a periodic sequence.
---
