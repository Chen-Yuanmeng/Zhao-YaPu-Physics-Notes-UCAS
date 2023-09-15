# 力学 赵亚溥老师 笔记

## 2023/9/11

### Introduction

**2022 Nobel Prize for Physics**: for experiments with entangled photons, establishing the violation of Bell inequalities and pioneering quantum information science

Three people won the prize: 
- Alain Aspect (France)
- John Clauser (the U.S.)
- Anton Zeilinger (Austria)

This brings about the problem of **`local realism (局部现实主义)`** and **`principle of locality (定域性原理)`**, which is believed true in CLASSICAL mechanics or electromagnetics.

> 思考：科学哲学上，“真实”是如何定义的？

### 1. Newtonian Mechanics, 1687: 牛顿力学

In the *Principia* writes `the first Principle`: 

$$\overrightarrow F=\frac{\mathrm d \vec p} {\mathrm dt}$$

and Newton also gives `the Law of Universal Gravitation`:

$$ \overrightarrow F = -\frac{Gm_1m_2}{r^2} \hat {\vec r} $$


### 2. Some equations

- #### Navier-Stokes equations: 粘性不可压缩流体动量守恒的运动方程
$$ {\partial \vec v \over \partial t} +(\vec v \cdot \overrightarrow V) \cdot \vec v = -{1 \over \rho} \overrightarrow \nabla p + \mu \nabla^2 \vec v + \vec g$$

- #### Euler-Lagrange equation: 拉格朗日方程
$${\partial L \over \partial q_\alpha}-{\mathrm d \over \mathrm dt}\cdot {\partial L \over \partial \dot q_\alpha}=0, L=T-V$$

- #### Hamilton Mechanics: 哈密顿力学
$$
\left \{
\begin{array} {c}
\dot q_\alpha = \dfrac{\partial H}{\partial p_\alpha} \\ 
\dot p_\alpha = \dfrac{\partial H}{\partial q_\alpha}
\end{array}
\right.
$$

### 3. 