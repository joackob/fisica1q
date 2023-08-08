---
title: "Guía 2 - Dinámica: Movimiento circular"
description: "Por lo que sabemos hasta ahora, cualquier cambio en la velocidad de un cuerpo se debe a la existencia de una aceleración. En el caso del movimiento circular uniforme, la velocidad se mantiene constante en tanto magnitud, pero no en cuanto a su dirección, y esto se debía a la existencia de una aceleración perpendicular al movimiento del cuerpo."
pubDate: "April 19 2023"
heroImage: "https://www.notion.so/images/page-cover/met_henri_rousseau_1907.jpg"
notes: "http://materias.df.uba.ar/f1qa2020v/files/2020/02/Mec%C3%A1nica-5.pdf"
vclass: "https://youtu.be/1WGnudQDCTE?list=PLNbPNPgqTfs6Ec9d03-1q_dYiNjJ3WNEF"
---

# Movimiento circular

Por lo que sabemos hasta ahora, cualquier cambio en la velocidad de un cuerpo se debe a la existencia de una aceleración. En el caso del movimiento circular uniforme, la velocidad se mantiene constante en tanto magnitud, pero no en cuanto a su dirección, y esto se debía a la existencia de una aceleración perpendicular al movimiento del cuerpo.

![Untitled](/fisica1q/Gui%CC%81a%202%20-%20Dina%CC%81mica%20Movimiento%20circular%20d64c06173b444f5699c7153b3fd173a3/Untitled.png)

Repasamos rápidamente las principales ecuaciones del movimiento circular. En coordenadas polares, se puede describir la posición, velocidad y aceleración de un cuerpo mediante las versores $\hat r$ y $\hat \theta$, como

$$
\vec r(t) = r\hat r
$$

$$
\vec v(t) = \dot r \hat r + r \dot \theta \hat \theta
$$

$$
\vec a(t) = (\ddot r - r {\dot \theta}^2 )\hat r + (r \ddot \theta + 2 \dot r \dot \theta)\hat \theta
$$

Donde $r$ es la distancia entre el origen de coordenadas y el objeto en cuestión.

![Untitled](/fisica1q/Gui%CC%81a%202%20-%20Dina%CC%81mica%20Movimiento%20circular%20d64c06173b444f5699c7153b3fd173a3/Untitled%201.png)

Todo esto a sabiendas de que tanto $\hat \theta$ como $\hat r$ acompañan al movimiento del cuerpo en todo instante de tiempo.

$$
\hat r(t) = \cos \theta(t) \hat i + \sin \theta(t) \hat j
$$

$$
⁍.
$$

En el caso en que el movimiento descripto por el cuerpo es **circular** de radio $R$, entonces

$$
\vec r(t)=R\hat r
$$

$$
\vec v(t) = R\dot \theta \hat \theta
$$

$$
\vec a(t) = - R\dot \theta ^2 \hat r + R\ddot \theta \hat \theta
$$

Donde $\dot \theta$ se la describe como **velocidad angular** con la letra $\omega$ y $\ddot \theta$ como **aceleración angular** con la letra $\gamma$. Esto da paso a la **ecuación para el movimiento angular** de un cuerpo.

$$
\theta (t) = \theta_0 + \omega_0 t + \frac{1}{2} \gamma t^2
$$

$$
\vec a(t) = - R\omega ^2 \hat r + R\gamma\hat \theta
$$

$$
\vec v(t) = R\omega\hat \theta
$$

Si el movimiento descripto por el cuerpo es **circular** y además **uniforme**, entonces tenemos un objeto recorre de forma periódica la misma trayectoria con la misma velocidad (en tanto magnitud), por ende, podemos hablar de **periodo** que es el tiempo en el que un objeto completa un giro.

Al periodo de un MCU se lo simboliza con la letra $T$ y se lo puede calcular a través de $\omega_0 = \frac{2 \pi}{T}$.

Y si hablamos de periodo, podemos hablar de **frecuencia**, que se simboliza con la letra $\nu$ y representa la cantidad de giros que realiza un objeto en una unidad de tiempo. Se lo puede calcular a través de $T$ como $T = \frac{1}{\nu}$ o como $\omega_0 = 2\pi\nu$.

Para MCU se simplifican aún más las ecuaciones de movimiento dadas, ya que $\gamma = 0$. Por tanto

$$
\vec a(t) = - R\omega_0 ^2 \hat r
$$

$$
\vec v(t) = R\omega_0\hat \theta
$$

La primera ecuación describe a la **aceleración centrípeta**, y la segunda a la **velocidad tangencial.** Cabe recalcar que para estos casos, la velocidad tangencial es constante en magnitud, es decir $|\vec v| = |R\omega_0\hat \theta| = |R\omega_0| = R\omega_0= v$, por lo que se puede calcular la aceleración centrípeta como

$$
\vec a(t) = - \frac{v ^2}{R} \hat r
$$

Esta aceleración es la responsable del movimiento de giro y su existencia es condición necesaria para el movimiento circular.

# Fuerzas en el movimiento circular

Si un objeto realiza un movimiento circular, entonces debe existir una fuerza que provoque la aceración, a esta se la conoce como **fuerza centrípeta.** No se trata de una fuerza nueva, se puede dar por la tensión de una cuerda, por la atracción gravitatoria o por el contacto de vías. En definitiva, cualquier fuerza o resultante de fuerzas que apunten hacia el centro de giro será la fuerza centrípeta.

Veamos un caso particular. Analicemos un aspa del rotor de cola de un helicóptero largo $R$, ¿Qué fuerzas actúan sobre el aspa? ¿Cómo actúan esas fuerzas con relación a los versores?

![Untitled](/fisica1q/Gui%CC%81a%202%20-%20Dina%CC%81mica%20Movimiento%20circular%20d64c06173b444f5699c7153b3fd173a3/Untitled%202.png)

![Untitled](/fisica1q/Gui%CC%81a%202%20-%20Dina%CC%81mica%20Movimiento%20circular%20d64c06173b444f5699c7153b3fd173a3/Untitled%203.png)

Sobre la dirección del versor $\hat r$ actúan dos fuerzas, la fuerza de vinculo del aspa y el peso. Aplicando la segunda ley de Newton, la ecuación nos queda como

$$
-T_r - P_r = -mR\omega^2
$$

En la dirección del versor $\hat \theta$ también las mismas dos fuerzas. Aplicando la segunda ley de Newton, la ecuación nos queda como

$$
T_{\theta} - P_{\theta} = mR\gamma
$$

Para que nuestro rotor de cola sea útil, es necesario que circule de forma sostenida a lo largo del tiempo, es decir que su velocidad angular sea constante. Con este datos, podemos decir que la fuerza $T$ que debe hacer el motor del rotor es igual a

$$
T_r = mR\omega_0^2 - P_r
$$

$$
T_{\theta}  = P_{\theta}
$$
