---
title: Moving charges and magnetism
authors: [aman, amarnath] 
math: true

categories: [Physics, Magnetism]
tags: [charge, motion, magnet]     # TAG names should always be lowercase
---

# magnetic fields

> A magnetic field is an invisible region in which a magnetic current carrying wire or a moving charge experience a magnetic force.

SI unit: tesla (T), weber per metre squared ($\mathrm{Wb~m^{-2}}$).
CGS unit: gauss (G), $1~\mathrm T = 10^4~\mathrm G$.

![magfield.png](/assets/images/magfield.png)

## biot-savart law

Use: To find the magnitude of the magnetic field.

> The elemental magnetic field due to a current carrying conductor is directly proportional to the current through the conductor, the length of the element taken, the angle between the distance vector from $dl$ to the point, and the element $dl$, and inversely proportional to the square of the distance between the $dl$ to the point ($|\vec r|$)

Consider an infinitely long conductor, with current $i$ passing through it

![biot-savart.png](./biot-savart.png)

According to Biot-Savart law,$$dB=\frac{\mu_0}{4\pi}\frac{idl\sin\theta}{r^2}$$
where $\mu_0/4\pi$ is a constant for vacuum, the permeability of free space. For$$\mu_0=4\pi\times 10^{-7}$$
Then, $$dB=10^{-7}\times\frac{idl\sin\theta}{r^2}$$

### vector form of biot-savart law

Multiply and divide by $r$ to get the cross product $$dB=\frac{\mu_0}{4\pi}\frac{i\vec{dl}\times \vec{r}}{r^3}$$Use the right-hand thumb rule to find the direction of the cross product.




