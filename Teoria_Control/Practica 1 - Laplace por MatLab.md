## a) $f(t)=e^{t+7}$
---
#### 1. Definición de la integral de Laplace
$$\large
\mathscr{L}\{e^{t+7}\}
=\int^{\infty}_{0}e^{-(s-1)t+7}\ dt
$$
#### 2. Integración por cambio de variable
$$\large
\mathscr{L}\{e^{t+7}\}

=-\frac{1}{s-1}e^{-(s-1)t+7}\bigg|^\infty_0
$$
#### 3. Evaluación
$$\large
\mathscr{L}\{e^{t+7}\}
=-\frac{1}{s-1}\left[0-e^7\right]
=\boxed{\frac{e^7}{s-1}}
$$
## b) $f(t)=te^{4t}$
---
#### 1. Definición de la integral de Laplace
$$\large
\mathscr{L}\{te^{4t}\}
=\int^{\infty}_{0}e^{-(s-4)t}t\ dt
$$
#### 2. Integración por partes
$$\large
\mathscr{L}\{te^{4t}\}
=-\frac{1}{s-4}e^{-(s-4)t}t\bigg|^\infty_0
+\frac{1}{s-4}\int^\infty_0e^{-(s-4)t}\ dt
$$
#### 3. Evaluación 
$$\large
\mathscr{L}\{te^{4t}\}
=-\frac{1}{s-4}[0-0]
+\frac{1}{s-4}\int^\infty_0e^{-(s-4)t}\ dt
$$
#### 4. Simplificación
$$\large
\mathscr{L}\{te^{4t}\}
=\frac{1}{s-4}\int^\infty_0e^{-(s-4)t}\ dt
$$
#### 5. Integración por cambio de variable
$$\large
\mathscr{L}\{te^{4t}\}
=\frac{1}{s-4}\left[-\frac{1}{s-4}e^{-(s-4)t}\bigg|^\infty_0\right]
$$
#### 6. Evaluación 
$$\large
\mathscr{L}\{te^{4t}\}
=\frac{1}{s-4}\left[-\frac{1}{s-4}(0-1)\right]
=\boxed{\frac{1}{(s-4)^2}}
$$
## c) $f(t)=e^{-t}\sin(t)$
---
$$\large
\mathscr L\left\{e^{-t}\sin(t)\right\}
$$
#### 1. Definición de la integral de Laplace
$$\large
\mathscr L\left\{e^{-t}\sin(t)\right\}
=\int^{\infty}_0e^{-(s+1)t}\sin(t)\ dt
$$
#### 2. Integración por partes
$$\large
\mathscr L\left\{e^{-t}\sin(t)\right\}
=-\frac{1}{s+1}e^{-(s+1)t}\sin(t)\bigg|^\infty_0
+\frac{1}{s+1}\int^{\infty}_0e^{-(s+1)t}\cos(t)\ dt
$$
#### 3. Evaluación
$$\large
\mathscr L\left\{e^{-t}\sin(t)\right\}
=\frac{1}{s+1}\int^{\infty}_0e^{-(s+1)t}\cos(t)\ dt
$$
#### 4. Integración por partes
$$\large
\mathscr L\left\{e^{-t}\sin(t)\right\}
=\frac{1}{s+1}\left[
-\frac{1}{s+1}e^{-(s+1)t}\cos(t)\bigg|^\infty_0
-\frac{1}{s+1}\int^{\infty}_0e^{-(s+1)t}\sin(t)\ dt
\right]
$$
#### 5. Evaluación
$$\large
\mathscr L\left\{e^{-t}\sin(t)\right\}
=\frac{1}{(s+1)^2}
-\frac{1}{(s+1)^2}\int^{\infty}_0e^{-(s+1)t}\sin(t)\ dt
$$
#### 6. Definición y agrupamiento de valores
$$\large
1+\frac{1}{(s+1)^2}\int^{\infty}_0e^{-(s+1)t}\sin(t)\ dt
=\frac{1}{(s+1)^2}
$$
#### 7. Simplificación
$$\large
\int^{\infty}_0e^{-(s+1)t}\sin(t)\ dt
=\frac{1}{(s+1)^2}\times\frac{(s+1)^2}{(s+1)^2+1}
=\boxed{\frac{1}{(s+1)^2+1}}
$$
## d) $f(t)=t\cos(t)$
---
#### 1. Sustitución de la formula de Euler
$$\large
\mathscr{L}\{t\cos(t)\}
=\mathscr{L}\left\{\frac{e^{it}+e^{-it}}{2}t\right\}
$$
#### 2. Aplicación de propiedades
$$\large
\mathscr{L}\{t\cos(t)\}
=\frac12\left[
\mathscr{L}\left\{e^{it}t\right\}
+\mathscr{L}\left\{e^{-it}t\right\}
\right]
$$
#### 3. Sustitución de valores conocidos
$$\large
\mathscr{L}\{t\cos(t)\}
=\frac12\left[
\frac{1}{(s-i)^2} + \frac{1}{(s+i)^2}
\right]
$$
#### 4. Desarrollo
$$\large
\begin{aligned}
\mathscr{L}\{t\cos(t)\}
&=\frac12\left[
\frac{(s+i)^2+(s-i)^2}{(s^2-i^2)^2} 
\right]\\[2mm]
&=\frac12\left[
\frac{s^2+2si+i^2+s^2-2si+i^2}{(s^2-i^2)^2} 
\right]\\[2mm]
&=\frac12\left[
\frac{2s^2+2i^2}{(s^2-i^2)^2}
\right]
\end{aligned}
$$
#### 5. Simplificación
$$\large
\mathscr{L}\{t\cos(t)\}
=\frac{s^2+i^2}{(s^2-i^2)^2}=\boxed{\frac{s^2-1}{(s^2+1)^2}}
$$
## e) $f(t)=2t^4$
---
#### 1. Aplicación de propiedades
$$\large
\mathscr{L}\{2t^4\}=2\mathscr{L}\{t^4\}
$$
#### 2. Sustitución de valores conocidos
>[!info] $$\large\mathscr{L}\{t^n\}=\frac{n!}{s^{n+1}}$$

$$\large
2\mathscr{L}\{t^4\}=2\frac{24}{s^5}=\boxed{\frac{48}{s^5}}
$$
## f) $f(4t-10)$
---
#### 1. Aplicación de propiedades
$$\large
\mathscr{L}\{4t-10\}
=4\mathscr{L}\{t\}-\mathscr{L}\{10\}
$$
#### 2. Sustitución de valores conocidos
$$\large
\mathscr{L}\{4t-10\}=\boxed{\frac{4}{s^2}-\frac{10}{s}}
$$
## g) $f(t)=t^2+6t-3$
---
#### 1. Aplicación de propiedades
$$\large
\mathscr{L}\{t^2+6t-3\}
=\mathscr{L}\{t^2\}+6\mathscr{L}\{t\}-\mathscr{L}\{3\}
$$
#### 2. Sustitución de valores conocidos
$$\large
\mathscr{L}\{t^2+6t-3\}=\frac{2}{s^3}+\frac{6}{s^2}-\frac{3}{s}=\boxed{\frac{-3s^2+6s+2}{s^3}}
$$
## h) $f(t)=(t+1)^3$
---
#### 1. Desarrollo
$$\large
\mathscr{L}\{(t+1)^3\}=\mathscr{L}\{t^3+3t^2+3t+1\}
$$
#### 2. Aplicación de propiedades
$$\large
\mathscr{L}\{(t+1)^3\}=\mathscr{L}\{t^3\}+3\mathscr{L}\{t^2\}+3\mathscr{L}\{t\}+\mathscr{L}\{1\}
$$
#### 3. Sustitución de valores conocidos
$$\large
\mathscr{L}\{(t+1)^3\}=\frac{6}{s^4}+\frac{6}{s^3}+\frac{3}{s^2}+\frac{1}{s}=\boxed{\frac{s^3+3s^2+6s+6}{s^4}}
$$
## i) $f(t)=1+e^{4t}$
---
#### 1. Aplicación de propiedades
$$\large
\mathscr{L}\{1+e^{4t}\}
=\mathscr{L}\{1\}+\mathscr{L}\{e^{4t}\}
$$
#### 2. Sustitución de valores conocidos
$$\large
\mathscr{L}\{1+e^{4t}\}=\frac{1}{s}+\int^\infty_0e^{-(s-4)t}\ dt
$$
#### 3. Integración por cambio de variable
$$\large
\mathscr{L}\{1+e^{4t}\}
=\frac{1}{s}-\frac{1}{s-4}e^{-(s-4)t}\bigg|^\infty_0
$$
#### 4. Evaluación
$$\large
\mathscr{L}\{1+e^{4t}\}
=\frac{1}{s}-\frac{1}{s-4}\left[0-1\right]=\boxed{\frac{1}{s}+\frac{1}{s-4}}
$$
## j) $f(t)=(1+e^{2t})^2$
---
#### 1. Desarrollo
$$\large
\mathscr{L}\{(1+e^{2t})^2\}=\mathscr{L}\{e^{4t}+2e^{2t}+1\}
$$
#### 2. Aplicación de propiedades
$$\large
\mathscr{L}\{(1+e^{2t})\}
=\mathscr{L}\{e^{4t}\}+2\mathscr{L}\{e^{2t}\}+\mathscr{L}\{1\}
$$
#### 3. Sustitución de valores conocidos
$$\large
\mathscr{L}\{(1+e^{2t})\}
=\boxed{\frac{1}{s-4}+\frac{2}{s-2}+\frac{1}{s}}
$$
#### k) $f(t)=4t^2-5\sin(3t)$
---
#### 1. Aplicación de propiedades
$$\large
\mathscr{L}\{4t^2-5\sin(3t)\}
=4\mathscr{L}\{t^2\}-5\mathscr{L}\{\sin(3t)\}
$$
#### 2. Sustitución de valores conocidos
$$\large
\mathscr{L}\{4t^2-5\sin(3t)\}
=\frac{8}{s^3}-5\int^{\infty}_0e^{-st}\sin(3t)\ dt
$$
#### 3. Resolviendo $\int^{\infty}_0e^{-st}\sin(3t)\ dt$ 
$$\large
\int^{\infty}_0e^{-st}\sin(3t)\ dt
= -\frac{1}{s}e^{-st}\sin(3t)\bigg|^\infty_0
+\frac{3}{s}\int^{\infty}_0e^{-st}\cos(3t)\ dt
$$
#### 4. Evaluación
$$\large
\int^{\infty}_0e^{-st}\sin(3t)\ dt
= \frac{3}{s}\int^{\infty}_0e^{-st}\cos(3t)\ dt
$$
#### 5. Integración por partes
$$\large
\int^{\infty}_0e^{-st}\sin(3t)\ dt
= \frac{3}{s}\left[-\frac{1}{s}e^{-st}\cos(3t)\bigg|^\infty_0
-\frac{3}{s}\int^{\infty}_0e^{-st}\sin(3t)\ dt
\right]
$$
#### 6. Evaluación
$$\large
\int^{\infty}_0e^{-st}\sin(3t)\ dt
= \frac{3}{s^2}
-\frac{9}{s^2}\int^{\infty}_0e^{-st}\sin(3t)\ dt
$$
#### 7. Agrupación de valores
$$\large
\frac{s^2+9}{s^2}\int^{\infty}_0e^{-st}\sin(3t)\ dt
= \frac{3}{s^2}
$$
#### 8. Simplificación
$$\large
\int^{\infty}_0e^{-st}\sin(3t)\ dt
= \frac{3}{s^2}\times \frac{s^2}{s^2+9}={\frac{3}{s^2+9}}
$$
#### 9. Sustituyendo en 2
$$\large
\mathscr{L}\{4t^2-5\sin(3t)\}
=\frac{8}{s^3}-5\frac{3}{s^2+9}=\boxed{\frac{8}{s^3}-\frac{15}{s^2+9}}
$$
## l) $f(t)=\sinh(kt)$
---
#### 1. Definición del seno hiperbólico
$$\large
\mathscr{L}\{\sinh(kt)\}
=\mathscr{L}\left\{
\frac{e^{kt}-e^{-kt}}{2}
\right\}
$$
#### 2. Aplicación de propiedades
$$\large
\mathscr{L}\{\sinh(kt)\}
=\frac{1}{2}\left[\mathscr{L}\{e^{kt}\}-\mathscr{L}\{e^{-kt}\}\right]
$$
#### 3. Sustitución de valores conocidos
$$\large
\mathscr{L}\{\sinh(kt)\}
=\frac{1}{2}\left[
\frac{1}{s-k}-\frac{1}{s+k}
\right]
$$
#### 4. Desarrollo
$$\large
\mathscr{L}\{\sinh(kt)\}
=\frac{s+k-s+k}{2(s^2-k^2)}=\boxed{\frac{k}{s^2-k^2}}
$$
## m) $f(t)=e^t\sinh(t)$
#### 1. Definición del seno hiperbólico
$$\large
\mathscr{L}\{e^t\sinh(t)\}
=\mathscr{L}\left\{
e^t\left(
\frac{e^t-e^{-t}}{2}
\right)
\right\}
=\frac12\mathscr{L}\{e^{2t}-e^{0}\}
$$
#### 2. Sustitución de valores conocidos
$$\large
\large
\mathscr{L}\{e^t\sinh(t)\}
=\frac12\left[
\frac{1}{s-2}-\frac1s
\right]
$$
#### 3. Simplificación
$$\large
\large
\mathscr{L}\{e^t\sinh(t)\}
=\frac12\left[
\frac{s-s+2}{s^2-2s}
\right]
=\boxed{\frac{1}{s^2-2s}}
$$
