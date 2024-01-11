#notes
Conceptos básicos sobre la [[Teoría de Control]]
- **Variable controlada**: Es la cantidad o condición que se mide y controla. Es salida (el resultado)
- **Variable manipulada**: Es la cantidad o condición que el controlador cambia para afectar el valor de la variable controlada
- **Controlar**: Medir el valor de la variable controlada del sistema y aplica la variable manipulada al sistema para corregir o limitar una desviación del valor medido a partir de un valor deseado.
-  **Planta**: Cualquier objeto físico que se va a controlar (tal como un dispositivo mecánico, un horno de calefacción, un reactor químico, una nave espacial).
-  **Proceso**: Es cualquier operación que se va a controlar.
-  **Sistema**: Es una combinación de componentes que actúan juntos para lograr un objetivo determinado.
-  **Perturbación**: Es una señal que tiende a afectar negativamente el valor de la salida de un sistema. Si genera dentro del sistema se denomina interno, en tanto. Una perturbación externa se produce fuera del sistema y es una entrada.
-  **Control realimentado**: Se refiere a una operación en presencia de perturbaciones tiende a reducir la diferencia entre la salida de un sistema y alguna entrada de referencia y continua haciendo con base a esta diferencia.

# Objetivo
Poder manejar con una o más entrada (o referencia), una o más salidas de una planta o sistema.

# Sistema de Lazo abierto
Es un sistema en el cual la salida no afecta la acción de control.
Un ejemplo clásico de control en lazo abierto es una lavadora de ropa ya que ésta funciona durante un ciclo predeterminado sin hacer uso de sensores.

#### Lavadora
Llena -> Lava -> Enjuaga -> Exprime
Realiza un ciclo con un temporizador que inicia cuando se coloca la ropa sucia en la lavadora y termina al exprimirla.

# Sistema de lazo cerrado
Es un sistema que mantiene una relación prescrita entre la salida y la entrada de referencia. 
¿Cómo controlamos la temperatura en una habitación?

#### Variables
- Temperatura deseada
- Controlador
- Termostato
- Habitación
- Sensor
- Temperatura real

#### Ejercicio
Identificar las variables 
Crea el diagrama de bloques

# Comparación
- **Lazo abierto**:
  - Jamás se conoce la planta. 
  - No se puede usar para controlar plantas inestables.
- **Lazo cerrado**:
  - Se conoce la planta.El uso de sensores hace más caro (en dinero) el control
  - Se introduce el problema del ruido, al hacer la medición.
  
    **Ventajas**:
  - Puede controlar sistemas inestables
  - Puede controlar sistemas incluso si estos tienen errores de modelado.

# Características de los sistemas lineales invariantes en el tiempo
**Lo sistemas pueden clasificarse como**:
- Lineal
- No lineal
- Invariantes en el tiempo
- Variantes en el tiempo

- La clase de sistemas que son simultáneamente lineales e invariantes en el tiempo se denominan Sistemas Lineales Invariantes en el Tiempo (SLIT).
- Los sistemas SLIT son muy importantes porque tienen gran cantidad de aplicaciones en el procesamiento de señales.
- Su utilidad práctica proviene 
  

# Introducción
La transformada de Laplace es un operador LINEAL muy útil para la resolución de ecuaciones diferenciales.

Laplace demostró como transformar ecuaciones lineales NO HOMOGÉNEAS en ecuaciones algebraicas que pueden resolverse por medios algebraicos.

## Variable compleja
- Parte real
- Parte imaginario
- Si es una variable compleja
  - $S = \sigma + j\omega$
  - $\sigma$: Parte real
  - $\omega$: Parte imaginaria
- $F(s) = \sqrt{F(x)^2+F(y)^2}$
- $\theta = \arctan{\frac{y}{x}}$