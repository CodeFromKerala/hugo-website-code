---
Title: Operator and Basics
---

### What is an Operator ?

An operator can be thought of as a function of functions. To be clearer, it maps a function to another. For example, similar to how $ f(x) $ maps $ x \to y $ as $f(x) = y$, we can use $O$, which is an operator to map $f \to g$ as $O \\, f = g$.

### Where did this fractional calculus idea come from ?

Well, the fractional calculus story begins with Riemann, *who formed a kernel through heuristic methods*, which is a complicated way of saying that he made an educated guess as to which what the fractional derivative operator will look like. His work was continued by Liouville, who found a inductive proof of the Riemann operator.

There are two classical operators for fractional calculus I prefer, they are called the Riemann-Liouville Differ-Integral (mentioned above) and the Caputo Derivative.

The Riemann-Liouville Differ-Integral ($I^r_\alpha$) or RL for short,

$$ I^r_\alpha f(x) = \frac{1}{\Gamma(r)} \int_\alpha^x (x-t)^{r-1} f(t) \\, dt $$

The Caputo Derivative, which I will write as just Caputo,

$$ {}^{C}D_t^\alpha f(x) = \frac{1}{\Gamma(n-\alpha)}\int_0^x\frac{f^{(n)}(t)}{(x-t)^{\alpha-n+1}}\\, dt, \qquad n-1 < \alpha < n. $$

Now, don't be scared by these huge fuckass formulae. These are just the classical versions of the theory condensed to scare people. We will discuss these with more clarity in the next note.

## My Idea

Ok. Lets get into my ideas.

Take some function $f$. It is said to be *analytic* in $\mathbb{R}$ if all of its natural derivatives exist, and it's Taylor series converge to the function throughout $\mathbb{R}$. Keep that in the noggin for now.

For a function $f(x) = x^n$, we can write
$$ \frac{d}{dx} f(x) = nx^{n-1} \qquad \frac{d^2}{dx^2} f(x) = n(n-1)x^{n-2} $$

If we continue this madness for a while, we can see that for some $r \in \mathbb{N}$ and $r < n$,
$$ \frac{d^r}{dx^r} f(x) = \frac{n!}{(n-r)!}x^{n-r} $$

But why though ?

We can see that $\frac{d^r}{dx^r} f(x)$ eventually approaches something like $n(n-1)(n-2).....(n-r)x^{n-r}$. So, we can conclude that it can be written as above, if you have learnt a bit of 12th math.

Now suppose we want to extend this to the fractional derivative. We already chose $D^r$ as a name of our operator, where $r$ is the order of derivative. So we can write out,

$$ D^r x^n = \frac{n!}{(n-r)!} x^{n-r}$$

But earlier we said that this can only be used if $n, r \in \mathbb{N}$, and for good reason. Lookie here at the factorial functions, $n!$ and $(n-r)! \\,$. For just natural number $n$ and $r$ this is fine, but when we extend to real numbers, we gotta use a replacement, called the Gamma function ($\Gamma(x)$).

Hence, for any $n, r \in \mathbb{R}$,

$$ D^r x^n = \frac{\Gamma(n+1)}{\Gamma(n-r+1)}x^{n-r} $$

since $\Gamma(x+1) = (x)!$

### The Gamma Function

Welcome to where it gets interesting.

The Gamma function, $\Gamma(x)$, is used to *analytically extend* the factorial function to the real numbers. What this word soup means is that the Gamma function behaves just like factorial function at natural numbers, but gives you meaningful results for real values.

Here's some figures for you people who can only understand with colours.

![Factorial Natural](/images/factorial-n.png)
Here, we show a scatter plot for the factorial function $y = x!$. If we draw a smooth graph along this framework, holding on to intuition like if $x_1 < x_2$, then $x_1! < x_2!$, we get the Gamma function, as shown below.

![Factorial Real](/images/factorial-r.png)
Here, you may notice some inconsistancies with both graphs around $x = 0$. This is because the analytic continuation, otherwise the Gamma function, has *poles* at $x = 0$. Now, poles is a fun way of saying that the function diverges to $\pm \infty$.

In fractional calculus, we use the function $\Gamma(x)$ to replace the factorial functions, but in the practical field, we use the logarithm of the Gamma function for more accurate results.