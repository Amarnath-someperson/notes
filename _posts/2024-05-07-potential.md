---
title: Electric potential
authors: amarnath
math: true
categories: [Physics, Electrostatics]
tags: [charge, rest, potential]     # TAG names should always be lowercase
---

## General idea of potential

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

## continuous charge distributions

### ring of charge

![ring-charge.png](/assets/images/ring-charge.png)

Due to this ring of charge, the potential at the point where this is a charge $q$ is the sum of all potentials due to infinitesimal charges $dq$ on the ring. Since we do not have to worry about vectors here, we can just add the charge elements to get a charge $Q$ of the ring. Then, the potential

$$V=\frac{kQ}{\sqrt{R^2+r^2}}$$

where $r$ is the variable. This equation can also be obtained by integrating $\vec E \cdot d\vec r$.

The potential energy difference between the points $r=0$ and $r=r'$ (where $r'$ is the position of the point charge) is the exact amount of kinetic energy required to move that point charge from $r'$ to $r=0$, under ideal conditions. Solve using the work-energy theorem to get the equation for the minimum velocity to be imparted to the point charge (let it have a mass $m$) to get an equation


$$v_\text{min}=\sqrt{\frac{2kQ}{m}\left(\frac1a-\frac1{\sqrt{r^2+R^2}} \right)}$$
### thin shell of charge

![sphere-charge.png](/assets/images/sphere-charge.png)

In this given sphere of charge $Q$, we need to find the potential at three different points to get the whole idea of what is actually going on with it, which explains the three points taken in the pic. We know that spheres tend to behave like pont charges from both the outside and the surface (use gauss theorem to prove this). So, we can simply write

$$V_s=\frac{kQ}{R}$$
$$V_\text{ext}=\frac{kQ}{R+r_{P_s\to P_\text{ext}}}$$

For the interior point, we must find the electric field and integrate with $r$ in the equation $V=-\int \vec E\cdot \vec r$. If it is uniformly charged, find the electric field with gauss theorem or just by integration, and then integrate to find $V$. Subtract this with the surface potential to get the potential difference.

Take this sphere as conducting sphere, this will make things a lot easier. A conducting sphere has no $E$ inside, so the potential difference will be 0. Then, $V_\text{inside}=V_\text{surface}$.
Graph this to get a similar curve with a flat line after we go into the surface of the sphere.

![ef622d80288c38dd2c068f3f0a2fe77d.png](/assets/images/ef622d80288c38dd2c068f3f0a2fe77d.png)

Hey! Notice that this also explains the potential for a thin shell. This makes things a lot easier for me. But if it is a thick shell whose potentials at points must be found, then integrate.

Brielfly showing the potential at points for a thick shell with a point charge centrally enclosed within it:

![1b11e343dffcbfe76910185ca062a7fe.png](/assets/images/1b11e343dffcbfe76910185ca062a7fe.png)

At (1) the potential is

$$V_1=\frac{k(Q+q_0)}{b+r}$$

where $r$ is the distance from the surface of the larger shell (a thick shell can be considered as two thin shells with vacuum in between).

At (2) the potential is

$$V_2=\frac{k(Q+q_0)}{b}$$

The same for (3) and (4) as the negative and positive potential due to the point charge and inner thin shell cancel out.

At (5) the potential is

$$V_5=\frac{k(Q+q_0)}{b}+\frac{kq_0}{r}-\frac{kq_0}{a}$$

A plotted graph would look similar to the below figure

![85b6b0c0630a16a14fb1a6f6023c9670.png](/assets/images/85b6b0c0630a16a14fb1a6f6023c9670.png)

Now, consider a uniformly charged insulating sphere.

```(TO BE DERIVED)```

The final equations take the form

$$V_\text{out}=\frac{\rho R^3}{3\varepsilon_0}\times\frac1r$$

At the surface

$$V_\text{surf}=\frac{\rho R^3}{3\varepsilon_0}$$

On the inside

$$V_\text{ins}=\frac{\rho}{3\varepsilon_0}\left(\frac{R^2-r^2}{2}\right)$$

At the centre

$$V_0=\frac{3}{2}V_\text{surf}$$

### line of charge

```TO CONTINUE```
