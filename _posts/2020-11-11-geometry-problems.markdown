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

![solution image](/assets/images/image-20201109101623268.png){:class="img-responsive"}

Rotate $\triangle{BDC}$ by $60^{\circ}$ to $\triangle{AEC}$ so we have $AE=b$.

Then $cos{\angle{ADE}}=\dfrac{a^2+c^2-b^2}{2ac}$,

$sin{\angle{ADE}}=\sqrt{1-\dfrac{(a^2+c^2-b^2)^2}{4a^2c^2}}$

$=\dfrac{\sqrt{(2ac+a^2+c^2-b^2)(2ac-a^2-c^2+b^2)}}{2ac}$

$=\dfrac{\sqrt{(a+c+b)(a+c-b)(b+a-c)(b-a+c)}}{2ac}$

Then we know

$cos{\angle{ADC}}=cos(\angle{ADE}+60^{\circ})=cos{\angle{ADE}} \cdot cos60^{\circ} - sin{\angle{ADE}} \cdot sin{60^{\circ}}$

$=\dfrac{a^2+c^2-b^2}{4ac}-\dfrac{\sqrt{3(a+b+c)(a+b-c)(b+c-a)(c+a-b)}}{4ac}$

$=\dfrac{a^2+c^2-AC^2}{2ac}$

$\implies AC^2=\dfrac{a^2+b^2+c^2}{2}+\dfrac{\sqrt{3(a+b+c)(a+b-c)(b+c-a)(c+a-b)}}{2}$

$\implies S_{\triangle{ABC}}=\dfrac{\sqrt{3}}{4}AC^2$

$=\boxed{\dfrac{\sqrt{3}}{8}(a^2+b^2+c^2)+\dfrac{3}{8}\sqrt{(a+b+c)(a+b-c)(b+c-a)(c+a-b)}}$