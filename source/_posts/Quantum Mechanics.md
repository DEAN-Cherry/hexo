---
title: Quantum Mechanics
tag: physics
---

# Quantum Mechanics


## § 1 波函数与 Schrödinger 方程

### § 1.1 波函数的统计诠释

#### 1. 归一化条件

$$
\large\int_{(全)}|\psi(\mathbf{r})|^2\mathrm{d^3} r = 1 \qquad (\mathrm{d}^3r= \mathrm{d}x\mathrm{d}y\mathrm{d}z)
$$

和
$$
\large\int_{(全)}|\frac{1}{\sqrt{A}}\psi(\mathbf{r})|^2\mathrm{d^3} r = 1 \qquad
$$
描述的是同一个波函数



<font color = 'Lightblue'>附：高斯公式</font>
$$
\large\int_{-\infty}^{\infty} a \mathrm e^{\frac{-(x-b)^{2}}{c^{2}}} \mathrm{d} x = ac \int_{-\infty}^{\infty} \mathrm e^{-z^{2}} \,{\rm d}  z=a c \sqrt{\pi}
$$

### § 1.3 Schrödinger 方程

$$
E=h\nu=\hbar\omega=\frac{\vec{p}^2}{2m}\\
 \large P=\frac{h}{\lambda}=\hbar k
$$

$$
波函数 \quad \psi(\vec{r},t)\sim e^{i(\vec{k}\cdot \vec{r}-\omega t)}
$$

##### 1) 自由粒子的Schrödinger 方程

$$
\left\{

\begin{array}{c}
	\begin{align} 
	&\left.
		\begin{array}{}

    \frac{\partial\psi}{\partial t}=-i\omega\psi(\vec{r},t) &=-i\frac{E}{\hbar}\psi(\vec{r},t)\\ 
    \nabla^2\psi(\vec{r}, t)=-k^2\psi(\vec{r},t) &=-\frac{p^2}{\hbar^2}\psi(\vec{r},t) 
    
		\end{array}
 	\right\}
 	
 	\qquad \Longrightarrow \qquad \underbrace{ i\hbar\frac{\partial}{\partial{t}}\psi(\vec{r},t)=-\overbrace{\frac{\hbar^2}{2m}}^\text{动能}\nabla^2_{(r)}\psi(\vec r, t) }_\text{自由粒子的薛定谔方程}
 	
 	\\
    &E=\frac{p^2}{2m}
	\end{align}
\end{array}
\right.
$$

对于自由粒子的Schrödinger 方程，解析求解非常有限。可以解析解的H、He原子.

<font color = 'Lightblue'>此方程表明只要知道初始波函数，就可以知道此后任意时刻的波函数.</font>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          

##### 2) 势场${V(\vec{r},t)}$中的Schrödinger 方程

$$
\mathrm i\hbar\frac{\partial}{\partial t}\psi(\vec r,t)=\overbrace{[-\frac{\hbar^2}{2m}\nabla^2 + V(\vec r,t)]}^\text{动能+势能}\psi(\vec r,t)=\hat H\psi(\vec r,t)
$$

<font color = 'lightblue'> $\large \hat H = -\frac{\hbar^2}{2m}\nabla^2+V(\boldsymbol r) \qquad\hat H$是体系的Hamilton算符</font>

##### 3) 定态的Schrödinger 方程

若$V(\boldsymbol r)$与t无关，可以采用分离变量
$$
\large\psi(\boldsymbol r,t) = \psi(\boldsymbol r)f(t)
$$

$$
\large \frac{(-\frac{\hbar^2}{2m} \nabla^2 + V)\psi(\boldsymbol r)}{\psi(\boldsymbol r)}=\frac{\mathrm i \hbar \frac{\partial f(t)}{\partial t}}{f(t)}=E
$$
对于$f(t)$，有
$$
\mathrm i \hbar \frac{\mathrm d f(t)}{f(t)}=E\mathrm dt \quad \Longrightarrow \quad f(t)=C\mathrm e^{-\frac{\mathrm i}{\hbar}Et}
$$

$$
\psi(\boldsymbol r,t) = \psi(\boldsymbol r)f(t)=\psi(\boldsymbol r)e^{-\frac{\mathrm i}{\hbar}Et}
$$

对于$\psi(\boldsymbol r)$，则有
$$
(-\frac{\hbar^2}{2m} \nabla^2 + V)\psi(\boldsymbol r) = E\psi(\boldsymbol r)\quad \Longrightarrow \quad
\hat H\psi(\boldsymbol r) =E\psi(\boldsymbol r) \tag{*}
$$

###### 定态性质

粒子在空间中几率密度与时间无关 $psi(\boldsymbol r,t) = \psi(\boldsymbol r)f(t)=\psi(\boldsymbol r)e^{-\frac{\mathrm i}{\hbar}Et}$ 
$$
\rho_ n(\boldsymbol r,t)=|\psi(\boldsymbol r,t)|^2=|\psi(\boldsymbol r)|^2 \tag{与t无关}
$$

<font  color = 'Lightblue'>判断条件：</font>

① 能量是否为定值

② 几率是否与时间无关

### § 2 一维势场中的粒子

#### § 2.1 一维势场中粒子能量本征态的一般性质

- ##### 定理 1：

  设 $\psi^*(x)$ 是方程 ( \* ) 的一个解，对应的能量本征值为 $E$,  $\psi^*(x)$ 也是方程 (\*) 的一个解，对应的能量也为 $E$

  <font color = 'Lightblue'>推论：</font>假设对应于能量的某个本征值 $E$，方程 (*) 的解无简并 (即只有一个独立的解)，则可取为实解 

