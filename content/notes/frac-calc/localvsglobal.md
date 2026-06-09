---
Title: Locality vs Globality
---
[back](/notes/frac-calc)

9th June 2026

Ooh baby, this is where shit gets real.

### What is Locality and Globality btw ?

Ok so think about an operator like derivative at some point $a$. This derivative only requires the behaviour of the function in the *neighbourhood* of a point like $a = 0$. Hence, we call it local.

We denote this "neighbourhood" by $x \in [a - \epsilon, a + \epsilon]$ or $|x-a| < \epsilon$.

For an operator like convolution, it requires the behaviour of the function over a range, $x \in [\alpha, \beta]$. The resultant is dependent on how the function behaves throughout the given interval. Hence we call it global.

Confused ? Here's a better definition.

Operator - Local $\iff$ function - near $a$ matters.

Operator - Global $\iff$ function - all throughout some interval like $[\alpha, \beta]$.

*Lemme be real for a moment - Don't worry if you don't get this, hit me up if you got any questions as always.*

### Why talk about this in fractional calculus ?

Well, the main difference between my idea and classical operators are that my framework is local and the classical operators are global in nature.

Locality does have it's perks, because it allows the use of infinite series, which, once truncated (cut into smaller pieces), can be used to numerically approximate fractional derivatives.

But globality is why most applications exist for fractional calculus, of the wierd ability of the operators to take the "past" of the function into account to produce a value for a given point.

My operator can be developed into the classical operators through some clever algebra and analysis tricks, but the philosophical answer as to how the local series becomes global remains unanswered.

Thanks for reading, lots of ummas,

Madhav

PS: Most of my extended work are to be presented at [RAAM, 2026](https://sites.google.com/view/raam2026/) at IIT Hyderabad. So after the conference, I will post the break down of the paper here in further notes.