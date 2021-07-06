---
title: Foo
author: Billy
date: 2021-07-04
---

A while ago I stumbled across an integral:

$$I_n \coloneqq \int_0^\pi e^{\cos\theta} \cos(\sin\theta - n\theta) \diff\theta.$$

Using Euler's formula, $\cos x$ is the real part of $e^{ix}$, so we can rewrite the integral as

$$I_n = \frac{1}{2} \Re\left[\int_0^{2\pi} e^{e^{i\theta}} e^{-i n \theta} \diff\theta \right].$$

With the substitution $u = e^{i\theta}$ and $\diff u = iu\diff\theta$, $I_n$ becomes a contour integral around the unit disk $\gamma$:

$$I_n = \frac{1}{2} \Re\left[i \oint_\gamma \frac{e^u}{u^{n+1}} \diff u \right]$$

This expression is tantalizingly reminiscent of [Cauchy's integral formula]

$$f^{(n)}(a) = \frac{n!}{2\pi i} \oint_\gamma \frac{f(z)}{(z-a)^{n+1}} \diff z.$$

<img src="./goat_avatar.jpg" style="clip-path: circle(50%);"></img>

[Cauchy's integral formula]: https://en.wikipedia.org/wiki/Cauchy%27s_integral_formula