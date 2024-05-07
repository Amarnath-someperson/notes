---
title: Electric potential
authors: amarnath 
math: true
categories: [Physics, Electrostatics]
tags: [charge, rest, potential]     # TAG names should always be lowercase
---

# General idea of potential

> The potential at a point in a conservative force vector field is the work done by an opposing force in bringing a unit quantity from a point where there is no conservative force field to a point within it. From an electrostatics point of view, the origin point is considered to be infinity.

Thus, the potential can be negative or positive or 0. Following the equation for work done 

$$V=W_{\infty\to P}=\vec F_\text{applied}\cdot \vec r_{\infty\to P}=\vec F_E\cdot \vec r$$

In electrostatics, the force experienced by a unit charge at a point is the electric field at that point, so the work done against the electric field to bring a unit positive test charge from infinity to a point $P$ is the integral of infinitesimally small work done in bringing it from infinity to that point, i.e., 

$$V=-\int_\infty^P\vec E \cdot d\vec r$$

The negative sign is due to the fact that the applied force per unit charge is against the electric field direction at a point. 

In space, take the partial derivative of the potential in all three axes to find the direction of electric field in each 

$$E=-\left(\frac{\partial V}{\partial x}\hat i + \frac{\partial V}{\partial y}\hat j + \frac{\partial V}{\partial z}\hat k \right)$$

If the electric field is in the direction of the potential, then $V=-E\Delta r$  (dot product gives $\cos 0 = 1$).

Potential energy is the potential multiplied by the magnitude of quantity to be brought in, as

$$U=-\int \vec F_E \cdot \vec r \\\implies F_E=\frac {dU}{dr}=qE=q\frac {dV}{dr}$$

## note on equipotential surfaces

An equipotential surface is one that at no two points in it has a potential difference. The work done in moving any charge on the surface to any other point in the sruface is 0, i.e., $W=q\Delta V =0$.

Equipotential surfaces have certain properties as listed below.

1. Electric field lines are always normal to equipotential surface ($dV=Edr\cos\theta=0\implies \theta = 90^\circ$). **Conducting surfaces** are equipotential in nature (they have no electric field within).
2. Equipotential surfaces **do not** intersect each other.
3. For a given potential difference, equipotential surfaces are closely packed in a region of high electric field, and far apart in one of low electric field intensity.

Example

![e_field_pot.png](/assets/images/e_field_pot.png)


## potential due to charges

### point charges

![single_point_charge.png](/assets/images/single_point_charge.png)

To bring the test charge from infinity to $r$, find the work done to find the potential at the point at that distance. Integrate

$$V=-\int_\infty^r Edx\cos 0$$

Solve to get

$$V=+\frac{kq}r\\ U=q_0V$$

For a system of charges, use the superposition principle to add the potential due to each charge, which yields the equation $V=\sum_n V_{q_0, q_n}$ ($n \in \mathbb N$).

###  dipoles

![dipole.png](/assets/images/dipole.png)

Along the **axial** line, 

$$V_C=\frac{kq}{r-a}+ \frac{k(-q)}{r+a}$$

Solve to get 

$$V_C=\frac{kp}{r^2-a^2}$$

If $r>>a$, $V= kp/r^2$.

![equatorial_p_dipole.png](/assets/images/equatorial_p_dipole.png)

Along the **equatorial** line,

$$V_C=\frac{kq}{\sqrt{a^2+r^2}}+\frac{k(-q)}{\sqrt{a^2+r^2}}=\fbox 0$$

![short_dipole_2.png](/assets/images/short_dipole_2.png)

At **any point** due to a **short dipole**,

$$V_c=\frac{kq}{r_2}-\frac{kq}{r_1}$$

For $r_1r_2\approx r^2$, and $r_2-r_1=2a\cos\theta$, solve to get

$$V_C=\frac{kp\cos\theta}{r^2}$$

## PLACEHOLDER ( TO BEGIN FROM RING )






