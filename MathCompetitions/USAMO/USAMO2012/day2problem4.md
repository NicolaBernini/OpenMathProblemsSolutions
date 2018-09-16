

# Overview 

Some USAMO Problems [here](https://artofproblemsolving.com/wiki/index.php?title=USAMO_Problems_and_Solutions)

## USAMO 2012 - Day 2 - P 4

Reference [here](https://artofproblemsolving.com/wiki/index.php?title=2012_USAMO_Problems)


### Observations 

- First let's observe that $f(n!)=f(n)! \quad n \in \mathbb{Z}^{+}$ means that $f(\cdot)$ needs to be invariant to factorial as we want the factorial applied to the transformation input or output leads to the same result 
- So let's explore if something simple like a linear transformation has this property 
  - let's take $g(n) = a + bn \quad a,b \in \mathbb{Z}^{+}$ to start and see that in general, hence $\forall a,b$ it is 


$$ a + bn! \neq (a + bn)! $$

- Let's explore the 2 restrictions hence 1) $a=0$ and 2) $b=0$

- So in 1) case in general 

$$ bn! \neq (bn)! $$

but there is one specific case in which the scale factor does not affect the factorial which is $b=1$ hence finally we observe the linear transformation $g(n;a,b)$ with the $\theta_{0}=\{a=0, b=1\}$ parametrization, which makes it an identity transformation essentially, is candidate for the solution 

- In case 2) we easily observe the shift $a$ always affect the factorial but in the case $a=0$ hence we get again to the identity transformation 

Furthermore it is required $c = m-n$ divides $d = f(m) - f(n)$ in $\forall m,n \in \mathbb{Z}^{+}$ (assuming also $m>n$) and it's easy to verify identity gives $d = I(m) - I(n) = m - n = c$ and $c$ divives itself 

Hence $I(n)=n$ is a valid solution 

**Is this the only valid solution ?**

It has been found a solution depending on $n$ but we could explore solutions not depending on it hence mapping $\forall n$ to a constant $k$ : $g(n)=k$

It essentially consists of solving the equation 

$$ k = k! $$

which it is known to be solved by $k=\{1,2\}$


# Solution 

1) $f(n)=n$
2) $f(n)=1$
3) $f(n)=2$











