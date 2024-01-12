#assignment 1 de [[Teoría de Control]]
## Sistemas lineales
Los sistemas lineales tienen la propiedad de que el output está linealmente relacionado con el input. Cambiar el input de manera linear cambiará el output de la misma forma. Entonces, si el input $x_1(t)$ genera el output $y_1(t)$ y el input $x_2(t)$ genera el output $y_2(t)$, entonces las combinaciones lineales de esos inputs producirán la combinación lineal de los outputs. El input $(x_1(t)+x_2(t))$ producirá el output $(y_1(t)+y_2(t))$. Además, el input $(a_1\cdot x_1(t)+a_2\cdot x_2(t))$ producirá el output $(a_1\cdot y_1(t)+a_2 \cdot y_2(t))$ para cualquier constantes $a_1$ y $a_2$.
En otras palabras, para un sistema $T$ sobre el tiempo $t$, compuesto de señales $x_1(t)$ y $x_2(t)$ with outputs $y_1(t)$ y $y_2(t)$,
$$T[a_{1}x_{1}(t)+a_{2}x_{2}(t)] = a_{1}T[x_{1}(t)] + a_{2}T[x_{2}(t)] = a_{1}y{1}(t)+a_{2}y_{2}(t)$$
Donde $a_1$ y $a_2$ son constantes. Igualmente, el output de un sistema linear de un input de $0$ será $0$.
## Sistemas invariantes en el tiempo
Los sistemas invariantes en el tiempo son los que el output de un input particular no cambia dependiendo de cuando ese input es aplicado. Un sistema invariante en el tiempo que toma una señal $x(t)$ y produce un output $y(t)$ también, cuando tenga como input una señal $x(t+\sigma)$, producirá el output recorrido en el tiempo $y(t+\sigma)$.
## Propiedades
Ambos sistemas, lineales y lineales invariantes en el tiempo, tiene como propiedades :
- ### Escalado lineal
![[xLy.png]]      ![[axLay.png]]
- ### Principio de superposición
![[x1x2Ly1y2.png]]
- ### Principio de superposición con escalado lineal
![[ax1bx2Lay1by2.png]]