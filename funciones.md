***
  
#  ✏️ *FUNCIONES DE STRINGS Y PRINTING*

---

### 1. **¿Por qué y para qué se utilizan?**

Las **funciones de Strings** permiten trabajar con texto: modificarlo, analizarlo o transformarlo. Son muy usadas para mostrar información, validar entradas o construir mensajes.

El **`System.out.println()`** (printing) se usa para **mostrar datos en consola**. También se puede usar `System.out.print()` (sin salto de línea).

---

### Algunas funciones comunes de `String` en Java:

- `length()`: devuelve la longitud del string.
- `toUpperCase()`: convierte a mayúsculas.
- `toLowerCase()`: convierte a minúsculas.
- `equals()`: compara si dos strings son iguales.
- `contains()`: verifica si contiene un texto.
- `substring(inicio, fin)`: extrae una parte del texto.
- `charAt(pos)`: devuelve el carácter en la posición dada.
- `replace(a, b)`: reemplaza texto.
- `trim()`: elimina espacios al inicio y al final.

---

### 2. **Ejemplo en Java**

```java
public class StringsEjemplo {
    public static void main(String[] args) {
        String mensaje = "  Hola Mundo  ";

        // Funciones de String
        System.out.println("Original: '" + mensaje + "'");
        System.out.println("Trim: '" + mensaje.trim() + "'");
        System.out.println("Longitud: " + mensaje.length());
        System.out.println("Mayúsculas: " + mensaje.toUpperCase());
        System.out.println("Minúsculas: " + mensaje.toLowerCase());
        System.out.println("¿Contiene 'Mundo'? " + mensaje.contains("Mundo"));
        System.out.println("Subcadena (0,4): " + mensaje.substring(0, 4));
        System.out.println("Carácter en posición 1: " + mensaje.charAt(1));
        System.out.println("Reemplazo de 'o' por '*': " + mensaje.replace('o', '*'));

        // Printing
        System.out.print("Este es un print ");
        System.out.println("y este es un println");
    }
}
```

---


#### 💡 Nota Explicación 

// Este ejemplo muestra cómo manipular cadenas de texto con métodos propios del tipo String.
// También se demuestra cómo imprimir información en consola usando System.out.print y println.

🔍 **¿Cuál es la diferencia?**

`System.out.print(...)`: imprime en la consola sin salto de línea al final.

`System.out.println(...)`: imprime en consola con salto de línea al final.

---


**3.** Audio 🎵