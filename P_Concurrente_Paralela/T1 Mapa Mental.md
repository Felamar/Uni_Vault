[[Programación Concurrente y Paralela]] #assignment
## Pipes
Una pipe es una técnica para pasar información desde un proceso o comando hacia otro. A diferencia de otras formas de comunicación interna entre procesos (IPC), una pipe se refiere a una comunicación de un solo sentido.
## Named pipes (fifo)
Una named pipe (también conocida como an FIFO por su comportamiento) es una extensión del concepto tradicional de pipe en sistemas Unix, y es uno de los métodos de comunicación inter-proceso (IPC). 
Una pipe tradicional esta "*unnamed*" y dura el mismo tiempo que el proceso. Una named pipe, sin embargo, puede permanecer mientras que el sistema esté listo, más allá de la vida del proceso. Se puede borrar si ya no se usa. Normalmente una named pipe aparece como un archivo. Dos procesos pueden hacer uso de una named pipe, uno que escribe en el archivo y el otro que lo lee.
## Colas de mensajes
Las colas de mensajes guardan "mensajes" --paquetes de data que las aplicaciones crean para que otras las consuman-- en el orden que son transmitidas hasta que una aplicación consumidora pueda procesarlas. Esto habilita el resguardo de los mensajes hasta que la aplicación receptora este lista, por si hay un problema con la red o con la aplicación, los mensajes en la cola no sean perdidos.
## Semáforos
Es una variable o un tipo de dato abstracto usado para controlar el acceso a un recurso común por múltiples hilos y evitar problemas en un sistema concurrente, como un sistema operativo de multitarea.
## Memoria compartida
Es una característica de un sistema operativo que permite a los hilos de servidor de una base de datos y a procesos compartir información por medio de conjuntos de memoria de acceso compartido.
Los servidores de bases de datos usan memoria compartida por los siguientes propósitos:
- Reducir el uso de memoria y disco I/O
- Realizar comunicación entre procesos a gran velocidad
## Sockets
El sistema operativo incluye el recurso de comunicación entre procesos (IPC) de Berkeley Software Distribution (BSD) conocido como *sockets*.
Los sockets son canales de comunicación que permiten que procesos no relacionados intercambien datos localmente y entre redes. Un único socket es un punto final de un canal de comunicación bidireccional. 
