---
title: "Chap 1"
date: 2018-04-14T18:04:29-04:00
draft: False
categories: ["An Introduction to the Boltzmann Equation and Transport Processes in Gases by Gilberto Medeiros Kremer"]
tags: ["Boltzman"]

---

# 1. Collision frequency in ideal gas

$$\nu=n\pi d^2 \overline{g}$$

n is the number density, $\overline{g}$ is a mean relative velocity.

<!--more-->

# 2. Maxwellian Velocity Distribution Function

$$f(c_1,c_2,c_3)=n(\frac{m}{2\pi kT})^{\frac{3}{2}}e^{-mc^2/(2kT)}$$
defines the probability of finding molecules having velocity ($c_1$,$c_2$,$c_3$) &

$$F( c )dc=\int_0^{2\pi}\int_0^\pi n(\frac{m}{2\pi kT})^{\frac{3}{2}}
e^{-mc^2/(2kT)}c^2\sin\theta d\theta d\varphi dc$$
defines the probability of finding molecules having velocity magnitude c.

$$\rho=mn=\int_{-\infty}^{\infty}mfdc_1dc_2dc_3$$

$$\rho \epsilon=\frac{3}{2}nkT=\int_{-\infty}^{\infty}\frac{1}{2}mc^2fdc_1dc_2dc_3$$


$$=n(\frac{m}{2\pi kT})^\frac{3}{2}4\pi c^2e^{-mc^2/(2kT)}$$

Therefore, the mean thermal velocity of a molecule is

$$\overline{c}=\frac{\int_0^{\infty}cF( c )dc}{\int_0^{\infty}F( c )dc}=\sqrt{\frac{8kT}{\pi m}}$$

and the most probable velocity is 

$$c_{mp}=\sqrt\frac{2kT}{m}$$

and the mean quadratic velocity is 
$$c_{mq}=\sqrt{\overline{c^2}}=\sqrt{\frac{\int_0^{\infty}c^2F( c )dc}{\int_0^{\infty}F( c )dc}}=\sqrt\frac{3kT}{m}$$

The mean relative velocity, mean free time, and mean free path:
$$\overline{g}=\sqrt{2}\overline{c}$$

$$\tau=\frac{1}{4nd^2}\sqrt\frac{m}{\pi kT}$$

$$l=\frac{1}{\sqrt{2}\pi d^2 n}$$

The molecular flux over surface perp to $x_3$
$$\phi=\int_0^\infty\int_0^\frac{\pi}{2}\int_0^{2\pi}n(\frac{m}{2\pi kT})^\frac{3}{2}e^{-mc^2/(2kT)}c\cos\theta\sin\theta d\varphi d\theta dc$$

$$=\frac{n}{4}\sqrt\frac{8kT}{\pi m}=\frac{n}{4}\overline{c}$$

The total pressure
$$p=2\int_0^{+\infty} \int\_{-\infty}^{+\infty}\int\_{-\infty}^{+\infty}mc_3^2f(c_1,c_2,c_3)dc_1dc_2dc_3$$

$$=\frac{1}{3}\int\_{-\infty}^{+\infty}\int\_{-\infty}^{+\infty}\int\_{-\infty}^{+\infty}mc^2f(c_1,c_2,c_3)dc_1dc_2dc_3=nkT$$

$$p=\frac{2\rho \epsilon}{3}$$

## 2.1 Pressure tensor, heat flux vector and the molecular flux
(a) Consider a fluid confined between two parallel plates and the plate at the bottom is at rest while the top plate is moving with a constant
velocity. The velocity is dependent on the distance.
Sheer viscocity coefficient, independent of gas's density and proportional to the square root of the temperature
$$\mu=\frac{2\sqrt{mkT}}{3\pi^\frac{3}{2}d^2}$$

(b) Consider two parallel plates, the bottom one has a temperature $T_1$ and the top one has a temperature $T_2$, 
the total heat flux vector is given by
$$q=-3kl\frac{dT}{dx_3}\int_0^{\infty}\int_0^\frac{\pi}{2}\int_0^{2\pi}n(
\frac{m}{2\pi kT})^\frac{3}{2}e^{-mc^2/(2kT)}c^3\cos^2\theta\sin\theta d\varphi d\theta dc$$

$$=-\frac{nkl\overline{c}}{2}\frac{dT}{dx_3}$$

where $\lambda=\frac{nkl\overline{c}}{2}=\frac{k}{m}\frac{\sqrt{mkT}}{\pi^{\frac{3}{2}}d^2}$ is the thermal conductivity coefficient, independent on the density and is proportional to square root of temperature (similar to shear viscocity).

(3) The diffusion is process which follows from the thermal motion of the molecules of a gas mixture, when mass transfer from one region to another occurs due to the existence of density gradients of its consituents.
Consider gas is confined between two fixed parallel plates having the same temperature but different number density. 
Then the molecular flux cross a surface is
$$j_3=-2(\frac{m}{2\pi kT})\frac{3}{2}\frac{dn}{dx_3}l\int_0^\infty\int_0^\frac{\pi}{2}\int_0^{2\pi}c^3 e^{-mc^2/(2kT)}c^3\cos^2\theta\sin\theta d\varphi d\theta dc$$

$$=-\frac{\overline{c}l}{3}\frac{dn}{dx_3}=-D\frac{dn}{dx_3}$$

where the self-diffusion coefficient $D=\frac{\overline{c}l}{3}=\frac{2}{3\pi^\frac{3}{2}}\frac{\sqrt{mkT}}{mnd^2}$

The self-diffusion coefficient is inversely proportional to the number density but has the sam dependence on the temperature as the shear viscocity and thermal conductiviey coefficients.

## 2.2 Characteristic Dimensions
{{% figure class="center" src="/boltzmann/table1.png" alt="hugo even showcase" title="Characteristic Dimensions" %}}

## 2.3 Potentials
Short range force-valence force-repulsive, and due to a superposition of the electronic clouds of the molecules when they get closer to each other.

Long range force-van der Waals force-attractive and includes:

(1) electrostatic contributions (interactions between different multipole moments)

(2) induction contributions (interaction between a charge distribution of one molecule and the induced moments of another molecule)

(3) dispersion contribution (interaction between two induced charged distribution)

(a) Potential of hard sphere

$$\Psi( r )=\infty,  r<d$$

$$\Psi( r )=0,  r>d$$

(b) Potential of Centers of Repulsion
$$\Psi( r )=\frac{\kappa}{\nu-1}\frac{1}{r^{\nu-1}}, \kappa>0,\nu>1$$

$\nu=5$ is called Maxwellian potential

( c ) Potential of Lennard-Jones
$$\Psi ( r )=4\epsilon[(\frac{\sigma}{r})^{12}-(\frac{\sigma}{r})^6]$$

# 3. Brownian Motion
