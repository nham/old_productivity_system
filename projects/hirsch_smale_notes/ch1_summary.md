## A first example

One of the simplest class of differential equations is

$$x'(t) = ax(t)$$

holding for all $t \in U$.

$x$ must be some function $U \to \mathbb{R}$ where $U$ is some open subset, presumably. 

(we could also say $Dx = ax$)

They just say "real-valued function of a real variable", but it's some set that must have a derivative everywhere I am assuming.


## Characterizing $x' = ax$
All solutions $x$ to this diff. eq must have the form:

$$x(t) = Ke^t$$

for some $K \in \mathbb{R}$.


One proof of this starts by considering $D[u(t) e^{-at}]$, proves that that derivative is $0$, so therefore $u(t) e^{-at}$ is constant and there must be some $M \in \mathbb{R}$ such that $M = u(t) e^{-at}$ for all $t$. So 

$u(t) e^{-at} e^{at} = M e^{at}$

and therefore $u(t) = M e^{at}$ for any solution $u$.

## What are the values?

Note that if $x(0)$ is known for a particular solution $x$, then the rest of the values are known as well since $x(0) = K$.

Can we say the same for all $b \neq 0$? That is, if we know $x(b)$, can we get $K$?

Yes. H&S do this:

First we define $\sigma_C$ as a map that takes solutions $x$ and is defined by

$$ x \mapsto (t \mapsto x(t - C)$$

($\sigma_C$ takes any solution $x$ and moves the time forward by $C$ units)

Then $(\sigma_{-b} x)$ is such that  $(\sigma_{-b} x)(0) = x(b)$. In other words,

$$(\sigma_{-b} x)(t) = x(b) e^{at}$$

for all $t$.

We now consider two ways to look at $[\sigma_b (\sigma_{-b} x)](t)$. By definition this is $x(t + b - b) = x(t)$, since $(\sigma_{-b} x) : t \mapsto x(t + b)$. So we have that $x = \sigma_b (\sigma_{-b} x)$.

On the other hand, from the above we know $(\sigma_{-b} x)(t) = x(b) e^{at}$, so since

$$\sigma_C: x -> e^{-aC} x$$

for all $C$, we have that

$$[\sigma_b (\sigma_{-b} x)] (t) = e^{-ab} x(b) e^{at}$$

This proves that $x(t) = e^{-ab} x(b) e^{at}$ for all $t$, giving us the rest of the values.

If $x$ is a solution and $x(b)$ is known for some $b \neq 0$, then defining $y(t) := x(t - b)$. Then $y(b) = x(0) = K$. This means

Define $\phi_C x: t \mapsto x(t - C)$. Then $[\phi_{-b} x](t) = x(t + b)$, so $[\phi_{-b} x](0) = x(b)$. We know (from the above) that $[\phi_{-b} x](t) = x(b) e^{at}$, so 

$$x(t) = x((t - b) + b) = \phi_b[\phi_{-b} x](t)$, and that

$\phi_b[x(b) e^{at}] (t) = x(b) e^{-ab} e^{at} = x(t)$. This proves that given the state of the system at any time, we can determine the rest.

## Initial value problem

For simplicity we will usually only consider *initial value problems*, where we know $x(0)$ for some solution $x$. The above shows that this is acceptable.

To summarize, for every solution $x$ with some specified value for $x(0)$, there is in fact exactly one solution: $x(t) := x(0) e^{at}$


## $a$ as a parameter

We can also treat $a$ as a parameter and vary it, seeing how solutions vary as $a$ varies.

[image of varying solutions for $a > 0$, $a = 0$, $a < 0$]

The solutions are *stable* when $a \neq 0$ in the following sense: you can always find, for every $a$, some $b$ sufficiently close to $a$ such that $a$ and $b$ have the same sign, and hence the same qualitative behavior.
