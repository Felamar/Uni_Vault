[[Programación Concurrente y Paralela]] #assignment 
## Java
Usando la técnica de herencia podemos crear una nueva clase llamada `factorial2` que hereda de la clase `Thread` para calcular el factorial de, en este caso, el número 10.

```java
// Declaración con herencia del objeto
// factorial2
public class factorial2 extends Thread { 
    private long myFact; // Variable que almacena el resultado del factorial

    public factorial2(){ this.myFact = 1; } // Constructor 

    @Override // Sobrecarga de la función run()
    public void run(){
        int number = 10;
        myFact = 1;
        for (int i = 1; i <= number; i++){ myFact *= i; } // Cálculo del factorial
        System.out.println("Factorial de " + number + " es: " + myFact);
    }
    
    public static void main(String[] args){
        factorial2 fact = new factorial2(); // Objeto hijo de thread
        fact.start(); // Inicia el nuevo hilo
        try{ fact.join(); } // Espera que termine el nuevo hilo
        // Muestra si hubo algun error
        catch(InterruptedException e){ e.printStackTrace(); } 
    }
}
```
## Python
Para la implementación de python sólo es necesario importar la librería `threading` para crear objetos `Thread` inicializados con un ``target`` (la función que ejecutarán) y `args` (los argumentos necesarios para la función).
#### Implementación con un sólo hilo
```python
import threading
from time import perf_counter

def factorial(n):
    fact = 1
    for i in range(1, n+1): fact *= i # i toma valores desde 1 hasta n
    print(f"El factorial de {n} es {fact}")

if __name__ == '__main__':
    number = 20
    start_time = perf_counter()
    # Crea un hilo que ejecutará la función factorial con el argumento 10
    fact = threading.Thread(target=factorial, args=(number,))
    fact.start() # Inicia el hilo
    fact.join() # Espera que termine el hilo
    print(f"Time: {perf_counter() - start_time}")
```
##### Output:
```bash
El factorial de 20 es 2432902008176640000
Time: 0.0008416999999099062
```
#### Implementación con multiples hilos
```python
import threading
from time import perf_counter

global result
result = 1

def factorial(start: int, finish: int) -> None:
    fact = 1
    [fact := fact * i for i in range(start, finish + 1)]
    global result
    result *= fact

def factorial_by_slices(number: int, threads=1) -> None:
    slice = number // threads
    ts = []
    for i in range(threads):
        start = i * slice + 1
        if i == threads - 1: finish = number
        else : finish = start + slice - 1
        thread = threading.Thread(target=factorial, args=(start, finish))
        ts.append(thread)
        
    [thread.start() for thread in ts]
    [thread.join() for thread in ts]

if __name__ == '__main__':
    number = 20
    start_time = perf_counter()
    factorial_by_slices(number, threads=2)
    end_time = perf_counter()
    print(f"El factorial de {number} es {result}")
    print(f"Time: {end_time - start_time}")
```
##### Output
```bash
El factorial de 20 es 2432902008176640000
Time: 0.000793300000623276
```
>[!TODO] To do:
>- [ ] Checar rendimiento del algoritmo más a detalle
