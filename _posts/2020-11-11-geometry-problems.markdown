---
layout: post
title:
date: 2020-11-11 20:58
category:
author:
tags: []
summary:
---

## Geometry Problems ##

### 11/09/2020

![problem image](/assets/images/image-20201109101018448.png){:class="img-responsive"}

### The distance from a point D inside equilateral triangle $\triangle{ABC}$ to the vertices are a, b and c respectively. Solve the area for $S_{\triangle{ABC}}$

#### Solution 1

![solution 1 image](/assets/images/image-20201109101623268.png){:class="img-responsive"}

Rotate $\triangle{BDC}$ by $60^{\circ}$ to $\triangle{AEC}$ so we have $AE=b$.

Then $cos{\angle{ADE}}=\dfrac{a^2+c^2-b^2}{2ac}$,

$sin{\angle{ADE}}=\sqrt{1-\dfrac{(a^2+c^2-b^2)^2}{4a^2c^2}}$

$ = \dfrac{ \sqrt{(2ac+a^2+c^2-b^2)(2ac-a^2-c^2+b^2)} }{2ac} $

$ = \dfrac{\sqrt{(a+c+b)(a+c-b)(b+a-c)(b-a+c)}}{2ac} $

Then we know

$cos{\angle{ADC}}=cos(\angle{ADE}+60^{\circ})=cos{\angle{ADE}} \cdot cos60^{\circ} - sin{\angle{ADE}} \cdot sin{60^{\circ}}$

$=\dfrac{a^2+c^2-b^2}{4ac}-\dfrac{\sqrt{3(a+b+c)(a+b-c)(b+c-a)(c+a-b)}}{4ac}$

$=\dfrac{a^2+c^2-AC^2}{2ac}$

$ \implies AC^2=\dfrac{a^2+b^2+c^2}{2}+\dfrac{\sqrt{3(a+b+c)(a+b-c)(b+c-a)(c+a-b)}}{2} $

$ \implies S_{\triangle{ABC}}=\dfrac{\sqrt{3}}{4}AC^2 $

$=\boxed{\dfrac{\sqrt{3}}{8}(a^2+b^2+c^2)+\dfrac{3}{8}\sqrt{(a+b+c)(a+b-c)(b+c-a)(c+a-b)}}$

#### Solution 2

![Solution 2 image](/assets/images/image-20201112142202515.png)

Rotate $\triangle{BDC}$ by $60^{\circ}$ to $\triangle{AEC}$ , $\triangle{CDA}$ by $60^{\circ}$ to $\triangle{BFA}$, $\triangle{ADB}$ by $60^{\circ}$ to $\triangle{CGB}$.

Easy to find that $CG=AF=a, AE=BG=b, BF=CE=c$.

So $S_{AFBGCE}=2 \cdot S_{\triangle{ABC}}=3 \cdot S_{\triangle{CDG}} + S_{\triangle{CDE}} + S_{\triangle{BDG}} + S_{\triangle{ADF}}$

According to [Heron's formula](https://en.wikipedia.org/wiki/Heron%27s_formula) :

$S_{\triangle{CDG}}=\dfrac{\sqrt{(a+b+c)(a+b-c)(b+c-a)(c+a-b)}}{4}$

And we know

$S_{\triangle{CDE}}=\dfrac{\sqrt{3}}{4} c^2$, $S_{\triangle{BDG}}=\dfrac{\sqrt{3}}{4} b^2$, $S_{\triangle{ADF}}=\dfrac{\sqrt{3}}{4} a^2$

So we have

$S_{\triangle{ABC}}=\boxed{\dfrac{\sqrt{3}}{8}(a^2+b^2+c^2)+\dfrac{3}{8}\sqrt{(a+b+c)(a+b-c)(b+c-a)(c+a-b)}}$