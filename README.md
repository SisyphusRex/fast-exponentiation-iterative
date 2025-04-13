# fast-exponentiation-iterative
Implementation of Fast Exponentiation using Iteration Algorithm.

## What is
Computing $`x^{y}`$ can take an impractical amount of time.  

We can reduce the time to calculate an exponent by using binary expansion.  

$`x^{y} = x^{a_{k}2^{k} + a_{k-1}2^{k-1}+...+a_{1}2^{1}+a_{0}2^{0}}=x^{a_{k}2^{k}}*x^{a_{k-1}2^{k-1}}*...*x^{a_{1}2^{1}}*x^{a_{0}2^{0}}`$  

Remember, $`x^{a+b}=x^{a}*x^{b}`$.  Also, each coefficient $`a_{j}`$ is 0 or 1.  

For example, take $`7^{11}`$.  The binary expansion of $`11=(1011)_{2}`$.   
$`7^{11}=7^{(1*2^{3})+(0*2^{2})+(1*2^{1})+(1*2^{0})}=7^{8}*7^{2}*7^{1}`$  

## Pseudocode
Input: positive integers x and y  
Output: $`x^{y}`$  

p=1 //partial result  
s=x //current $`x^{2^{j}}`$  
r=y // used to compute binary expansion of y

