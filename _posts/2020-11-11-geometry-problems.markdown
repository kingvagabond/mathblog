---
layout: post
title: Geometry Problems
date: 2020-11-11 20:58
category:
author:
tags: []
summary:
---

### 11/09/2020

![problem image](/assets/images/image-20201109101018448.png){:class="img-responsive"}

The distance from a point D inside equilateral triangle $\triangle{ABC}$ to the vertices are a, b and c respectively. Solve the area for $S_{\triangle{ABC}}$

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

---

### 11/12/2020

![A semicircle is constructed on line segment AB. Another  semicircle is constructed on chord CD, intersecting AB  at P and Q. If AP = 3,PQ = 7, and QB = 2, then  find the length CD.  c  Q  D  B ](/assets/images/clip_image001.jpg)

####  Solution 1

![image-20201113071324978](/assets/images/image-20201113071324978.png)

#### Solution 2

$OE=\dfrac{1}{2}, PE=\dfrac{7}{2},O_1E^2+OE^2=OO_1^2$, $O_1E^2 + PE^2 = PO_1^2 = CO_1^2=OO_1^2-\dfrac{1}{4}+\dfrac{49}{4}=OO_1^2 + 12$

$OO_1^2 + CO_1^2 = CO^2 = 6^2 \implies CO_1^2 = 24 \implies CD = \boxed{2\sqrt{24}=\sqrt{96}}$

---

### 11/13/2020

![image-20201113073810590](/assets/images/image-20201113073810590.png)

Point D is outside of circle O with diameter MN. From D make two lines DM and DB with points D, A and B on the circle O.

Extend OD and NA to intersect at point C. Prove that $CD \perp DB$.

