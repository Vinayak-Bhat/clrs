---
page: true
---
{% include mathjax.html %}

## Analysis of Algorithms

Before we start exploring different algorithms, we need a toolset to assess the algorithms we come across.
After we know that an algorithm is correct (gives correct output for the inputs of interest), we assess the algorithm on two counts:
1) running time of the algorithm
2) memory requirements of the algorithm.
For example, of the two algorithms that correctly work out a problem at hand, the one which takes less running time (or memory) for the same input, is better.

Also we are mainly concerned with how the performance time increases(or memory usage) with the increase in input size.
And that brings us to asymptotic efficiency of algorithms.
Asymptotic analysis is about analyzing runtime when input size is in the limit. Or tends to infinity.
 
Why the focus on aysmptotic efficiency?
If an algorithm performs well in aysmptotic analysis, it will be good enough for all but few inputs.
Also it saves us from calculating the exact performance numbers but yet is detailed enough a metric to compare algorithms for various inputs.


There are five asymptotic notations in use:

### O() - "big Oh" notation

An algorithm is said to run in $$O(g(n))$$ time, when there exists a positive constant c, for some positive $$ n_0 $$, such that:
$$ 0 \le f(n) \le c * g(n) $$ for all $$ n  \ge n_0 $$.
where $$f(n) $$ is the function representing the runtime of the algorithm.

Examples:
* An algorithm, whose running time is reqpresented by function $$f(n) = an^2 + bn +c $$ is said to be  $$ O(n^2) $$
* $$f(n) = an+ b$$ then $$ f(n) = O(n)$$
* $$f(n) = a_1 $$ then $$f(n) = O(1) $$.  Here, function here is constant and does not increase with input. This represents an algorithm that takes constant time $$a_1$$ to run. Also note that the  $$O(1)$$ is easy representation for $$O(n^0)$$. $$O(1)$$ does not indicate the variable that is increasing asymptotically.

When we say a function $$f(n) = O(g(n))$$, it is meant that $$f(n)$$, belongs to a set of functions reprensented by $$O(g(n))$$.
The equality is commonly used instead of the more accurate belonging to a set. This is true for other asymptotic notations below as wel.

### $$\Theta()$$ - Theta notation 

An algorithm is said to run in $$ \Theta(g(n)) $$ time, when there exist positive constants $$ c_1 , c_2 $$, for some positive $$ n_0 $$, such that:
$$ 0 \le c_1 * g(n) \le f(n) \le c_2 * g(n) $$ for all $$ n \ge n_0 $$
where $$ f(n) $$ is the function representing the runtime of the algorithm.

### $$\Omega()$$ - Omega notation

An algorithm is said to run in $$\Omega(g(n))$$ time, when there exists a positive constant c, for some positive $$ n_0 $$, such that:
$$ 0 \le  c * g(n) \le f(n) $$ for all $$ n  \ge n_0 $$.
where $$f(n) $$ is the function representing the runtime of the algorithm.

### $$o()$$ - Small o notation

An algorithm is said to run in $$o(g(n))$$ time, there exists a positive $$ n_0 $$, such that:
$$ 0 \le f(n) \lt c * g(n) $$ for all $$ n  \ge n_0 $$ and for any positive constant c
where $$f(n) $$ is the function representing the runtime of the algorithm.

### $$\omega()$$ - Small omega notation

An algorithm is said to run in $$\omega(g(n))$$ time, there exists a positive $$ n_0 $$, such that:
$$ 0 \le c * g(n) \lt f(n) $$ for all $$ n  \ge n_0 $$ and for any positive constant c
where $$f(n) $$ is the function representing the runtime of the algorithm.


Note that all the asymptotic notations work on the set of natural numbers. And the functions $$g(n)$$ and $$f(n)$$ are asymptotically nonnegative.

