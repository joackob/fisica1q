---
title: "Apéndice - Ecuaciones diferenciales lineales homogéneas de segundo orden con coeficientes constantes"
description: "Apéndice - Ecuaciones diferenciales lineales homogéneas de segundo orden con coeficientes constantes"
pubDate: "April 25 2023"
heroImage: "https://www.notion.so/images/page-cover/woodcuts_9.jpg"
notes: "http://materias.df.uba.ar/f1qa2020v/files/2020/02/Mec%C3%A1nica-6.pdf"
vclass: "https://youtu.be/pggkjCHyBHI?list=PLNbPNPgqTfs6Ec9d03-1q_dYiNjJ3WNEF"
---

# Ecuaciones lineales de coeficientes constantes homogéneas

La forma general de las ecuaciones de este tipo es

$$
\ddot y + p\dot y + qy = 0 \space \text{con}\space p,q \in \R
$$

Proponemos como solución la función $y = e^{rx}$ con $r\in \R$, cuyas derivadas son de la forma $y^{(n)}(x) = r^ne^{rx}$. Con esta solución, nuestra ecuación se vería algo así:

$$
\begin{split}
r^2e^{rx} + rpe^{rx} + qe^{rx} &= 0\\
e^{rx}(r^2 + rp +q) = 0
\end{split}
$$

Se conoce como **ecuación característica** de la ecuación $\ddot y + p\dot y + qy = 0$, a la ecuación algebraica asociada

$$
r^2 + rp +q
$$

Conociendo las raíces de la ecuación característica podemos formar la solución general de la ecuación diferencial original.

### **Caso 1: Raíces reales distintas**

La ecuación característica tiene raíces reales distintas $r_1$ y $r_2$. En este caso, las bases del sistema de soluciones son

$$
e^{r_1x},e^{r_2x}
$$

Por tanto, la solución general tendrá la forma

$$
y(x) = C_1e^{r_1x} + C_2e^{r_2x}
$$

Con $C_1,C_2$ constantes.

### Caso 2: Raíces reales iguales

La ecuación característica tiene una sola raíz $r$. En este caso, las bases del sistema de soluciones son

$$
e^{rx},xe^{r_2x}
$$

Por tanto, la solución general tendrá la forma

$$
\begin{split}
y(x) &= C_1e^{rx} + C_2xe^{rx}\\
&= e^{rx}(C_1 + C_2x)
\end{split}
$$

Con $C_1,C_2$ constantes .

### Caso 3: Raíces complejas

La ecuación característica tiene raíces complejas distintas $r_1 = a + bi$ y $r_2 = a - bi$. En este caso, las bases del sistema de soluciones son

$$
e^{(a+bi)x},e^{(a-bi)x}
$$

Por tanto, la solución general tendrá la forma

$$
\begin{split}
y(x) &= C_1e^{(a+bi)x} + C_2e^{(a-bi)x}\\
&=e^{ax}( C_1e^{bix} + C_2e^{-bix})
\end{split}
$$

Usando la [expresión de Euler](https://es.wikipedia.org/wiki/F%C3%B3rmula_de_Euler)

$$
e^{ix} = \cos x + i\sin x\\
e^{-ix} = \cos x - i\sin x
$$

Podemos llegar a la siguiente expresión de la solución general

$$
y(x) = e^{ax}(D_1\cos bx + iD_2 \sin bx)
$$

Con $D_1,D_2$ constantes. Si adoptamos $G_1 = D1, G_2 = iD_2$, entonces, podemos hallar una solución general con la forma

$$
y(x) = e^{ax}(G_1\cos bx + G_2 \sin bx)
$$

Con $G_1,G_2$ constantes. Es importante notar que dada esta expresión, se puede decir que las siguientes funciones son base del sistema de soluciones

$$
e^{ax}\cos bx , e^{ax}\sin bx
$$

<aside>

💡 Determinar las constantes de cada familia dependerá de las condiciones de cada problema. Por ejemplo, $y(0) = 1, y^\prime (1) = 2$. Dadas estas condiciones, se pueden calcular las constantes mencionadas.

</aside>

<aside>

💡 Las familias que se mostraron en este artículo no son determinantes. Pueden existir más familias de soluciones. Observar que al inicio cuando se propuso a $y(x) = e^{rx}$ como base de soluciones, bien se podría tomar $y(x) = e^{rx + r\prime}$ con $r,r\prime$ constantes. Esto daría lugar a nuevas familias de soluciones aún más generales, pero con el fin de centrarse en el método, se evito esta opción.

</aside>
