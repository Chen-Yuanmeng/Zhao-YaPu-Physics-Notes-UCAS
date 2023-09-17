# 力学 赵亚溥老师 笔记

## 2023/9/11

### Introduction

**2022 Nobel Prize for Physics**: for experiments with entangled photons, establishing the violation of Bell inequalities and pioneering quantum information science

Three people won the prize: 
- Alain Aspect (France)
- John Clauser (the U.S.)
- Anton Zeilinger (Austria)

This brings about the problem of **`local realism (局部现实主义)`** and **`principle of locality (定域性原理)`**, which is believed true in CLASSICAL mechanics or electromagnetics.

> 作业：1. 思考：科学哲学上，“真实”是如何定义的？

### 1. Newtonian Mechanics, 1687 牛顿力学

In the *Principia* writes `the first Principle`: 

$$\overrightarrow F=\frac{\mathrm d \vec p} {\mathrm dt}$$

and Newton also gives `the Law of Universal Gravitation`:

$$ \overrightarrow F = -\frac{Gm_1m_2}{r^2} \hat {\vec r} $$


### 2. Some equations

- #### Navier-Stokes equations 纳维-斯托克斯方程
$$ {\partial \vec v \over \partial t} +(\vec v \cdot \overrightarrow V) \cdot \vec v = -{1 \over \rho} \overrightarrow \nabla p + \mu \nabla^2 \vec v + \vec g$$

- #### Euler-Lagrange equation 拉格朗日方程
$${\partial L \over \partial q_\alpha}-{\mathrm d \over \mathrm dt} {\partial L \over \partial \dot q_\alpha}=0, \ L=T-V$$

- #### Hamilton Canonical Equations 哈密顿正则方程
$$
\left \{
\begin{array} {l}
\dfrac{\partial H}{\partial p_\alpha}=\dot q_\alpha \\[3ex]
\dfrac{\partial H}{\partial q_\alpha}=-\dot p_\alpha
\end{array}
\right.
$$

### 3. Schrödinger Equation 薛定谔方程

$$-{ \hbar \over 2m } \nabla ^2 \psi + U \psi =i\hbar {\partial \psi \over \partial t}$$ 

**Freeman Dyson: Four jokes by Nature**
- `the square root of minus one that the physicist Erwin Schrödinger put into his wave equation when he invented wave mechanics` 被放入薛定谔波函数的-1的平方根
- `the precise linearity of quantum mechanics, the fact that the possible states of any physical object form a linear space` 量子力学的精确线性，即物理对象的所有可能状态构成线性空间
- `the existence of quasi-crystals` 拟晶体的存在
- `a similarity in behavior between quasi-crystals and the zeros of the Riemann Zeta function` 拟晶体和黎曼$\zeta$函数在行为上的相似性


**Maxwell's equations 麦克斯韦方程组**

$$
\left \{
\begin{array} {c} 
\overrightarrow \nabla \cdot \overrightarrow E = \dfrac{\rho}{\varepsilon_0} \\[2ex]
\overrightarrow \nabla \cdot \overrightarrow E = 0 \\[2ex]
\overrightarrow \nabla \times \overrightarrow E = \dfrac{\partial B}{\partial t} \\[2ex]
\overrightarrow \nabla \times \overrightarrow B = \mu_0(\vec j+\varepsilon_0 \dfrac{\partial \overrightarrow E}{ \partial t}) \\
\end{array} 
\right.
$$

### 4. General Relativity 广义相对论

**爱因斯坦引力场方程**

$$G_{\mu v}=R_{\mu v}-{1\over2}g_{\mu v}R=\frac{4\pi G}{c^4}T_{\mu v}$$

```
Matter tells space how to curve.
Curvature tells matter how to move.
```

### 5. Time reversal: A few examples 时间反演性的一些例子

$$t \mapsto -t$$
$$\vec r \mapsto \vec r$$
$$\vec v = {\mathrm d \vec r \over \mathrm dt} \mapsto -v$$
$$\vec a = {\mathrm d \vec v \over \mathrm dt} \mapsto a$$
$$\cdots$$
$$\overrightarrow {U_d} \mapsto -\overrightarrow {U_d} $$
$$\vec j \mapsto - \vec j$$
$$\overrightarrow B \mapsto - \overrightarrow B $$

#### (1) Lagrangian 拉格朗日量

CPT invariant: 
- C: `Charge Conjugation` 电荷共轭变换
- P: `Parity` 空间反射
- T: `Time Reversal` 时间反演

We can conclude from the Maxwell equations that the Lagrangian remains invariable under CPT changes.

#### (2) Schrödinger Equation 薛定谔方程

$$\Psi(\vec r,t) \mapsto \Psi(\vec r,-t) \ \ \ \ (*)$$
$$t \mapsto -t$$
$$\mathrm i \mapsto -\mathrm i$$

It can be seen that whether the Schrödinger equation remains unchanged under time reversal depends on $(*)$.

#### (3) Euler-Lagrange equation 拉格朗日方程
The equation is $${\mathrm d \over \mathrm dt} {\partial L \over \partial \dot q_\alpha}- {\partial L \over \partial q_\alpha}=0, \ L= T - V $$ , in which $q_\alpha$ is the **generalized coordinate** (广义坐标), and $\dot q_\alpha$ is its **generalized velocity** (广义速度).

> 作业：2. 推导哈密顿正则方程 
> $$
\left \{
\begin{array} {l}
\dfrac{\partial H}{\partial p_\alpha}=\dot q_\alpha \\[3ex]
\dfrac{\partial H}{\partial q_\alpha}=-\dot p_\alpha
\end{array}
\right.
> $$
> 的时间反演不变性。



### 6. Hamilton-Jacobian equation 哈密顿-雅可比方程

$$S=  \int^{t_1}_{t_2} L \mathrm dt$$
$$ {\partial S \over \partial t}+H =0$$


## 2023/9/13 

### 1. Something about Hamilton Canonical Equations 关于哈密顿正则方程的一点讨论
The second equation can be derived to this form

$$\dot p_\alpha=-\dfrac{\partial H}{\partial q_\alpha}=-\dfrac{\partial (T+V)}{\partial q_\alpha}=-\dfrac{\partial V}{\partial q_\alpha}$$
, in which $T=\dfrac{p_\alpha ^2} {2m}$ is independent of $q_\alpha$.

This is in accordance with $F(x) = -\dfrac{\mathrm dV(x) }{\mathrm dx}$ in Newtonian mechanics.

### 2. EPR paradox EPR详谬

> 作业1：什么是EPR paradox？

Albert Einstein VS N. Bohr: The Great Debate 玻尔和爱因斯坦论战

### 3. Something about quantum mechanics 关于量子力学的一点讨论

- In 1905, Einstein, in his famous `On the Electrodynamics of Moving Bodies (论动体的电动力学)` essay, pointed out two famous postulates (假设): `length compression 尺缩现象` and `time dilation 钟慢现象`.

- Heisenberg's Uncertainty Principle: 不确定性关系/测不准原理
<br>
e.q. $$\Delta x \cdot \Delta p_x \geq {\hbar \over 2}$$
$$\Delta E \cdot \Delta t \geq {\hbar \over 2}$$
$$\Delta \tau \cdot \Delta \theta \geq {\hbar \over 2}$$

- Occam's Razor: 奥卡姆剃刀原理
<br>
Entities should not be multiplied unnecessarily. 
如无必要，勿增实体。

### 4. Newtonianism VS Darwinism 牛顿主义和达尔文主义

Newtonianism 牛顿主义:
linear (线性的), simple (简洁的), superposable (空间可叠加的)

Darwinism 达尔文主义:
non-linear (非线性的), complex (复杂的), non-superposable (空间不可叠加的)

> 作业2：康德的“二律背反”是什么？

> 作业3：了解新冠肺炎和社会达尔文主义

### 5. About the Hamiltonian operator (哈密顿算子) $\nabla$

*Hamilton 23岁就当上了正教授！要学习他！*

The notation $\nabla$ is pronounced as `del`或`nabla`.

We define $\overrightarrow \nabla$ under three-dimensional Cartesian coordinate (三维笛卡尔坐标系), the base/unit vector (基矢/单位矢量) of three orthogonal (正交的) directions being $\hat i$, $\hat j$ and $\hat k$ (also sometimes written as $\vec e_x$, $\vec e_y$ and $\vec e_z$):

$$\overrightarrow \nabla= {\partial \over \partial x}\hat i + {\partial \over \partial y}\hat j + {\partial \over \partial z}\hat k$$

Do note that this Hamiltonian operator is not the same as the one by the same name in quantum mechanics (与量子力学中的哈密顿算符做区分), which, in quantum mechanics, is $$H= -{\hbar^2 \over 2m} \nabla^2 + U.$$

Then we can define: 
#### (1) Gradient 梯度

- The gradient of a scalar becomes a vector (essentially a first-order tensor) 对标量求梯度得到矢量（其实质为一阶张量）:
<br> $$\mathrm{grad} \ \phi = \overrightarrow \nabla \phi = {\partial \phi \over \partial x}\hat i + {\partial \phi \over \partial y}\hat j + {\partial \phi \over \partial z}\hat k$$
For example: $\overrightarrow F=-\overrightarrow \nabla U$

- The gradient of a vector becomes a second-order tensor 对矢量求梯度得到二阶张量:
<br> $$\mathrm{grad} \overrightarrow A = \overrightarrow \nabla \ \overrightarrow A = ({\partial \over \partial x_i}\hat i) \otimes (A_j \hat j) = {\partial A_j \over \partial x_i} (\hat i \otimes \hat j) = \begin{bmatrix}
\dfrac{\partial A_x}{\partial x} & \dfrac{\partial A_y}{\partial x} & \dfrac{\partial A_z}{\partial x} \\[3ex]
\dfrac{\partial A_x}{\partial y} & \dfrac{\partial A_y}{\partial y} & \dfrac{\partial A_z}{\partial y} \\[3ex]
\dfrac{\partial A_x}{\partial z} & \dfrac{\partial A_y}{\partial z} & \dfrac{\partial A_z}{\partial z} \\
\end{bmatrix}$$

#### (2) Divergence 散度

$$\mathrm{div} \overrightarrow A = \overrightarrow \nabla \cdot \overrightarrow A = {\partial A_x \over \partial x} + {\partial A_y \over \partial y} + {\partial A_z \over \partial z}$$

In its essence we are performing the act of the deduction of $\overrightarrow A$ ($\overrightarrow A$的降阶) when we calculate $\mathrm{div} \overrightarrow A$.

Note that we can only calculate the divergence of **vectors**, not **scalars**.

#### (3) Curl 旋度

$$\mathrm{curl} \overrightarrow A = \overrightarrow \nabla \times \overrightarrow A = \begin{vmatrix}
\hat i & \hat j & \hat k \\[1ex]
\dfrac{\partial}{\partial x} & \dfrac{\partial}{\partial y} & \dfrac{\partial}{\partial z} \\[2ex]
A_x & A_y & A_z \\
\end{vmatrix}$$


> 作业4：证明标量的梯度无旋、矢量的旋度无散

> 作业5：把Maxwell方程组写成分量形式


#### (4) Some practice 应用

In field theory, we define $\vec r = x \hat i + y \hat j + z \hat k$.

##### ① $\vec r$ 的散度

$$\overrightarrow \nabla \cdot \vec r = ({\partial \over \partial x}\hat i + {\partial \over \partial y}\hat j + {\partial \over \partial z}\hat k) \cdot (x \hat i + y \hat j + z \hat k) = {\partial x \over \partial x} + {\partial y \over \partial y} + {\partial z \over \partial z} =3$$

##### ② The gravitational field 引力场

$$\overrightarrow \nabla r = \dfrac{\vec r}{|\vec r|} = \hat{\vec r}$$

In the gravitational field, we have $$U(r) = -{Gm_1m_2 \over r}.$$

Thus we have
$$\overrightarrow F = -\overrightarrow \nabla U = Gm_1m_2 \cdot \overrightarrow \nabla(\dfrac{1}{r}), $$
in which
$$\overrightarrow \nabla(\dfrac{1}{r})={-\overrightarrow \nabla r \over r^2}, $$
and consequently 
$$\overrightarrow F = - {G m_1 m_2 \over r^3}\vec r = - {G m_1 m_2 \over r^2} \hat {\vec r}.$$

##### ③ $\vec r$ 的梯度

$$\begin{align*}
\overrightarrow \nabla \vec r & = \overrightarrow \nabla \otimes \vec r \\
& = ({\partial \over \partial x}\hat i + {\partial \over \partial y}\hat j + {\partial \over \partial z}\hat k) \otimes (x \hat i + y \hat j + z \hat k) \\
& = {\partial x \over \partial x} (\hat i \otimes \hat i) + {\partial y \over \partial y}(\hat j \otimes \hat j)  + {\partial z \over \partial z}(\hat k \otimes \hat k)\\
& = (\hat i \otimes \hat i) + (\hat j \otimes \hat j) + (\hat k \otimes \hat k) \\
& = \underline {\underline I} \\
& = \begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{bmatrix} \\
\end{align*}$$

##### ④ The Laplacian operator 拉普拉斯算符

The Laplacian operator is linear. 拉普拉斯算符是线性算符。

Defined as: 

$$\nabla^2 = \Delta = \overrightarrow \nabla \cdot \overrightarrow \nabla = {\partial^2 \over \partial x^2} + {\partial^2 \over \partial y^2} + {\partial^2 \over \partial z^2}$$

For example, $$\nabla^2 r = \overrightarrow \nabla \cdot \overrightarrow \nabla r = \overrightarrow \nabla \cdot (\overrightarrow \nabla r) = {2 \over r}$$

> 作业6：推导上式

### 6. Discussion about some equations 关于公式的一些讨论

#### (1) Electromagnetic wave equations 电磁波方程
$$
\left \{
\begin{array} {l}
\left(\dfrac{1}{c^2} \dfrac{\partial^2}{\partial t^2}- \nabla^2\right)\overrightarrow E = \vec 0 \\[2ex]
\left(\dfrac{1}{c^2} \dfrac{\partial^2}{\partial t^2}- \nabla^2\right)\overrightarrow B = \vec 0 
\end{array}
\right.
$$
In this equation, $\Box$ 或 $\Box^2$ is called the d'Alembert or quabla operator (达朗贝尔算符), and $$\Box  =\Box^2 = \dfrac{1}{c^2} \dfrac{\partial^2}{\partial t^2}- \nabla^2.$$

This set of equation is linear, because it is derived from the linear Maxwell equations.

#### (2) Navier-Stokes Equations 纳维-斯托克斯方程

$$\rho \left({\partial \vec v \over \partial t} + (\vec v \cdot \overrightarrow \nabla ) \vec v \right) = - \overrightarrow \nabla p+\underline{\mu\nabla^2\vec v}+ \rho \vec g$$

When $t \mapsto -t $, $\vec r \mapsto \vec r$, $\overrightarrow \nabla = \dfrac{\partial}{\partial r} \mapsto \overrightarrow \nabla$, $\vec v \mapsto -\vec v$. Consequently to make this equation right, the underlined part ($\mu\nabla^2\vec v$) shall be eliminated to make `Euler's equations`:
$$\rho \left({\partial \vec v \over \partial t} + (\vec v \cdot \overrightarrow \nabla ) \vec v \right) = - \overrightarrow \nabla p+ \rho \vec g$$

> 作业7：了解什么是第5种基本力 
