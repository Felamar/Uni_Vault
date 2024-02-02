## a) $F(s)=\frac{1}{s+1}$
#### 1. Fracciones parciales
$$\large
Y(s)=\frac{1}{s(s+1)}=\frac{a_1}{s}+\frac{a_2}{s+1}
$$
#### 2. Cálculo de $\large a_1$
$$\large
a_1=sY(s)=\frac{1}{s+1}\bigg|_0=\frac{1}{1}=1
$$
#### 3. Cálculo de $\large a_2$
$$\large
a_2=(s+1)Y(s)=\frac{1}{s}\bigg |_{-1}=\frac{1}{-1}=-1
$$
#### 4. Sustitución de valores en $\large Y(s)$
$$\large
Y(s)=\frac{1}{s}-\frac{1}{s+1}
$$
#### 5. Cálculo de Laplace inversa de $\large Y(s)$
$$\large
\mathscr{L}^{-1}\{Y(s)\}= 1-e^{-t}
$$
---
## b) $\large F(s)=\frac{s^2}{(s+9)^2}$
#### 1. Fracciones parciales
$$\large
Y(s)=\frac{s^2}{s(s+9)^2}=\frac{a}{s}+\frac{b_1}{s+9}+\frac{b_2}{(s+9)^2}
$$
#### 2. Cálculo de $\large a$
$$\large
a=sY(s)=\frac{s^2}{(s+9)^2}\bigg|_0=\frac{0}{9^2}=0
$$
#### 3. Cálculo de $\large b_2$
$$\large
\begin{gather}
(s+9)^2Y(s)=(s+9)^2\left[\frac{b_1}{s+9}+\frac{b_2}{(s+9)^2}\right]\\[3mm]
\frac{s^2}{s}=b_1(s+9)+b_2\bigg|_{-9}\rightarrow -9=b_1(0)+b_2\\[3mm]
\boxed{b_2=-9}

\end{gather}
$$
#### 4. Calculo de $\large b_1$
$$\large
\begin{gather}
\frac{d}{ds}\frac{s^2}{s}=\frac{d}{ds}b_1(s+9)+b_2\\[3mm]
\frac{d}{ds}s=b_1(s+9)+b_2\\[3mm]
\boxed{b_2=1}
\end{gather}
$$
#### 5. Sustitución de valores en $\large {Y}(s)$ 
$$\large
Y(s)=\frac{0}{s}+\frac{1}{s+9}+\frac{-9}{(s+9)^2}
$$
#### 6. Cálculo de Laplace inversa de $\large Y(s)$
$$\large
\mathscr{L}^{-1}\{Y(s)\}=e^{-9t}-9te^{-9t}
$$
---
## c) $\large F(s)=\frac{3s+1}{(s^2+1)(s-1)}$
#### 1. Fracciones parciales
$$\large
Y(s)=\frac{3s+1}{s(s^2+1)(s-1)}=\frac{a}{s}+\frac{b}{s-1}+\frac{cs+d}{s^2+1}
$$
#### 2. Cálculo de $\large a, b, c,$ y $\large d$
##### 2.1 Despeje de cocientes
$$\large
s(s^2+1)(s-1)Y(s)=s(s^2+1)(s-1)\left[\frac{a}{s}+\frac{b}{s-1}+\frac{cs+d}{s^2+1}\right]
$$
##### 2.2 Desarrollo de cocientes
$$\large
3s+1=a[(s^2+1)(s-1)]+b[s(s^2+1)]+[cs+d][s(s-1)]
$$
$$\large
3s+1 = a[s^3-s^2+s-1]+b[s^3+s]+c[s^3-s^2]+d[s^2-s]
$$
$$\large
0s^3+0s^2+3s+1=(a+b+c)s^3+(-a-c+d)s^2+(a+b-d)s-a
$$
$$\large
\begin{aligned}
Eq.s^3:\  0&=a+b+c\\
Eq.s^2:\  0&=-a-c+d\\
Eq.s^1:\ 3&=a+b-d\\
Eq.s^0:\ 1&=-a
\end{aligned}
$$
##### 2.3 Despeje de valores
$$\large
a=-1,\quad b=2,\quad c=-1,\quad d=-2
$$
#### 3. Sustitución de valores en $\large Y(s)$
$$\large 
Y(s)=-\frac{1}{s}+\frac{2}{s-1}-\frac{s}{s^2+1}-\frac{2}{s^2+1}
$$
#### 4. Cálculo de Laplace inversa
$$\large
\mathscr{L}^{-1}\{Y(s)\}=-1+2e^t-\cos(t)-2\sin(t)
$$