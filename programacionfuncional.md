# 🧠 FICHA DE ESTUDIO – PROGRAMACIÓN FUNCIONAL Y EXPRESIONES LAMBDA

### 1. ¿Qué es la Programación Funcional?

Es un paradigma de programación donde las funciones son ciudadanos de primera clase, lo que significa que:

* Se pueden almacenar en variables.

* Se pueden pasar como parámetros.

* Se pueden devolver desde otras funciones.


En java, esto se apoya en:

* *Intefaces funcionales:* interfaces con un solo metodo abstracto (por ejemplo: ,Runnable, comparador, Predicate)

* *Expresiones lambda:* funciones anónimas y concisas que implementan una interfaz funcional.


### *¿Qué es una expresión Lambda?*
Una lambda es una forma compacta de escribir funciones anónimas. Tiene esta forma general:

```java
(parámetros) -> { cuerpo de la función }
```

Ejemplo Java:

```java
(int x, int y) -> x + y
```
---

### 3. Ejemplo en código Java. 

```java
import java.util.*;
import java.util.function.*;

public class LambdaExample {
    public static void main(String[] args) {
        // 1. Usando lambda para crear un hilo
        Runnable runnable = () -> System.out.println("Hola desde un hilo!");
        new Thread(runnable).start();

        // 2. Usando lambda con Comparator para ordenar
        List<String> nombres = Arrays.asList("Carlos", "Ana", "Pedro");
        nombres.sort((a, b) -> a.compareTo(b));
        System.out.println("Ordenados: " + nombres);

        // 3. Usando Predicate con lambda
        Predicate<Integer> esPar = num -> num % 2 == 0;
        System.out.println("¿4 es par? " + esPar.test(4)); // true

        // 4. Usando Function
        Function<String, Integer> obtenerLongitud = s -> s.length();
        System.out.println("Longitud de 'Hola': " + obtenerLongitud.apply("Hola"));
    }
}
```
--- 

### 4. ¿Cómo funciona esta estructura?

Las lambda reemplazan clases anónimas para mayor claridad y menos código.

Requieren interfaces funcionales para funcionar.

Se usan mucho en programación con colecciones (filter, map, forEach, etc.) gracias a Java Streams.

--- 

**5.** Audio 🎵  



