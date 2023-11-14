# Advanced Mathematics

Reference: [https://www.bilibili.com/video/BV14A411C7ZE?t=5.5](https://www.bilibili.com/video/BV14A411C7ZE?t=5.5)

Reference: [https://www.bilibili.com/video/BV1JK4y1e7Ue?t=8.4](https://www.bilibili.com/video/BV1JK4y1e7Ue?t=8.4)

Reference: [https://www.bilibili.com/video/BV1GW411A73u?t=4.6](https://www.bilibili.com/video/BV1GW411A73u?t=4.6)

# 1. Limit

## 1.1 Fundamental Concepts

**Sence**

The limit of a function at a point means the value of the function when the unknowns converge infinitely to a certain point. e.g. $lim_{x\to 3}x^2+3=12$

**Left and Right Limits**

The necessary and sufficient condition for $lim_{x\to x_0}f(x)=A$ is $lim_{x\to x_0^+}f(x)=lim_{x\to x_0^-}f(x)=A$

**Relationship with Derivatives**

The rate of change of the function's values as the independent variable varies minimally and can represent the curvature at a specific point.

$$
lim_{\Delta\to 0}\frac{f(x_0+\alpha\Delta)-f(x_0+\beta\Delta)}{\Delta}=f'(x_0)(lim_{\Delta\to 0} \alpha-lim_{\Delta\to 0} \beta)
$$

## 1.2 Methods of Calculating Limits

### Common Problem Solutions

The noteworthy limit problems arise when the limit cannot be directly obtained. The most common three types of problems have different methods of approach.

**Type- $\frac{0}{0}$:** Performing substitution at the same level, e.g.

$$
lim_{x\to \infty}\frac{sin2x}{x}=lim_{x\to \infty}\frac{2x}{x}=2
$$

Common substitutions as shown in the figure below

![%E9%AB%98%E7%AD%89%E6%95%B0%E5%AD%A6%207403806347e44798b2ee2292b21e1594/Advanced_Mathematics_01.png](https://github.com/WanFengLi/Notes-for-Robotics/blob/99fb883a2d57d47c942ae102215d3b4ded277d5f/Mathematical%20Basics%20-%20%E6%95%B0%E5%AD%A6%E5%9F%BA%E7%A1%80/Advanced%20Mathematics%20-%20%E9%AB%98%E7%AD%89%E6%95%B0%E5%AD%A6/Advanced%20Mathematics%20Gallery/Advanced_Mathematics_01.png
)

**Type- $\frac{\infty}{\infty}$:** Retain only the term with the highest exponent of the variable, e.g.

$$
lim_{x\to \infty} \frac{x^{10}+x}{x^{100}+3x+5}=lim_{x\to \infty} \frac{x^{10}}{x^{100}}=lim_{x\to \infty} \frac{1}{x^{10}}=0
$$

 **Type-Infinite Power:** Applying special formula:

$$
lim_{x\to ?}Base^{Exponent}=e^{lim_{x \to ?} Exponent ×(aBase-1）}
$$

e.g.   $lim_{x\to \infty}(1+3x)^\frac{2}{x}=e^{lim_{x \to \infty}\frac{2}{x}×（1+3x-1）}=e^6$

p.s.   Its principle is derived from: $a^b=(e^{\ln a})^b=e^{b(\ln a)}$

These three types cannot cover all problems, which require more general tools.

### L'Hôpital's Rule

The limit result remains unchanged when both the numerator and denominator are simultaneously differentiated.

## 1.3 Sequence Limits and Series

### Common Sequence Patterns

The most commonly used inequality relations in the expressions of sequences are as follows.(These inequalities are often employed to replace expressions in a sequence, and then the limits are computed to determine the maximum/minimum values of the sequence.)

$$
\frac{2}{(T_1)^{-1}+(T_2)^{-1}} \le \sqrt{(T_1)×(T_2)} \le \frac{(T_1)+(T_2)}{2} \le \sqrt{\frac{(T_1)^2+(T_2)^2}{2}}
$$

By applying the same method to $a_{n+1}-a_n$, we can determine the monotonicity of the sequence and use this to judge the existence of the limit and its range.

### Squeeze Theorem

The Squeeze Theorem is one of the methods for finding the limits of specific sequences or functions. It involves manipulating a function to establish its maximum and minimum possible value: If the two limits happen to be equal, that becomes the limit of the function. For example, consider the limit $lim_{n \to \infty}(\frac{1}{\sqrt{n^2+1}}+\frac{1}{\sqrt{n^2+2}}+…+\frac{1}{\sqrt{n^2+n}})$. By making the denominators uniform, it's known that the range lies between $lim_{n \to \infty}(\frac{1}{\sqrt{n^2+1}}\cdot n)$ and $lim_{n \to \infty}(\frac{1}{\sqrt{n^2+n}}\cdot n)$. Because both limits are equal to 1, the limit of the sequence is also 1.

### ****Series and Convergence****

A series refers to a function formed by sequentially adding the terms of a sequence.

Typically, the focus in such problems lies in determining the **convergence or divergence** of the series, and the process for making this determination is as follows:

![%E9%AB%98%E7%AD%89%E6%95%B0%E5%AD%A6%207403806347e44798b2ee2292b21e1594/Advanced_Mathematics_02.png](https://github.com/WanFengLi/Notes-for-Robotics/blob/99fb883a2d57d47c942ae102215d3b4ded277d5f/Mathematical%20Basics%20-%20%E6%95%B0%E5%AD%A6%E5%9F%BA%E7%A1%80/Advanced%20Mathematics%20-%20%E9%AB%98%E7%AD%89%E6%95%B0%E5%AD%A6/Advanced%20Mathematics%20Gallery/Advanced_Mathematics_02.png)

**Conditional convergence** refers to a series that converges, but its absolute value does not. The **Absolute Convergence Theorem** states that if the absolute value of a series converges, then the original series must also converge. A common example of the conditionally convergent series is the **alternating series** (where each term alternates in sign).

# 2.Derivative

## 2.1 **Differentiation Methods**

### **Common Problem Comparison Table**

![%E9%AB%98%E7%AD%89%E6%95%B0%E5%AD%A6%207403806347e44798b2ee2292b21e1594/Advanced_Mathematics_03.png](https://github.com/WanFengLi/Notes-for-Robotics/blob/99fb883a2d57d47c942ae102215d3b4ded277d5f/Mathematical%20Basics%20-%20%E6%95%B0%E5%AD%A6%E5%9F%BA%E7%A1%80/Advanced%20Mathematics%20-%20%E9%AB%98%E7%AD%89%E6%95%B0%E5%AD%A6/Advanced%20Mathematics%20Gallery/Advanced_Mathematics_03.png)

### Implicit/Parametric Differentiation

The implicit function refers to the situation where $y(x)$ is not explicitly solved for but both $x$  and $y$ appear in the equation. In this case, differentiating both sides of the equation with respect to $x$  yields the same result.

The parametric equation is when $y(x)$ is not explicitly solved for, but $y(t)$ and $x(t)$ are known. To find the derivative, we may use the formula: $y'(x) = \frac{y'(t)}{x'(t)}$.

### **Multivariable Differentiation**

**Partial derivatives** are used in the context of multivariable functions. They represent the derivative of a function with respect to each individual independent variable. Geometrically (in the case of a bivariate function), they represent the slope of the tangent line on the surface. The partial derivative of a function $z = f(x, y)$ at the point $(x_0, y_0)$ with respect to the independent variable  $x$ is defined as the limit $lim_{\Delta x \to 0}\frac{f(x_0+\Delta x, y_0)-f(x_0, y_0)}{\Delta x}$ and is denoted as $\frac{\delta z}{\delta x}|{x=x_0, y=y_0}$ or $\frac{\delta f}{\delta x}|_{x=x_0,y=y_0}$.

The notation for **second partial derivatives** is: $\frac{\partial^2 z}{\partial x^2} = \frac{\partial (\frac{\partial z}{\partial x})}{\partial x}$ and $\frac{\partial^2 z}{\partial x\partial y} = \frac{\partial (\frac{\partial z}{\partial x})}{\partial y}$. This can be extended to higher-order derivatives.

When finding partial derivatives for implicit functions, an additional function that equals zero is introduced as representation. The derivative can be found using the formula $\frac{\partial z}{\partial x} = -\frac{\frac{\partial F}{\partial x}}{\frac{\partial F}{\partial z}}$, where $F$ is the equation representing the implicit function.

**Directional Derivatives:** If the function $z = f(x, y)$ is differentiable at a point $P(x, y)$, then the directional derivative along any direction exists (a point can have an infinite number of directional derivatives). It is defined as the limit of the increment caused by changes in the independent variables in the direction of a unit vector $\mathbf{u} = (cos\phi, sin\phi)$ as $\rho = \sqrt{(\Delta x)^2 + (\Delta y)^2}$ changes, i.e., $lim_{\Delta \rho \to 0}\frac{f(x_0+\Delta x, y_0+\Delta y)-f(x_0, y_0)}{\rho}$. Geometrically, the directional derivative $\frac{\delta f}{\delta l}$ in the direction of the unit vector $\mathbf{u}$ is given by $\frac{\delta f}{\delta x}cos\phi+\frac{\delta f}{\delta y}sin\phi$, where $\phi$ is the angle in the $x, y$ plane between the $X$-axis and the direction vector $\mathbf{u}$.

## 2.2 Applications of Derivatives

### **Basic Use Cases**

- Points where the derivative is 0 represent extrema, and extrema can be used to find the function's extreme values within an interval.
- The second derivative of a function can be used to determine the concavity (negative for convex, positive for concave).
- For multivariable functions, extremum points occur when the partial derivatives with respect to multiple independent variables are all zero. For the most common bivariate functions:
    
    Let $A = \frac{\partial^2 z}{\partial x^2}$, $B = \frac{\partial^2 z}{\partial x\partial y}$, and $C = \frac{\partial^2 z}{\partial y^2}$. We can use the following criteria to determine:
    

$$
B^2-AC =
\begin{cases}
\lt0\begin{cases}A\lt0  & \text{maxima point}\\ A \gt 0 & \text{minima point}\end{cases}\\
=0 & \text{indeterminate}\\
\gt0 & \text{non-extremum}
\end{cases}
$$

### **Concept: Gradient**

For multivariable functions, the **gradient** of a function at a certain point is the vector that points in the direction of the maximum directional derivative and has a magnitude equal to the maximum directional derivative. From a geometric perspective, the gradient of a bivariate function represents the normal vector to the contour lines.

### **Function Approximation: Taylor Series**

**Intuitive Understanding**

- Fit the trend of a function from a single point by using a polynomial that includes derivatives of all orders, aiming to closely match the complex function curve.
- Adjusting the values of lower-order derivative terms has a greater impact on the nearby fitting point, while higher-order derivative terms have a greater influence on more distant points in the future.
- The higher the order of expansion, the more accurate the function approximation and the smaller the error.

**Taylor Formula:** The $n$th order Taylor polynomial of a function $f(x)$ at $x_0$ is given by:

$$
P_n(x)=f(x_0)+f'(x_0)(x-x_0)+\frac{f''(x_0)}{2!}(x-x_0)^2+…+\frac{f^n(x_0)}{n!}(x-x_0)^n
$$

**Maclaurin Formula:** The Maclaurin formula is a special case of the Taylor formula where $x_0 = 0$ (and the last term is typically omitted when used):

$$
f(x)=f(0)+f'(0)x+\frac{f''(0)}{2!}x^2+…+\frac{f^n(0)}{n!}x^n+\frac{f^{(n+1)}(\theta x)}{(n+1)!}x^{n+1} (0\lt\theta\lt1)
$$

# 3. ** Calculus**

## **3.1 Indefinite Integration**

### **Basic Concepts**

If $a' = b$, then $\int b = a + C$.

### Table of Common Properties for Reference

![%E9%AB%98%E7%AD%89%E6%95%B0%E5%AD%A6%207403806347e44798b2ee2292b21e1594/Advanced_Mathematics_04.png](https://github.com/WanFengLi/Notes-for-Robotics/blob/99fb883a2d57d47c942ae102215d3b4ded277d5f/Mathematical%20Basics%20-%20%E6%95%B0%E5%AD%A6%E5%9F%BA%E7%A1%80/Advanced%20Mathematics%20-%20%E9%AB%98%E7%AD%89%E6%95%B0%E5%AD%A6/Advanced%20Mathematics%20Gallery/Advanced_Mathematics_04.png)

### **Substitution Method**

**Common Substitution Techniques:** Express the complex part in terms of $u$, and then replace $dx$ with $\frac{1}{u'}du$.

**Other Substitution Techniques:**

![%E9%AB%98%E7%AD%89%E6%95%B0%E5%AD%A6%207403806347e44798b2ee2292b21e1594/Advanced_Mathematics_05.png](https://github.com/WanFengLi/Notes-for-Robotics/blob/99fb883a2d57d47c942ae102215d3b4ded277d5f/Mathematical%20Basics%20-%20%E6%95%B0%E5%AD%A6%E5%9F%BA%E7%A1%80/Advanced%20Mathematics%20-%20%E9%AB%98%E7%AD%89%E6%95%B0%E5%AD%A6/Advanced%20Mathematics%20Gallery/Advanced_Mathematics_05.png)


### **Integration by Parts**

Principle: $\int U'V=UV-\int UV'$, typically applied when there is a product of terms involving $a^x$, $\sin/\cos$, $x^a$.

### **Basic Concepts**

In definite integration, the interval of integration [a, b] is fixed ($\lambda$ refers to the subinterval length, i.e., $\Delta x_i$).

$$
\int_a^b f(x)dx=lim_{\lambda \to 0}\sum_{i=1}^nf(\xi_i)\Delta x_i
$$

### **Lagrange's Mean Value Theorem**

Basic Theorem: For a function $f$ continuous on a closed interval $[a, b]$ and differentiable on the open interval $(a, b)$, there exists at least one point $\xi$ in the interval $(a, b)$ such that $f'(\xi) = \frac{f(b) - f(a)}{b - a}$.

Its extension - **Cauchy's Mean Value Theorem**: For two functions $f$ and $g$ where $g'(x) \neq 0$ for all $x$ in the open interval $(a, b)$, there exists at least one point $\xi$ such that $\frac{f'(\xi)}{g'(\xi)} = \frac{f(b) - f(a)}{g(b) - g(a)}$.

$$
F(b)-F(a)=\int_a^b f(x)dx
$$

### **Other Properties of Definite Integration**

- The properties related to addition, subtraction, and constant multiplication in indefinite integration also apply to definite integration.
- If $a < c < b$, then $\int_a^bf(x)dx = \int_a^cf(x)dx + \int_c^bf(x)dx$.
- If $f(x) \ge 0$ on the interval $[a, b]$, then $\int_a^bf(x)dx \ge 0$.

### **Variable Limits of Integration**

Variable limits of integration refer to the situation where the integration bounds are functions, and thus not completely determined. The method to handle this is:

![%E9%AB%98%E7%AD%89%E6%95%B0%E5%AD%A6%207403806347e44798b2ee2292b21e1594/Advanced_Mathematics_06.png](https://github.com/WanFengLi/Notes-for-Robotics/blob/99fb883a2d57d47c942ae102215d3b4ded277d5f/Mathematical%20Basics%20-%20%E6%95%B0%E5%AD%A6%E5%9F%BA%E7%A1%80/Advanced%20Mathematics%20-%20%E9%AB%98%E7%AD%89%E6%95%B0%E5%AD%A6/Advanced%20Mathematics%20Gallery/Advanced_Mathematics_06.png)

### **Double Integration**

The meaning of a double integral is the volume in Cartesian coordinate space. In calculations, it is usually projected onto each axis and computed sequentially, known as iterated integration, computed from right to left. Taking the projection onto the y-axis as an example, the result of the integration is as follows. (Note that the second integration may be a variable limit of integration determined by the relationship between $x$ and $y$.)

$$
\iint_Df(x,y)d\sigma=\iint_Df(x,y)dxdy=\int_a^bdy\int_{\phi_1(y)}^{\phi_2(y)}f(x,y)dx
$$

### **Applications of Definite Integration**

For a single-variable function, the definite integral is equivalent to calculating the area between the function and the x-axis over a given interval. For a bivariate function, its role is to calculate the volume. This serves as a fundamental concept for solving various mathematical problems in other applications.

## **3.3 Differentiation**

### **Total Differential**

Total differential is used for multivariable functions, and it is formed by summing up the partial differentials of each variable. For example, the total differential of a bivariate function is given by:

$$
dZ=\frac{\partial z}{\partial x}dx+\frac{\partial z}{\partial y}dy
$$

**Compound function** refers to the situation where the variable serving as the unknown in a function is itself a function of other variables. When finding the total differential of a compound function, the differential of the intermediate variable, which serves as a function, needs to be fully processed first, transformed into the differential of an independent variable, and then incorporated into the final result. It is worth noting that the derivatives of multivariable functions satisfy: $\frac{\partial^2 z}{\partial x\partial y}=\frac{\partial^2 z}{\partial y\partial x}$.

**Conditional Relationship** between differential and partial derivative: If the partial derivatives are continuous, then the function is differentiable. Conversely, if the function is differentiable, it is continuous and has continuous partial derivatives. However, the continuity of the function and the ability to compute partial derivatives do not necessarily have a causal relationship.

### **Differential Equations**

**Particular Solution and General Solution:** Differential equation problems typically involve providing an expression with multiple derivatives of the function $y$ and seeking a general solution (i.e., $y=f(x)=?$). Due to the characteristics of indefinite integration, the general solution often includes a constant term. If the values of $y$ corresponding to the certain $x$ are known, it is possible to find a particular solution.

**Solving Differential Equation:** Organizing the equation (placing $dy$, $dx$ and the corresponding unknowns on both sides of the equation) and then integrating both sides simultaneously. More advanced methods are required if this approach is not feasible(Detailed instructions refer to the video link on the top). Dealing with higher-order differential equations can be challenging, while for the condition that only three types of terms are present, it is still possible to successfully solve them through substitution or other methods.

**Types of Differential Equations**: Commonly solvable types can be categorized into **constant coefficient homogeneous differential equations** and **constant coefficient non-homogeneous differential equations**.

In this context, "homogeneous" refers to equations containing only $y$ and its multiple derivatives, without components of $x$ or constant terms. Conversely, equations that include $x$ or constant terms are termed non-homogeneous. The relationship of them is illustrated as follows:

![%E9%AB%98%E7%AD%89%E6%95%B0%E5%AD%A6%207403806347e44798b2ee2292b21e1594/Advanced_Mathematics_07.png](https://github.com/WanFengLi/Notes-for-Robotics/blob/99fb883a2d57d47c942ae102215d3b4ded277d5f/Mathematical%20Basics%20-%20%E6%95%B0%E5%AD%A6%E5%9F%BA%E7%A1%80/Advanced%20Mathematics%20-%20%E9%AB%98%E7%AD%89%E6%95%B0%E5%AD%A6/Advanced%20Mathematics%20Gallery/Advanced_Mathematics_07.png)

## **4.1 Vectors**

**Magnitude**: Regardless of dimension, the magnitude of a vector is the square root of the sum of the squares of its elements, denoted as the vector's norm.

**Dot Product**: The dot product involves multiplying corresponding elements of two vectors and summing the results (known as the inner product), resulting in a scalar. It satisfies the commutative and associative properties.

**Angle**: Regardless of dimension, the angle between vectors is determined using the formula: $\vec{a}\cdot\vec{b}=|\vec{a}|\cdot|\vec{b}|\cdot \cos\theta$. (Hence, the dot product being 0 can be used to determine if vectors are perpendicular.)

**Orthogonal**: Vectors being orthogonal means they are mutually perpendicular in space. In higher dimensions, this originates from linear independence and the inability to be expressed in terms of each other.

**Cross Product**: The result of the cross product is a vector that is orthogonal to both multiplied vectors (hence, the cross product being 0 can be used to determine if vectors are parallel). The cross-product calculation involves the use of determinants, for example, for a three-element vector:

![%E9%AB%98%E7%AD%89%E6%95%B0%E5%AD%A6%207403806347e44798b2ee2292b21e1594/Advanced_Mathematics_08.png](https://github.com/WanFengLi/Notes-for-Robotics/blob/99fb883a2d57d47c942ae102215d3b4ded277d5f/Mathematical%20Basics%20-%20%E6%95%B0%E5%AD%A6%E5%9F%BA%E7%A1%80/Advanced%20Mathematics%20-%20%E9%AB%98%E7%AD%89%E6%95%B0%E5%AD%A6/Advanced%20Mathematics%20Gallery/Advanced_Mathematics_08.png)


**Projection:** The length of the projection is calculated using the formula: $|\vec{a_{\text{proj}}}|=\frac{\vec{a}\cdot\vec{b}}{|\vec{b}|}$. If the direction needs to be considered, then the projection vector is $\vec{a_{\text{proj}}} = |\vec{a_{\text{proj}}}|\cdot\frac{\vec{b}}{|\vec{b}|}$.

## **4.2 Planes and Lines**

### **Planes**

**Equation Form**: $Ax+By+Cz+D=0$

**Parallel/Perpendicular Planes**: A plane $\pi$ is perpendicular to a vector $\vec{n}=\lbrace A,B,C\rbrace$, and the relationship between planes can be determined using their normal vectors.

**Distance from a Point to a Plane**: The distance from a point $M(x_0,y_0,z_0)$ to the plane $Ax+By+Cz+D=0$ is given by:

$$
d=\frac{|Ax_0+By_0+Cz_0+D|}{\sqrt{A^2+B^2+C^2}}
$$

### **Lines**

**Intersection Equation**: The intersection of two planes forms a system of equations, which is composed of the equation of two planes.

**Line-Plane Relationship**: If we express a line $L$ in the form of the intersection equation, then $\vec s=\lbrace A_1,B_1,C_1\rbrace \times \lbrace A_2,B_2,C_2\rbrace$ is parallel to the line.

An alternative expression for the **Equation of a Line**: If the line passes through a point $M(x_0,y_0,z_0)$ and has a direction vector $\vec s=\lbrace l,m,n\rbrace$, then the equation of the line can be expressed as:

$$
L：\frac{x-x_0}{l}=\frac{y-y_0}{m}=\frac{z-z_0}{n}
$$

**Distance from a Point to a Line**: If we know a point $M(x_0,y_0,z_0)$ and the equation of a line (along with its direction vector $\vec s=\lbrace l,m,n\rbrace$),

First, solve the system of equations:

$$
\begin{cases}
l(x-x_0)+m(y-y_0)+n(z-z_0)=0 \\
\frac{x-x_0}{l}=\frac{y-y_0}{m}=\frac{z-z_0}{n}
\end{cases}
$$

and obtain the results $x_p,y_p,z_p$. Then the distance is then given by:

$$
d=\sqrt{(x_p-x_0)^2+(y_p-y_0)^2+(z_p-z_0)^2}
$$

## **4.3 Surfaces and Curves**

### **Surfaces**

**Equation Form**: $Ax^2+By^2+Cz^2+D=0$

**Tangent Plane Equation to a Surface**: Equation of the tangent plane passing through the point $M(x_0,y_0,z_0)$

$$
F_x'(x_0,y_0,z_0)(x-x_0)+F_y'(x_0,y_0,z_0)(y-y_0)+F_z'(x_0,y_0,z_0)(z-z_0)=0
$$

**Surface Normal Equation**: Equation of the normal line passing through the point $M(x_0,y_0,z_0)$

$$
\frac{x-x_0}{F_x'(x_0,y_0,z_0)}=\frac{y-y_0}{F_y'(x_0,y_0,z_0)}=\frac{z-z_0}{F_z'(x_0,y_0,z_0)}
$$

### **Curves**

**Equation Form**: Can be represented as:

$$
\begin{cases}
x=x(t)\\ y=y(t)\\ z=z(t)
\end{cases}
$$

or written as a nonlinear system of two (surface) equations (not including $t$).

**Tangent Line to a Curve**: The equation of the tangent line passing through the point $M(x_0,y_0,z_0)$ is: $\frac{x-x(t_0)}{x'(t_0)}=\frac{y-y(t_0)}{y'(t_0)}=\frac{z-z(t_0)}{z'(t_0)}$. If it does not include $t$, then it can be written as:

$$
\frac{x-x_0}{1}=\frac{y-y_0}{y_x'(x_0)}=\frac{z-z_0}{z_x'(x_0)}
$$

**Normal Plane to a Curve**: Equation of the normal plane passing through the point $M(x_0,y_0,z_0)$:

$$
x'(t_0)[x-x(t_0)]+y'(t_0)[y-y(t_0)]+z'(t_0)[z-z(t_0)]=0
$$

$$
(x-x_0)+y_x'(x_0)(y-y_0)+z_x'(x_0)(z-z_0)=0
$$

## ****4.4 Other Common 3D Surfaces****

![%E9%AB%98%E7%AD%89%E6%95%B0%E5%AD%A6%207403806347e44798b2ee2292b21e1594/Advanced_Mathematics_09.png](https://github.com/WanFengLi/Notes-for-Robotics/blob/99fb883a2d57d47c942ae102215d3b4ded277d5f/Mathematical%20Basics%20-%20%E6%95%B0%E5%AD%A6%E5%9F%BA%E7%A1%80/Advanced%20Mathematics%20-%20%E9%AB%98%E7%AD%89%E6%95%B0%E5%AD%A6/Advanced%20Mathematics%20Gallery/Advanced_Mathematics_09.png)
