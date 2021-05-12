---
page: true
---
{% include mathjax.html %}

## Analysis of Algorithms

Analysis of algorithms has two considerations:
1) analysis to evaluate the running time of algorithms
2) analysis to evaluate the memory requirements during algorithm runs

Also we are mainly concerned with how the performance time increases(or memory usage) with the increase in input size.
And that brings us to asymptotic notation.
Asymptotic analysis is about analyzing runtime when input size is in the limit. Or tends to infinity.
 
Why the focus on aysmptotic analysis?
If an algorithm performs well in aysmptotic analysis, it will be good enough for all but few inputs.
Also it saves us from calculating the exact performance numbers but yet is detailed enough a metric to compare algorithms for various inputs.


There are five asymptotic notations that are used.

### O() - big O notation which is the most common.

An algorithm is said to run in $$O(g(n))$$ time, when there exists a positive constant c, for some positive $$ n{0} $$, such that:
$$ f(n) \le c * g(n) $$ for all $$ n  \ge n{0}$$.
where $$f(n) $$ is the function representing the runtime of the algorithm.

example 
$$ f(n) = an^2 + bn +c $$ is $$ O(n^2) $$

It means the running time of algorithm is always less than or equal to $$g(n)$$ for a sufficiently large n.

### $$\Omega()$$ - Omega notation 

An algorithm is said to run in $$ \Omega(g(n))$$ time, when there exist positive constants $$c{1} $$ $$c{2}$$, for some positive $$ n{0} $$, such that:
$$ c{1] * g(n) \ge f(n) \le c{2} * g(n)$$ for all $$ n \ge n{0} $$
where $$ f(n) $$ is the function representing the runtime of the algorithm.




