 # 🔁 *FICHA DE ESTUDIO – LOOPS / BUCLES*

 ### 1. ¿Qué son y para qué se utilizan?

Los bucles permiten repetir un bloque de código varias veces, ya sea una cantidad específica o mientras se cumpla una condición.

Son esenciales cuando necesitas:  

* Repetir tareas similares (como imprimir números del 1 al 10).

* Recorrer listas o arrays.

* Esperar que algo ocurra (como una entrada válida).

---

### Tipos De Bucles En Java:


| Tipo de Bucle | ¿Cuándo se usa?                                             |
| ------------- | ----------------------------------------------------------- |
| `for`         | Cuando conoces cuántas veces debe repetirse.                |
| `while`       | Mientras se cumpla una condición.                           |
| `do-while`    | Se ejecuta al menos una vez, y luego verifica la condición. |
| `for-each`    | Para recorrer colecciones o arrays sin usar índices.        |

 
         
   

---


### 2. **Ejemplo en Java**

```java

public class LoopExamples {
    public static void main(String[] args) {
        // Bucle for
        for (int i = 1; i <= 5; i++) {
            System.out.println("For loop: " + i);
        }

        // Bucle while
        int j = 1;
        while (j <= 3) {
            System.out.println("While loop: " + j);
            j++;
        }

        // Bucle do-while
        int k = 1;
        do {
            System.out.println("Do-while loop: " + k);
            k++;
        } while (k <= 2);

        // Bucle for-each
        String[] animals = {"Dog", "Cat", "Bird"};
        for (String animal : animals) {
            System.out.println("Animal: " + animal);
        }
    }
}
```

---


### 3. ¿Cómo funciona esta estructura?

***for:*** inicializa, evalúa condición y actualiza el valor automáticamente en cada iteración.

***while:*** evalúa la condición antes de ejecutar.

***do-while:*** ejecuta al menos una vez antes de verificar la condición.

***for-each:*** recorre todos los elementos de un array o colección.

---




**4.** Audio 🎵