---
title: "Guía 1 - Movimientos en dos o más dimensiones"
description: "El análisis dimensional nos permite verificar la consistencia de las ecuaciones que describen el movimiento de un objeto. También nos permite identificar las unidades de medida de las variables que intervienen en las ecuaciones y expresar las soluciones en unidades apropiadas. Por ejemplo, si tenemos una ecuación que describe la velocidad de un objeto en términos de su posición y tiempo, el análisis dimensional nos permitiría verificar que la ecuación tiene unidades de longitud dividido por tiempo, lo que corresponde a unidades de velocidad."
pubDate: "Marzo 29 2023"
heroImage: "https://www.notion.so/images/page-cover/rijksmuseum_rembrandt_1642.jpg"
notes: "http://materias.df.uba.ar/f1qa2020v/files/2020/02/Mec%C3%A1nica-2.pdf"
vclass: "https://youtu.be/sJvMpt7vCrE?list=PLNbPNPgqTfs6Ec9d03-1q_dYiNjJ3WNEF"
---

# Componentes de un vector en dos dimensiones

![Untitled](/fisica1q/Gui%CC%81a%201%20-%20Movimientos%20en%20dos%20o%20ma%CC%81s%20dimensiones%202a998e55c8454632b7ac431e580ebee4/Untitled.png)

Un vector en dos dimensiones posee dos componentes: una componente horizontal y una componente vertical. La componente horizontal se denota como $A_x$ y la componente vertical se denota como $A_y$. Estas dos componentes se pueden combinar para formar el vector original mediante el teorema de Pitágoras:

$$
A^2 = A_x^2 + A_y^2


$$

Donde $A = |\vec A|$, y $\vec A$ forma un ángulo $\theta$ con relación al eje $x$. Dicho esto, las siguientes funciones trigonométricas se cumplen

$$
A_x = A \cos \theta
$$

$$
A_y = A \sin \theta
$$

$$
\tan \theta = \frac{A_y}{A_x}
$$

# Desplazamiento, velocidad y aceleración en dos dimensiones

![Untitled](/fisica1q/Gui%CC%81a%201%20-%20Movimientos%20en%20dos%20o%20ma%CC%81s%20dimensiones%202a998e55c8454632b7ac431e580ebee4/Untitled%201.png)

Ahora la trayectoria de un objeto posee mucho más interes, ya que no solo se mueve sobre una recta, sino que lo hace sobre un plano. Si proponemos a $\vec r_i$ y $\vec r_f$ como vectores de posición inicial y final correspondientemente, podemos decir que el vector $\Delta \vec r$ que une los puntos $p$ y $q$ es el vector desplazamiento, por tanto vale que:

$$
\vec r_f - \vec r_i = \Delta \vec r
$$

Dicho esto, podemos definir a la velocidad media como

$$
\vec{v}_{media} = \frac{\Delta \vec{r}}{\Delta t}
$$

Y de esta forma podemos definir

$$
\vec v = \lim_{\Delta t \rightarrow 0} \frac{\Delta \vec r}{\Delta t}
$$

$$
\vec a = \lim_{\Delta t \rightarrow 0} \frac{\Delta \vec v}{\Delta t}
$$

Ahora “acelerar” no necesariamente significa un cambio en magnitud $|\vec v| = v$, sino que puede representar un cambio en la dirección de $\vec v$. Es decir, un movimiento puede ser acelerado y mantener una velocidad constante a la vez.

Veamos un ejemplo, supongamos que un movil dobla un esquina. Tanto antes como despues de girar, su velocidad fue la misma en tanto magnitud, pero cambio su dirección debido a una aceleración perpendicular a la trayectoria del movil.

![Untitled](/fisica1q/Gui%CC%81a%201%20-%20Movimientos%20en%20dos%20o%20ma%CC%81s%20dimensiones%202a998e55c8454632b7ac431e580ebee4/Untitled%202.png)

# Movimiento de un proyectil

Si arrojamos un objeto con una velocidad inicial $\vec v_i$ que no represente una caida libre o un tiro vertical, observamos que dicha velocidad tiene componentes tanto en el eje $x$ como en el eje $y$. A este tipo de movimiento se lo conoce como **tiro oblicuo,** y es un caso más de un MRUA donde la aceleración que percibe el objeto no es otra que la gravedad.

![Untitled](/fisica1q/Gui%CC%81a%201%20-%20Movimientos%20en%20dos%20o%20ma%CC%81s%20dimensiones%202a998e55c8454632b7ac431e580ebee4/Untitled%203.png)

![Untitled](/fisica1q/Gui%CC%81a%201%20-%20Movimientos%20en%20dos%20o%20ma%CC%81s%20dimensiones%202a998e55c8454632b7ac431e580ebee4/Untitled%204.png)

Las ecuaciones para este tipo de movimiento son similares a las ecuaciones dadas para movimientos unidimensionales, solo que precisa de la descomposición de los vectores.

<aside>
💡 En las ecuaciones siguientes usamos $t$ y no $(t-t_0)$, donde podemos suponer que $t_0=0$.

</aside>

$$
\Delta \vec r = (rx, ry) =
\left\{
\begin{matrix}
rx = r_{x0} + v_{x0} t + \frac{1}{2} a_x t^2 \\ \\
ry = r_{y0} + v_{y0} t + \frac{1}{2} a_y t^2
\end{matrix}
\right.
$$

$$
\Delta \vec v = (vx, vy) =
\left\{
\begin{matrix}
vx = v_{x0} + a_x t \\ \\
vy = v_{y0} + a_y t
\end{matrix}
\right.
$$

La caída libre o el tiro vertical son simplemente casos particulares en los que la $v_x=0, a_x =0, a_y=-9,8\frac{m}{s^2}$. A la componente de la aceleración en el eje $y$ se la conoce como **aceleración de la gravedad** y se la simboliza con la letra $g$.

Entonces podemos construir las ecuaciones para tiro oblicuo:

$$
\Delta \vec r = (rx, ry) =
\left\{
\begin{matrix}
rx = r_{x0} + v_{x0} t\\ \\
ry = r_{y0} + v_{y0} t - \frac{1}{2}gt^2
\end{matrix}
\right.
$$

$$
\Delta \vec v = (vx, vy) =
\left\{
\begin{matrix}
vx = v_{x0} \\ \\
vy = v_{y0} -g t
\end{matrix}
\right.
$$

El tiro oblicuo es la composición de dos movimientos, uno en MRU con relación a las componentes en $x$ y otro en MRUA con relación a las componentes en $y$.

<aside>
💡 Cuando afirmamos que $g=-9,8 \frac{m}{s^2}$, es porque suponemos un sistema de referencia con el eje $y$ apuntando hacia arriba. Si el eje apuntase hacia abajo, claramente la gravedad cobraría una magnitud positiva.

</aside>

Lo siguiente que vamos a hacer es describir la trayectoria del objeto. Para ello, usaremos las componentes de $\Delta \vec r = (x, y)$

$$
\Delta \vec r = (x, y) =
\left\{
\begin{matrix}
x = x_0 + v_{x0} t\\ \\
y = y_0 + v_{y0} t - \frac{1}{2}gt^2
\end{matrix}
\right.
$$

Despejando $t$ de la componente $x$ obtenemos:

$$
t= \frac{\Delta x}{v_{x0}}
$$

Reemplazando t en la componente $y$ obtenemos:

$$
y = y_0 + v_{y0} \frac{\Delta x}{v_{x0}} - \frac{1}{2}g\frac{\Delta x}{v_{x0}}^2
$$

Es una parábola cóncava hacia abajo

![Untitled](/fisica1q/Gui%CC%81a%201%20-%20Movimientos%20en%20dos%20o%20ma%CC%81s%20dimensiones%202a998e55c8454632b7ac431e580ebee4/Untitled%204.png)

<aside>

💡 Si el vector $\vec v_i$ forma un ángulo $\theta$ con relación al eje $x$, entonces, podemos decir que la componente en $x, y$ de $\vec v_i$ es $v_{ix} = |\vec v_i|\cos\theta$ , $v_{iy} = |\vec v_i|\sin\theta$.

</aside>
