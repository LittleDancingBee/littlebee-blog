---
title: "Note-An Introduction to the Boltzmann Equation and Transport Processes in Gases by Gilberto Medeiros Kremer"
date: 2018-04-14T18:04:29-04:00
draft: False
---

# Chap 1


## 1. Collision frequency in ideal gas:

$$\gamma=n\pi d^2 \overline{g}$$

n is the number density, $\overline{g}$ is a mean relative velocity.

<!--more-->

## 2. Maxwellian Velocity Distribution Function

$$f(c_1,c_2,c_3)=n(\frac{m}{2\pi kT})^{\frac{3}{2}}e^{-mc^2/(2kT)}$$
defines the probability of finding molecules having velocity ($c_1$,$c_2$,$c_3$)

$$\rho=mn=\int_{-\infty}^{\infty}mfdc_1dc_2dc_3$$

$$\rho \epsilon=\frac{3}{2}nkT=\int_{-\infty}^{\infty}\frac{1}{2}mc^2fdc_1dc_2dc_3$$

$$F( c )dc=\int_0^{2\pi}\int_0^\pi n(\frac{m}{2\pi kT})^{\frac{3}{2}}
e^{-mc^2/(2kT)}c^2\sin\theta d\theta d\varphi dc$$

$$=n(\frac{m}{2\pi kT})^\frac{3}{2}4\pi c^2e^{-mc^2/(2kT)}$$

Therefore, the mean thermal velocity of a molecule is

$$\overline{c}=\frac{\int_0^{\infty}cF( c )dc}{\int_0^{\infty}F( c )dc}=\sqrt{\frac{8kT}{\pi m}}$$

and the most probable velocity is 

$$c_{mp}=\sqrt\frac{2kT}{m}$$

and the mean quadratic velocity is 
$$c_{mq}=\sqrt{\overline{c^2}}=\frac{\int_0^{\infty}c^2F( c )dc}{\int_0^{\infty}F( c )dc}=\sqrt\frac{3kT}{m}$$

The mean relative velocity, mean free time and mean free path:
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

