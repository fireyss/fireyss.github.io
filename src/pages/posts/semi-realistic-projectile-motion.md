---
layout: ../../layouts/PostLayout.astro
title: 'A semi-realistic approach to projectile motion.'
pubDate: 2025-09-27
description: 'Notes on projectile motion for imprecises needs.'
author: 'fireys'
image:
    url: 'https://docs.astro.build/assets/rose.webp'
    alt: 'The Astro logo on a dark background with a pink glow.'
tags: ["Physics", "Projectile", "Ballistics", "Game", "Development", "Interactive"]
---

## The Naïve solution

Lets face it, for most systems that need a _good enough_ way of handling physics-based projectiles; a simple **parabolic** curve will do the trick. Such a trajectory would model the gravitational forces acting on the projectile _(typically ignoring the diminishing attraction gravity has the higher up you go)[^1]_ and provide a believable experience to anyone using your system.

#### The implementation

I am going to skim over the unnecessary details for this as the mathematics is already covered in most (if not, all) introductory mechanics classes across the globe.



[^1]: This an awfully pedantic thing to mention but I personally think it's funny. See: [Gravitational Fields](https://en.wikipedia.org/wiki/Gravitational_field)
