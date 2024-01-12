# Introducción a las [[Redes Inalámbricas]]
LAN inalámbrica (WLAN), funciona bajo el estándar IEEE 802.11, este estándar **define cómo se utiliza la radio frecuencia (RF)**
Las WLAN utilizan RF, en lugar de cables. La RF tiene las siguientes características:
- La RF no tiene límites, como los límites de un cable envuelto.
- La señal RF no está protegida de señales exteriores, como sí lo está el cable en su envoltura aislante. 
### Espectro electromagnético
El espectro electromagnético está constituido por **todos los posibles niveles de energía que la luz puede tomar**, el espectro electromagnético abarca, también, todas las **longitudes de onda** que la luz puede tener, desde miles de kilómetros hasta femto-metros. 

Newton al pasar un haz de luz por un prisma de cristal hizo visible el espectro de colores que componen la luz, **demostrando que cada color representa una frecuencia de onda diferente**. Cada onda al pasar por el prisma sufría una desviación, ésta variaba según su color.

El espectro electromagnético se divide en regiones espectrales, clasificadas según los métodos necesarios para generar y detectar los diversos tipos de radiación. Es por eso que estas regiones no tienen una frontera definida y **existen algunos solapamientos entre ellas**.

La luz visible es solamente una pequeña parte del espectro electromagnético, la longitud de onda **excita la retina del sistema visual humano** produciendo sensaciones de color y brillo.
### Análisis espectral de señales
El análisis espectral tiene que ver con vibraciones y oscilaciones, las cuales, en su forma más pura, son ondulaciones sin quiebres que se repiten periódicamente a través del tiempo, manteniendo siempre la misma amplitud y frecuencia de oscilación.

Estas ondulaciones se conocen como **ondas senoidales**, y son los componentes de prácticamente todas las señales conocidas, como el ruido blanco o la voz. El análisis espectral **separa una señal en las diversas ondas** senoidales que la conforman.

### Modelo de propagación de dos rayos de una señal
Este modelo es útil para conocer la reflexión de las señales sobre la tierra, se basa en óptica geométrica. Este modelo toma en cuenta la altura de las antenas receptora  y transmisora.

La reflexión es el cambio de dirección de un rayo o una onda que ocurre en la superficie de separación entre dos medios, de tal forma que regresa al medio inicial. Ejemplos comunes son la reflexión de la luz, el sonido y las ondas en el agua. 
# Elementos de una red Inalámbrica
En las WLAN cierto es que se requiere de **elementos externos** que realicen la operación de enlace, pero hay que recordar que el aire es un medio muy difícil de controlar para estos casos y como veremos **hay factores de riesgos involucrados** con la administración de la transmisión.

> [!info] Determinantes de la seguridad de la transmisión:  
> - **La curvatura de la tierra**
> 	Se toma en cuenta debido a que en largas distancias las señales no viajarían rectas, más bien caerían en el suelo y será una perdida.
> - **Las interferencias y tiempo atmosférico**
> 	Tiempo atmosférico y las interferencias son **inevitables**, pero con un caso de estudio se evitaría graves problemas del diseño e implementación.
> - **La zona de Fresnel**
> 	Divide el espacio de enlace en zonas dándole un valor a estas, y concluye que si los obstáculos que hay entre el enlace no pasa de un 60%, la transmisión puede efectuarse.

Lo componentes mínimos y comunes, de una WLAN, se puede resumir así:
- Puente o router Wireless
- Puntos de Acceso
- PC Cards o NIC inalámbrica
- Antena y otros

## Arquitecturas de red

