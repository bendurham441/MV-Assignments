---
header-includes: \usepackage{amsmath}
---

Ben Durham \
Multivariable Calculus

# Homework 5/7/20
p.719 #50 \
p.783 #31, 40, 48, 65 \

#### Problem \#50 \
To find the distance between a point and a plane, one find the projection of a
vector between the point and any point on the plane onto the unit normal vector
of the plane. In this case, the normal vector is simply $\langle 2, 4, -1
\rangle$ from the equation. Let A be any point on the plane.
\begin{align*}
A &= (0,0,1) \\
\overrightarrow{AP} &= \langle 2, -1, 2 \rangle \\
\hat{n} &= \frac{1}{\sqrt{21}}\langle 2, 4, -1 \rangle \\
\overrightarrow{AP} \cdot \hat{n} &= -\frac{2}{\sqrt{21}}
\end{align*}
Therefore, the distance between $P$ and the given plane is $\frac{2}{\sqrt{21}}$

#### Problem \#31 \
\begin{align*}
f(x,y) &= \sin(y^2 - xy) \\
\nabla\vec{f}(x,y) &= -y\cos(y^2 - xy)\hat{i} + (2y - x)\cos(y^2 - xy)\hat{j}
\end{align*}

#### Problem \#40 \
The directional derivative is defined as the dot product of a given unit vector
and the gradient.
\begin{align*}
f(x,y) &= x^3 - y^3 \\
\nabla\vec{f} (x,y) &= \langle 3x^2, 3y^2 \rangle \\
\vec{u} &= \langle 1, -1 \rangle \\
\hat{u} &= \frac{1}{\sqrt{2}}\langle 1, -1 \rangle \\
\nabla\vec{f}(2, -1) &= \langle 12, -3 \rangle \\
f_{\hat{u}}(2, -1) &= \nabla\vec{f}(2, -1) \cdot \hat{u} \\
f_{\hat{u}}(2, -1) &= \frac{15}{\sqrt{2}}
\end{align*}

#### Problem \#48 \
One approach to finding a vector normal to a surface such as $z^2 - 2xyz = 
x^2 + y^2$ at a given point $(1, 2, -1)$ is to rewrite the surface as if it was
the level curve of another function. Let $f(x,y,z)$ be a function
defined as follows
$$ f(x,y,z) = z^2 - 2xyz - x^2 - y^2 $$
Now, since the gradient of a function is always perpendicular to its level
curves, one need only find the gradient and evaluate it at the point in
question.
\begin{gather*}
\nabla\vec{f}(x,y,z) = (-2x - 2yz)\hat{i} + (-2y - 2xz)\hat{j} + (2z -
2xy)\hat{k} \\
\nabla\vec{f}(1,2,-1) = \langle 2, -2, -6 \rangle
\end{gather*}
As such, $\vec{n}$ will be perpendicular to the surface
$$\vec{n} = \langle 2, -2, -6 \rangle $$


#### Problem \#65 \
$$ f(x,y) = x^2e^{xy} $$
a.  One can use a normal vector and a point to construct a plane normal to a
given function. First, define a new function $g(x,y,z)$, which the given
function will be a level curve of.
\begin{gather*}
z = x^2e^{xy} \\
k = x^2e^{xy} - z \\
g(x,y,z) = x^2e^{xy} - z \\
\nabla\vec{g}(x,y,z) = (2xe^{xy} + x^2e^{xy})\hat{i} + x^3e^{xy}\hat{j} -
\hat{k} \\
\vec{n} = \nabla\vec{g}(1,0,1) = 2\hat{i} + \hat{j} - \hat{k}
\end{gather*}
By definition, the gradient of a function is perpendicular to the level curves
of that function, so now this can be used along with the given point to
construct a tangent plane.
$$ 2(x-1) + y - (z-1) = 0 $$
b.  The plane from (a) can be used to create a linearization by solving for $z$
$$ L(x,y) = z = 2x + y - 1 $$
From here, one can just plug in the point $(1,0)$.
$$ L(1, 0) = 1 $$
c.  By the definition of total differentials:
$$ df = f_x(a,b)dx + f_y(a,b)dy $$
$$ df = 2dx + dy $$



