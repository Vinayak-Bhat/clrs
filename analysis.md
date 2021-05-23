---
page: true
---
{% include mathjax.html %}

## Analysis of Algorithms

Before we start exploring different algorithms, we need a toolset to assess the algorithms we come across.
After we know that an algorithm is correct (gives correct output for the inputs of interest), we assess the algorithm on two counts:
1) running time of the algorithm
2) memory requirements of the algorithm
For example, of the two algorithms that correctly work out a problem at hand, the one which takes less running time (or memory) for the same input, is said to be better.

Also we are mainly concerned with how the performance time increases(or memory usage) with the increase in input size.
And that brings us to asymptotic notation.
Asymptotic analysis is about analyzing runtime when input size is in the limit. Or tends to infinity.
 
Why the focus on aysmptotic analysis?
If an algorithm performs well in aysmptotic analysis, it will be good enough for all but few inputs.
Also it saves us from calculating the exact performance numbers but yet is detailed enough a metric to compare algorithms for various inputs.


There are five asymptotic notations that are used.

### O() - big O notation which is the most common.

An algorithm is said to run in $$O(g(n))$$ time, when there exists a positive constant c, for some positive $$ n_0 $$, such that:
$$ f(n) \le c * g(n) $$ for all $$ n  \ge n_0 $$.
where $$f(n) $$ is the function representing the runtime of the algorithm.

example 
$$ f(n) = an^2 + bn +c $$ is $$ O(n^2) $$

It means the running time of algorithm is always less than or equal to $$g(n)$$ for a sufficiently large n.

### $$\Theta()$$ - Theta notation 

An algorithm is said to run in $$ \Omega(g(n)) $$ time, when there exist positive constants $$ c_1 , c_2 $$, for some positive $$ n_0 $$, such that:
$$ c_1 * g(n) \le f(n) \ge c_2 * g(n) $$ for all $$ n \ge n_0 $$
where $$ f(n) $$ is the function representing the runtime of the algorithm.

### $$\Omega()$$ - Omega notation

An algorithm is said to run in $$\Delta(g(n))$$ time, when there exists a positive constant c, for some positive $$ n_0 $$, such that:
$$ f(n) \ge c * g(n) $$ for all $$ n  \ge n_0 $$.
where $$f(n) $$ is the function representing the runtime of the algorithm.

### $$\delta()$$ - Small o notation

An algorithm is said to run in $$o(g(n))$$ time, there exists a positive $$ n_0 $$, such that:
$$ f(n) \lt c * g(n) $$ for all $$ n  \ge n_0 $$ and for any positive constant c
where $$f(n) $$ is the function representing the runtime of the algorithm.

### $$\omega()$$ - Small omega notation

An algorithm is said to run in $$\delta(g(n))$$ time, for a positive constant $$c_0$$ there exists a positive $$ n_0 $$, such that:
$$ f(n) \gt c_0 * g(n) $$ for all $$ n  \ge n_0 $$.
where $$f(n) $$ is the function representing the runtime of the algorithm.


