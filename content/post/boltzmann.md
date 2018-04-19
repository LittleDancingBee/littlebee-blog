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

$$\Phi( r )=\infty,  r<d$$

$$\Phi( r )=0,  r>d$$

(b) Potential of Centers of Repulsion
$$\Phi( r )=\frac{\kappa}{\nu-1}\frac{1}{r^{\nu-1}}, \kappa>0,\nu>1$$

$\nu=5$ is called Maxwellian potential

( c ) Potential of Lennard-Jones
$$\Phi ( r )=4\epsilon[(\frac{\sigma}{r})^{12}-(\frac{\sigma}{r})^6]$$

# 3. Brownian Motion
The particles in suspension in water are moving due to an impulse (collisions between the molecules of the fluid and the particles and some molecules of the fluid have colovities larger than its mean thermal velocity) and braked by viscous force. The motion of a particle is described by Langevin equation:
$$m\frac{dv}{dt}=-\frac{m}{\tau}v+F(t)$$

where $\tau$ is a constant characteristic time and $F(t)$ is a stationary random force with a vanishing time average:
$$\overline{F(t)}=\frac{1}{\theta}\int_0^\theta F(t+t')dt'=0$$

The Langevin's equation is valid if:

(a) the fluid is in a medium where the external actions are constant in time (e.g., the temperature must be constant in time)

(b) the mass of the particles in suspension is larger than the mass of the fluid molecules

\(c\) the particle number density of the suspension particles is small, so that the collisions between themselves are neglected

ergodic hypothesis: a mechanical system will go beyond all possible microstates before returning to a given microstate, i.e., over a long period of time all accessible microstates are equally probable.

Multiply through $x/m$, the Langiven equation becomes
$$\frac{d}{dt}(xv)+\frac{1}{\tau}(xv)=v^2+\frac{1}{m}xF(t)$$.

Taking the average and use $\langle xF(t)\rangle=0$ and $\frac{m\langle v^2\rangle}{2}=\frac{kT}{m}$ (energy equipartition principle), the Langiven equation becomes
$$\frac{d\langle xv\rangle}{dt}+\frac{1}{\tau}\langle xv\rangle=\frac{kT}{m}$$

The solution is 
$$\langle xv\rangle=Ce^{-\frac{t}{\tau}}+\frac{\tau kT}{m}$$

with initial condition $x(t=0)=0$, $C=-\tau kT/m$, therefore, we obtain

$$\langle x^2\rangle=\frac{2\tau kT}{m}[t-\tau(1-e^{-\frac{t}{\tau}})]$$

(a) for $t\gg\tau$, the solution is $\langle x^2\rangle=\frac{2\tau kT}{m}t$. The mean square displacement is proportional to time.

(b) for $t\ll\tau$, the solution is $\langle x^2\rangle=\langle v^2\rangle t^2$. The suspension particles move as free particles with velocity equal to its mean square velocity.
# 4. Binary Collision
## 4.1 Conservation laws 
In rarefied gases, the probability of collisions with three more molecules involved is negligible compared with the binary collision. 

Two particles having locations ($r_i^1$, $r_i^2$) and velocities pre-collision ($\bf c$, $\bf c_1$) and post-collision($\bf c'$, $\bf c'_1$) . Denote the relative position vector as $\bf {r}=\bf r^2-\bf r^1$ and the relative velocity as $\bf g=\bf c_1-\bf c$ and $\bf g'=\bf c_1'-\bf c'$. Denote the interaction potential as $\Phi( r )$. We have
$$m\ddot{r}_i^1=-\frac{\partial\Phi( r )}{\partial r_i^1},
m\ddot{r}_i^2=-\frac{\partial\Phi( r )}{\partial r_i^2}=\frac{\partial\Phi( r )}{\partial r_i^1}$$. 

By adding these two equations, we obtain
$$m\ddot{r}_i^1+m\ddot{r}_i^2=0$$

Therefore, we have the conservation of momentum before and after the collision
$$m{\bf c}+m{\textbf c_1}=m{\bf c'}+m\bf {c'_1}$$ 

and
$$\mu \ddot{\bf {r}}=-\frac{\partial\Phi}{\partial r}\frac{\bf {r}}{r}$$

where $\mu=m/2$.

Multiply by $\bf\dot{r}$ and integrate the above equation lead to
$$\frac{d}{dt}[\frac{\mu}{2}{\bf{\dot r}}^2+\Phi( r )]=0$$

This is energy conservation law through the collision

$$\frac{\mu}{2}{\bf{\dot r}}^2+\Phi( r )=\frac{\mu}{2}g^2=\frac{\mu}{2}g'^2$$

and then
$$\frac{1}{2}mc^2+\frac{1}{2}mc_1^2=\frac{1}{2}mc'^2+\frac{1}{2}mc_1'^2$$

From $\mu\ddot{\bf r}=-\frac{\partial \Phi}{\partial r}\frac{\bf r}{r}$, we have $\frac{d}{dt}[\mu\dot{\bf r}\times\bf{r}]=0$. Therefore, $\bf{\dot r}\times\bf{r}=$constant.
In the collision process, the momentum and energy is conserved and the relative motion between the molecules is confined to a plane.
Define apsidal vector $\bf{k}=\frac{\bf{g}-\bf{g'}}{|\bf{g}-\bf{g'}|}$

we have
$$\bf{c'_1}=\bf{c_1}-\bf k(k\cdot g)$$
$$\bf{c'}=\bf{c}+\bf k(k\cdot g)$$

## 4.2 Two Species Collision
If the binary collision occurs between two constituents $m\_\alpha$ and $m\_\beta$ with precollision velocity $\bf{c}\_\alpha$ and $\bf{c}\_\beta$ and postcollision velocity $\bf{c'}\_\alpha$ and $\bf{c'}\_\beta$, the conservations of momentum and energy are
$$m\_\alpha{\bf c}_\alpha+m\_\beta{\bf c}\_\beta=m\_\alpha{\bf c'}\_\alpha+m\_\beta{\bf c'}\_\beta$$

$$\frac{1}{2}m\_\alpha{\bf c}_\alpha^2+\frac{1}{2}m\_\beta{\bf c}\_\beta^2=\frac{1}{2}m\_\alpha{\bf c'}\_\alpha^2+\frac{1}{2}m\_\beta{\bf c'}\_\beta^2$$

With the apsidal vector 
$${\bf k}^{\beta\alpha}=\frac{{\bf g}_{\beta\alpha}-{\bf g'}\_{\beta\alpha}}{|{\bf g}\_{\beta\alpha}-{\bf g'}\_{\beta\alpha}|}$$

The asymptotic velcoties 
$${\bf c'}_{\beta}={\bf c}\_\beta-2\frac{m\_{\alpha\beta}}{m\_\beta}{\bf{k}^{\beta\alpha}}(\bf{k}^{\beta\alpha}\cdot {\bf g}\_{\beta\alpha})$$

$${\bf c'}_{\alpha}={\bf c}\_\alpha-2\frac{m\_{\alpha\beta}}{m\_\alpha}{\bf{k}^{\beta\alpha}}(\bf{k}^{\beta\alpha}\cdot {\bf g}\_{\beta\alpha})$$

with $m\_{\alpha\beta}=m\_\alpha m\_\beta /(m\_\alpha + m\_\beta)$

## 4.3 Scattering angle $\chi$
Write the equations in the polar coordinate ($r$,$\varphi$), we have
$$\frac{\mu}{2}(\dot r^2 + r^2\dot\varphi^2)+\Phi( r )=\frac{\mu}{2}g^2$$

$$r^2\dot\varphi=bg$$

follows:
$$(\frac{ds}{d\varphi})^2=1-s^2-\frac{2\Phi}{\mu g^2}$$

where $s=b/r$ is a dimensionless variable and $\dot r/\dot\varphi=dr/d\varphi=-b(ds/d\varphi)/s^2$

The scattering angle $\chi=\pi-2\theta$ is then
$$\chi=\pi-\int_{0}^{s\_{max}}(2/ \sqrt{1-s^2-\frac{2\Phi(b/s)}{\mu g^2}})ds$$

$s\_{max}$ is the positive root of the equation $1-s^2-\frac{2\Phi(b/s\_{max})}{\mu g^2}=0$

The scattering angle for a given potential is determined by the impact parameter $b$ and the relative velocity $g$.

{{% figure class="center" src="/boltzmann/binarycollision.png" alt="hugo even showcase" title="Binary Collision Sketch" %}}

(a) Centers of repulsion potential
$$\chi=\pi-\int_{0}^{s\_{max}}(2/ \sqrt{1-s^2-\frac{2}{\nu-1}(\frac{s}{s\_0})^{\nu-1}})ds$$

and $s\_0=b(\frac{\mu g^2}{\kappa})^{\frac{1}{\nu-1}}$ 

(b)The hard-sphere potential can be obtained by setting a limit of the centers of repulsion potential.

Introduce a new parameter $\kappa=\kappa' d^{\nu-1}$, where $\kappa'$ is a constant and d is the molecular diameter, we then have
$$\Phi( r )=\frac{\kappa'}{\nu-1}(\frac{d}{r})^{\nu-1}$$

then 
$$s\_0=\frac{b}{d}(\frac{\mu g^2}{\kappa'})^{\frac{1}{\nu-1}}$$

and 
$$\lim_{\nu \to \infty}=\frac{b}{d}$$

for $r\gg d$, $\lim\_{\nu\to\infty}\frac{1}{\nu-1}(\frac{s}{s{\_0}})^{\nu-1}=0$, then $\chi=\pi-\int\_{0}^{s\_{max}}(2 / \sqrt{1-s^2} ds=2\arccos s\_{max}$, where $s\_{max}=b/r^{min}$

(i) for $s\_0\gg 1$, nonexistence of collision, $\chi=0$

(ii) for $s\_0\ll 1$, existence of a collision and the scattering angle is $\chi=2\arccos(\frac{b}{d})$.
## 4.4 Differential Cross Section
{{% figure class="center" src="/boltzmann/differentialcrosssection" alt="hugo even showcase" title="Differential Cross Section" %}}

The differential cross section, a function of the scattering angle and of the kinetic energy of the relative motion $\sigma(\chi,g)$, is defined as the ratio of the number of scattered particles $\Delta N$ per unit of time and per element of solid angle, and the flux of the impinged molecules:
$$\sigma (\chi,g)=\frac{\Delta N(\Delta t d\Omega)}{\Delta N/(\Delta t b db d\epsilon}=\frac{bdbd\epsilon}{d\Omega}$$
