---
title: "Guía 1 - Movimiento circular, coordenadas polares, Movimiento relativo "
description: "Una forma alternativa de describir vectores es utilizando **coordenadas polares**. En este sistema, un vector r se describe mediante su magnitud r = |r| y su ángulo theta respecto a un eje de referencia que en general es el eje x."
pubDate: "April 4 2023"
heroImage: "https://www.notion.so/images/page-cover/rijksmuseum_jansz_1641.jpg"
notes: "http://materias.df.uba.ar/f1qa2020v/files/2020/02/Mec%C3%A1nica-2.pdf"
vclass: "https://youtu.be/vqIBKcEd8wQ?list=PLNbPNPgqTfs6Ec9d03-1q_dYiNjJ3WNEF"
---

# Movimientos curvilíneos

Otra forma de expresar los vectores es en base a los versores de los ejes de coordenadas. Por ejemplo, si adoptamos los ejes cartesianos $x$ e $y$, podemos expresar $\vec r = (x, y)$ como $\vec r = x \hat i + y \hat j$ donde $\hat i$ y $\hat j$ son los versores de los ejes $x$ e $y$.

![Untitled](/fisica1q/Gui%CC%81a%201%20-%20Movimiento%20circular,%20coordenadas%20polares%20e73db783c6d54edc85117c1dbf4ebd99/Untitled.png)

Una forma alternativa de describir vectores es utilizando **coordenadas polares**. En este sistema, un vector $\vec{r}$ se describe mediante su magnitud $r = |\vec r|$ y su ángulo $\theta$ respecto a un eje de referencia que en general es el eje $x$. Las coordenadas polares se pueden expresar como $\vec{r} = r\hat{r}$, donde $\hat{r}$ es un versor unitario que apunta en la dirección del vector.

![Untitled](/fisica1q/Gui%CC%81a%201%20-%20Movimiento%20circular,%20coordenadas%20polares%20e73db783c6d54edc85117c1dbf4ebd99/Untitled%201.png)

![Untitled](/fisica1q/Gui%CC%81a%201%20-%20Movimiento%20circular,%20coordenadas%20polares%20e73db783c6d54edc85117c1dbf4ebd99/Untitled%202.png)

Cuando uno observa la nueva notación $\vec{r} = r\hat{r}$, puede preguntarse donde se encuentra expresado $\theta$. Este último valor esta implícito dentro del verso $\hat r$. En la modida que $\hat r$ cambia, $\theta$ tambíen lo hace. Esto no ocuerre con las coordenadas cartesianas, donde las componentes son totalmente independientes.

![Untitled](/fisica1q/Gui%CC%81a%201%20-%20Movimiento%20circular,%20coordenadas%20polares%20e73db783c6d54edc85117c1dbf4ebd99/Untitled%203.png)

Otra dificultad con la que nos vamos a encontrar es al momento de derivar $\vec r$. En coordenadas cartesianas, derivar era algo sencillo ya que se trataba de una suma:

$$
\vec r(t) = x(t) \hat i + y(t) \hat j
$$

$$
\dot{\vec r(t)} = \dot{x(t)} \hat i + \dot{y(t)} \hat j
$$

Dado que $\hat i$ y $\hat j$ son constantes, todo quedaba en derivar $x(t)$ e $y(t)$, pero en coordenadas polares debemos derivar un producto y una función compuesta

$$
\vec{r}(t) = r(t)\hat r(t)
$$

Donde $\hat r(t)$ lo podemos expresar en coordenadas cartesianas como:

$$
\hat r(t) = \cos \theta(t) \hat i + \sin \theta(t) \hat j
$$

<aside>
🚨 Para simplificar, muchas veces se suele obviar $(t)$ y decir $\hat r = \cos \theta \hat i + \sin \theta \hat j$, dado que ya se estableció que $\theta$ varia en función del tiempo. Vamos a usar esta notación de ahora en más, pero nunca olvidar que $\theta$ es en realidad $\theta (t)$ y de hecho $\hat \theta (t) = -\sin\theta(t) \hat i + \cos \theta(t) \hat j$.

</aside>

Entonces para obtener la velocidad en coordenadas polares

$$
\vec v = \dot{\vec r} = \dot{(r \hat r)} = \dot r \hat r + r \dot{\hat r}
$$

Ahora debemos saber como derivar $\dot{\hat r}$. Para esto hay que tener en cuenta que:

$$
\dot{\hat r} = \dot{(\cos \theta \hat i + \sin \theta \hat j)} = \dot{(\cos \theta \hat i)} + \dot{(\sin \theta \hat j)}
$$

Y por tanto (recordar la regla de la cadena)

$$
\dot{\hat r} = - \dot \theta \sin \theta \hat i + \dot \theta \cos \theta \hat j = \dot \theta \hat \theta
$$

Entonces, la **velocidad** queda expresada como

$$
\vec v = \dot r \hat r + r \dot \theta \hat \theta
$$

Se puede decir que $\dot r \hat r$ representa la **velocidad radial**, mientras que $r\dot \theta \hat \theta$ representa la velocidad “en $\theta$”.

El siguiente paso es obtener $\vec a$ como la derivada de la velocidad. Para llevar adelante esta engorrosa tarea, antes vamos a calcular la derivada de $\hat \theta$

$$
\begin{split}
\dot{\hat\theta} &= \dot{(-\sin\theta\hat i)} + \dot{(\cos \theta \hat j)} \\
&=-\dot \theta \cos \theta \hat i - \dot \theta \sin \theta \hat j\\
&= -\dot \theta \hat r
\end{split}
$$

Con este resultado, tratamos de llegar a la expresión de la aceleración

$$
\begin{split}
\vec a = \dot{\vec v} &= \ddot r \hat r + \dot r \dot{\hat r} + \dot{(r\dot \theta)}\hat \theta + (r\dot\theta)\dot{\hat\theta} \\
&= \ddot r \hat r + \dot r \dot{\hat r} + (\dot r\dot\theta + r\ddot\theta)\hat\theta + (r\dot\theta)\dot{\hat\theta}\\
&= \ddot r \hat r + \dot r \dot\theta\hat\theta + (\dot r\dot\theta + r\ddot\theta)\hat\theta - (r\dot\theta)\dot\theta\hat r\\
&= \ddot r \hat r + \dot r \dot\theta\hat\theta + (\dot r\dot\theta + r\ddot\theta)\hat\theta - r\dot\theta^2\hat r\\
\vec a &= (\ddot r - r {\dot \theta}^2 )\hat r + (r \ddot \theta + 2 \dot r \dot \theta)\hat \theta
\end{split}
$$

Donde $(\ddot r - r {\dot \theta}^2 )\hat r$ es conocida como la **aceleración radial o centrípeta**, mientras que $(r \ddot \theta + 2 \dot r \dot \theta)\hat \theta$ es la aceleración en $\theta$

# Movimiento circular

Describir movimientos del tipo rectilíneos u oblicuos mediante coordenadas polares no tiene sentido en si mismo debido a su complejidad en comparación a las coordenadas cartesianas. Sin embargo, cuando el movimiento a describir es del tipo circular, la complejidad se invierte.

![Untitled](/fisica1q/Gui%CC%81a%201%20-%20Movimiento%20circular,%20coordenadas%20polares%20e73db783c6d54edc85117c1dbf4ebd99/Untitled%204.png)

Si un móvil describe un movimiento circular de radio $R$ constante, entonces $\vec r (t) = R$ es constante para todo $t$ y lo único que varia es $\theta (t)$. Hasta ahora no le prestamos mucha atención a la variación del ángulo, pero ahora tiene sentido derivarla y obtener $\omega = \dot \theta (t)$ que se conoce como **velocidad angular**.

En cuanto a las unidades, se suele usar radiantes para $\theta$ dado que si los multiplicamos por el radio del movimiento, obtenemos el arco recorrido. Dicho lo anterior, decimos que $[\omega] = \frac{rad}{s}$ aunque es muy común obviar los $rad$ y expresar sus unidades como $[\omega] = \frac{1}{s}$.

Siguiendo nuestra línea de trabajo, no tardamos en llegar al concepto de **aceleración angular** definida como $\gamma = \dot \omega = \ddot \theta$, donde $[\gamma] = \frac{1}{s^2}$.

Análogamente a lo que ya vimos, podemos definir las **ecuaciones de movimiento angular** como

$$
\theta (t) = \theta_0 + \omega_0 t + \frac{1}{2} \gamma t^2
$$

$$
\omega (t) = \omega_0 + \gamma t
$$

Dado que $|\vec r| = r = R$ es constante para todo instante de tiempo $t$, simplifica bastante las ecuaciones antes dadas para aceleración y velocidad, quedando

$$
\vec v = R\omega \hat \theta
$$

Notar que la velocidad esta definido únicamente sobre el versor $\hat \theta$ que es tangente al movimiento, razón por la cual, a esta velocidad se la llama **velocidad tangencial**.

$$
\vec a = -R\omega^2 \hat r + R \gamma \hat \theta
$$

En este caso, la aceleración posee componentes tanto en $\hat r$ versor como en $\hat \theta$ versor. A la componente en $\hat \theta$ se la conoce como **aceleración tangencial.**

Observar que la componente en $\hat r$ que llamamos **aceleración centrípeta**, es negativa, es decir, apunta hacia el centro del movimiento circular. Esta aceleración es la responsable del movimiento circular. De hecho, podemos tener una aceleración tangencial nula y aun poseer un movimiento circular. A este caso se lo conoce como **movimiento circular uniforme** (MCU) donde $\gamma = 0$ y el modulo de la velocidad tangencial es siempre constante, es decir, $\omega = \omega_0$, y la aceleración centrípeta también resulta constante $\vec a = -R {\omega_o}^2 \hat r$ .

En MCU tenemos que un objeto recorre de forma periódica la misma trayectoria con la misma velocidad (en tanto magnitud), por ende, podemos hablar de **periodo** que es el tiempo en el que un objeto completa un giro.

Al periodo de un MCU se lo simboliza con la letra $T$ y se lo puede calcular a través de $\omega_0 = \frac{2 \pi}{T}$.

Y si hablamos de periodo, podemos hablar de **frecuencia**, que se simboliza con la letra $\nu$ y representa la cantidad de giros que realiza un objeto en una unidad de tiempo. Se lo puede calcular a través de $T$ como $T = \frac{1}{\nu}$ o como $\omega_0 = 2\pi\nu$.

# Movimiento relativo

Dado dos observadores $o$ y $o\prime$, con sus propios sistemas de referencia, pueden observar a un mismo objeto y describirlo de forma distinta.

![Untitled](/fisica1q/Gui%CC%81a%201%20-%20Movimiento%20circular,%20coordenadas%20polares%20e73db783c6d54edc85117c1dbf4ebd99/Untitled%205.png)

En estos casos, lo que se suele plantear es a un observador como fijo, digamos $o$ (esto por convención) y a través de él describir al sistema de referencia de $o\prime$.

![Untitled](/fisica1q/Gui%CC%81a%201%20-%20Movimiento%20circular,%20coordenadas%20polares%20e73db783c6d54edc85117c1dbf4ebd99/Untitled%206.png)

De esta forma, podemos establecer una relación entre los observadores y el objeto observado

$$
\vec r = \vec r \prime  + \vec r_{0 0\prime}
$$

Con esto, ya podemos determinar las subsecuentes magnitudes: velocidad y aceleración

$$
\vec v = \dot{\vec r} = \dot{\vec r} \prime + \dot{\vec r_{oo \prime}} = \vec v \prime + \vec v_{oo\prime}
$$

$$
\vec a = \dot{\vec v} = \dot{\vec v} \prime + \dot{\vec v_{oo \prime}} = \vec a \prime + \vec a_{oo\prime}
$$
