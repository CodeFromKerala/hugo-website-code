---
Title: Variational Calculus
---

Welcome. Variational Calculus is not THAT scary. It's just big-brain optimisation.

Remember how we used to find the minimum of a function $ f(x) $ ?

Same thing. Instead, we use a functional.

## WTF is a functional ?

Functional can be compared to a function, but instead of mapping a number to another, we map a function to a number.

In weird math symbols, $ f : A \to B $ as $y = f(x), \\, x \in A, y \in B$. Here, the functional, $J : \mathcal{F} \to A$ as $ J[f] = n, \\, f \in \mathcal{F}, n \in A$.

*All this scary stuff just says that the functional J takes in some function and gives output number.*

In the works of Leonhard Euler and Joseph-Louis Lagrange, the functional is minimised. *forshadowing*


## Minimisation of functional

To find the minimum of a functional, we just use the first derivative - to find where the slope reaches zero. However, this is not really the minimum, but where the function becomes stationary.

But here, if you look closer, the functional is defined by a function, rather than a number. We already know that in multivariable calculus, there is an infinite number of directions we can take the derivative in. 

It is the same for function spaces in the sense as they are infinite dimensional. The fun thingy is that we can choose the "direction" of the derivative we take so that we can minimise along it.

Suppose our functional is $ J[f] $ and $ y $, the required function, minimises it.

Now if we just determine that the input $f$ is of the form below such that it is the "variation" of optimal function $y$.

$$ f = y + \epsilon \eta $$

where we take $\eta$ as an arbitrary function (random function we chose for "direction").

Why tho ?

See, here $\epsilon$ is the only change-able variable. Hence, we can re-write the functional as a function.

$$ \phi(\epsilon) = J[y+\epsilon\eta] $$

Yay. We are almost there.

Now we can just minimise / maximise this function like any real function. Just take derivative, set to zero.

$$ \frac{d}{d\epsilon} \phi(\epsilon) = 0$$

Now, this functional can be of very, very, weird forms. Maybe integral forms.

But, the notation of the stationary-ness of a function is given by 

$$ \delta J = 0 $$

called the *variation* of $J$, which is equivalent to the ODE of $\phi (\epsilon)$ above.

If you have trouble keeping up with the notation - consult analysis textbooks for basic real analysis.

*Just know the ideas here are non-rigorous for just understanding physics. I will be uploading a more rigorous definitions later in my real analysis series.*