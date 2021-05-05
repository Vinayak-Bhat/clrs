---
page: true
---
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

O() - big O notation which is the most common.

An algorithm is said to run in O(g(n)) time, when the running time f(n) is such that f(n) is less than c * g(n) for all n greater than some positive n0 and positive constant c.
example $$ f(n) = an^2 + bn +c $$ is O(n2) 

