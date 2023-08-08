---
title: "Guía 6 - Teoremas de conservación"
description: "Dado un sistema de $n$ partículas, tal que cada una de ellas puede o no estar sometida tanto a fuerzas externas como internas, notaremos con símbolo F_i{ext} a la resultante de las fuerzas externas que se aplican sobre la partícula $i$, mientras que f_{ij} es el símbolo que adjudicaremos a la fuerza interna que actúa sobre la partícula $i$, pero que es ejercida por la partícula $j$. Aquí debemos hacer una breve aclaración, si se llega a considerar a la partícula $j$ como una entidad no perteneciente al sistema analizado, entonces la fuerza f_{ij}, pasa a ser una fuerza externa."
pubDate: "June 17 2023"
heroImage: "https://www.notion.so/images/page-cover/met_vincent_van_gogh_oleanders.jpg"
notes: ""
vclass: "https://youtu.be/kLz682g2chc?list=PLNbPNPgqTfs6Ec9d03-1q_dYiNjJ3WNEF"
---

# Teoremas de conservación

Dado un sistema de $n$ partículas, tal que cada una de ellas puede o no estar sometida tanto a fuerzas externas como internas, notaremos con símbolo $\vec F_i^{ext}$ a la resultante de las fuerzas externas que se aplican sobre la partícula $i$, mientras que $\vec f_{ij}$ es el símbolo que adjudicaremos a la fuerza interna que actúa sobre la partícula $i$, pero que es ejercida por la partícula $j$. Aquí debemos hacer una breve aclaración, si se llega a considerar a la partícula $j$ como una entidad no perteneciente al sistema analizado, entonces la fuerza $\vec f_{ij}$, pasa a ser una fuerza externa.

Definimos también a la posición del centro de masa como

$$
\vec R_{cm} = \frac{\sum\limits_{i=1}^n m_i\vec r_i}{M}
$$

Donde $M$ es la masa total del sistema o $M=\sum\limits_{i=1}^n m_i$. De igual forma, definimos la velocidad del centro de masa como

$$
\vec V_{cm} = \frac{\sum\limits_{i=1}^n m_i\vec v_i}{M}
$$

## Teorema de conservación del impulso lineal en un sistema de partículas

La cantidad de movimiento total de un sistema de partículas se puede definir como

$$
\begin{split}
\vec p &= \sum\limits_{i=1}^n \vec p_i \\
&= \sum\limits_{i=1}^n m_i\vec v_i\\
&= MV_{cm}
\end{split}
$$

Como es sabido, para que la cantidad de movimiento se conserve, esta debe ser constante, y por tanto, su derivada tiene que ser nula.

$$
\begin{split}
\frac{d\vec p}{dt} &= \sum\limits_{i=1}^n \frac{d\vec p_i}{dt}\\
&= \sum\limits_{i=1}^n \vec (\vec F_i^{ext} + \sum\limits_{j\neq i} \vec f_{ij})\\
&= \sum\limits_{i=1}^n \vec F_i^{ext} + \sum\limits_{i=1}^n \sum\limits_{j\neq i}\vec f_{ij}
\end{split}
$$

Si observamos por un momento el segundo termino del reciente resultado, podemos ver que en la sumatoria total aparecerá tanto $\vec f_{ij}$ como su par de reacción $\vec f_{ji}$, los cuales se anulan mutuamente, dando como resultado

$$
\begin{split}
\frac{d\vec p}{dt} &= \sum\limits_{i=1}^n \vec F_i^{ext}\\
&= MA_{cm}
\end{split}
$$

<aside>

💡 Por ende, la cantidad total de movimiento de un sistema de partículas es constante, si y solo si, $\sum\limits_{i=1}^n \vec F_i^{ext} = 0$.

</aside>

Corolarios a tener en cuenta:

- La cantidad de movimiento total de un sistema de partículas se conserva, si y solo si, la velocidad del centro de masa es constante.
- La cantidad de movimiento total de un sistema de partículas es una magnitud vectorial, por lo que se puede aplicar el teorema de conservación de forma independiente a cada una de sus componentes. Por ejemplo: en un tiro oblicuo, se puede decir que la cantidad de movimiento se conserva en el eje horizontal, dado que no existen fuerzas externas que actúen en esa componente.

## Teorema de conservación de la energía en un sistema de partículas

<aside>

💡 Por defecto, se usan los términos de energía y energía mecánica como iguales. Si uno no menciona explícitamente a que tipo de energía se esta refiriendo en una oración o expresión, se puede asumir que se trata de energía mecánica.

</aside>

Para un sistema de $n$ partículas, podemos decir que la energía total del sistema esta dada por

$$
\begin{split}
E &= \sum\limits_{i=1}^n E_i\\
&= \sum\limits_{i=1}^n (E_{c_i} + E_{p_i})
\end{split}
$$

Donde $E_{c_i},E_{p_i}$ corresponden a la energía cinética y potencial de la partícula $i$. Por otro lado, sabemos que

$$
\Delta E = 0 \iff W_{nc} = 0
$$

Nuestro problema se focaliza en determinar si las fuerzas internas realizan trabajo no conservativo.

$$
\begin{split}
W_{nc} &= W_{nc}^{ext} + W_{nc}^{int}\\
dW_{nc} &= dW_{nc}^{ext} + dW_{nc}^{int}\\
&= \sum\limits_{i=1}^n \vec F_i^{ext}d\vec r_i + \sum\limits_{i=1}^n \sum\limits_{j\neq i}\vec f_{ij}d\vec r_i
\end{split}
$$

Si observamos por un momento el segundo termino del reciente resultado, podemos ver que en la sumatoria total aparecerá tanto $\vec f_{ij}$ como su par de reacción $\vec f_{ji}$, cuya relación es $\vec f_{ij} = -\vec f_{ji}$. Dicho esto, podemos acomodar nuestra sumatoria tal que podamos definir un termino $dw_i$ que sea igual a $\vec f_{ij}d\vec r_i + \vec f_{ji}d\vec r_j$.

$$
\begin{split}
dw_i &= \vec f_{ij}d\vec r_i + \vec f_{ji}d\vec r_j\\
&= \vec f_{ij}d\vec r_i - \vec f_{ij}d\vec r_j\\
&= \vec f_{ij}(d\vec r_i - d\vec r_j)\\
&= \vec f_{ij}d(\vec r_i - \vec r_j)
\end{split}
$$

Es decir que $dw_i = 0 \iff d(\vec r_i - \vec r_j) = 0$, ósea que, el trabajo realizado por los pares de acción y reacción de fuerzas internas de un sistema será cero, cuando la distancia entre las partículas que ejercen dichas fuerzas es constante.

Un cuerpo solido es un ejemplo de un sistema cuyas partículas mantienen siempre una distancia constante.

Solo en esos casos, podemos decir que al sistema solo lo afectan las fuerzas externas. En otros casos, no me queda otras que considerar el trabajo realizado por las fuerzas internas.

Por ende, en general, la energía de un sistema solo se conserva cuando

$$
\Delta E = 0 \iff W_{nc}^{ext} + W_{nc}^{int} = 0
$$

## Teorema de conservación del impulso angular en un sistema de partículas

Podemos decir que el impulso angular de un sistema de partículas visto desde un punto $o$ es

$$
\begin{split}
\vec L_o &= \sum\limits_{i=1}^n \vec L_i\\
&= \sum\limits_{i=1}^n  \vec r_i \times \vec p_i
\end{split}
$$

El impulso angular se conserva si y solo si, el torque, en este caso, del sistema de partículas es igual a cero

$$
\begin{split}
\vec M_o &= \frac{d\vec L_o}{dt}\\
&= \sum\limits_{i=1}^n \frac{d\vec L_i}{dt}\\
&= \sum\limits_{i=1}^n  \vec r_i \times \vec F_i
\end{split}
$$

Donde $\vec F_i$ son las fuerzas que afectan a la partícula $i$, ya sean internas como externas.

$$
\vec F_i = \vec F_i^{ext} + \sum\limits_{j\neq i} \vec f_{ij}
$$

Aplicamos esta expresión a la definición de torque para un sistema de partículas

$$
\begin{split}
\vec M_o &= \sum\limits_{i=1}^n  \vec r_i \times \vec F_i\\
&= \sum\limits_{i=1}^n  \vec r_i \times (\vec F_i^{ext} + \sum\limits_{j\neq i} \vec f_{ij})\\
&= \sum\limits_{i=1}^n  (\vec r_i \times \vec F_i^{ext}) +( \vec r_i \times \sum\limits_{j\neq i} \vec f_{ij})\\
&= \sum\limits_{i=1}^n  \vec r_i \times \vec F_i^{ext} + \sum\limits_{i=1}^n (\vec r_i \times \sum\limits_{j\neq i} \vec f_{ij})\\
\end{split}
$$

Si observamos por un momento el segundo termino del reciente resultado, podemos ver que en la sumatoria total aparecerá tanto $\vec f_{ij}$ como su par de reacción $\vec f_{ji}$, cuya relación es $\vec f_{ij} = -\vec f_{ji}$. Dicho esto, podemos acomodar la sumatoria tal que se generen los siguientes pares: $(\vec r_i \times \vec f_{ij}) + (\vec r_j \times \vec f_{ji})$. Si trabajamos sobre esta suma, nos aparecerá lo siguiente

$$
\begin{split}
(\vec r_i \times \vec f_{ij}) + (\vec r_j \times \vec f_{ji})
&= (\vec r_i \times \vec f_{ij}) + (\vec r_j \times -\vec f_{ij})\\
&= (\vec r_i \times \vec f_{ij}) - (\vec r_j \times \vec f_{ij})\\
&= (\vec r_i -\vec r_j) \times \vec f_{ij}\\
&= \vec r_i^\prime \times \vec f_{ij}
\end{split}
$$

Si ocurre que el vector $\vec r_i -\vec r_j$, que no es otra cosa más que la posición de la partícula $i$ visto desde la partícula $j$, es paralela a la dirección de la fuerza que ejerce la partícula $j$ sobre la partícula $i$, el producto vectorial se anula.

En dicho caso, el torque del sistema solo seria afectado por las fuerzas externas., por tanto, el impulso angular se conserva cuando

$$
\begin{split}
\vec M_o^{ext} &= 0 \iff \sum\limits_{i=1}^n  \vec r_i \times \vec F_i^{ext} = 0
\end{split}
$$

Afortunadamente, el vector $\vec r_i -\vec r_j$ suele ser paralelo al vector $\vec f_{ij},$ por lo que este último resultado puede aplicarse fácilmente.
