---
layout: ../../layouts/PostLayout.astro
title: 'A semi-realistic approach to projectile motion.'
pubDate: 2025-09-27
description: 'Notes on projectile motion for imprecises needs.'
author: 'fireys'
tags: ["Physics", "Projectile", "Ballistics", "Game", "Development", "Interactive"]
---
## The Naïve approach
Let's face it. For most systems that need a _good enough_ way of handling physics-based projectiles, a simple **parabolic** curve will do the trick. Such a trajectory would model the gravitational forces acting on the projectile *`(incorrectly, mind you)`*[^1], and _assumes negligible air resistance_, a phrase which has permeated into thousands of papers and whose echo remains etched into the poor minds of every student learning mechanics.

#### The implementation
I'll briefly skim over the derivation of the underlying maths, as it has been documented[^2] extensively and taught[^3] to anyone ever enrolled in introductory mechanics classes. This will serve as the foundation for the projectile system, as I will build on it later.

For a parabolic trajectory, all projectiles will require both an initial **velocity** $u$ and a constant **acceleration** $a$. As well as a function to calculate both a **displacement**, or position, $s$, and velocity $v$ as a function of **time** $t$.

Having defined our values, we can derive the following functions:
$$
\begin{aligned}
f(t)&=s=ut+\frac{1}{2}at^2 \\
f(t)&=v=u+at
\end{aligned}
$$
These functions 

###### ⚠ more to be added... soon.... ⚠ ⚠ ⚠

[^1]: I am being awfully pedantic here -- but I personally think it'd be funny to mention that most systems fail to model the diminishing influence of gravity on the projectile. See: [Gravitational Fields](https://en.wikipedia.org/wiki/Gravitational_field)

[^2]: https://phys.libretexts.org/Bookshelves/University_Physics/Physics_(Boundless)/3%3A_Two-Dimensional_Kinematics/3.3%3A_Projectile_Motion

[^3]: https://www.sciencefacts.net/projectile-motion.html