   
# 📦 *COLLECTIONS, JSON Y MANEJO DE DATOS*

---

### 1. **¿Por qué y para qué se utilizan?**

Las **collections** (colecciones) permiten trabajar con **grupos de datos** en Java, como listas, conjuntos o mapas.

El **manejo de datos** incluye almacenar, acceder y modificar información.

`JSON` (JavaScript Object Notation) es un formato de texto ligero que se usa para **intercambiar datos**, muy común en APIs y almacenamiento.



---

### Tipos comunes de colecciones en Java:

- `ArrayList`:  lista ordenada donde se agregan frutas con `.add()`. Permite duplicados y mantiene el orden.
- `HashSet`: conjunto que no permite duplicados. El orden no importa.
- `HashMap`: estructura clave-valor (como un diccionario). Guarda edades asociadas a nombres y permite acceder por clave.


---

### 2. **Ejemplo en Java**

```java
import java.util.*;

public class CollectionsJsonEjemplo {
    public static void main(String[] args) {
        // ArrayList
        ArrayList<String> frutas = new ArrayList<>();
        frutas.add("Manzana");
        frutas.add("Banana");
        frutas.add("Pera");
        System.out.println("Frutas: " + frutas);

        // HashSet
        HashSet<String> colores = new HashSet<>();
        colores.add("Rojo");
        colores.add("Azul");
        colores.add("Rojo"); // Ignorado (duplicado)
        System.out.println("Colores: " + colores);

        // HashMap
        HashMap<String, Integer> edades = new HashMap<>();
        edades.put("Ana", 25);
        edades.put("Luis", 30);
        System.out.println("Edad de Luis: " + edades.get("Luis"));

        // Simulación de JSON (clave-valor)
        HashMap<String, Object> persona = new HashMap<>();
        persona.put("nombre", "Carlos");
        persona.put("edad", 28);
        persona.put("activo", true);
        System.out.println("Datos JSON simulados: " + persona);
    }
}
```

 **ArrayList**

```java
ArrayList<String> frutas = new ArrayList<>();
frutas.add("Manzana");
frutas.add("Banana");
frutas.add("Pera");
System.out.println("Frutas: " + frutas);
```

🔍 **¿Qué hace?**


* Crea una lista `(ArrayList)` para guardar frutas.

* Usa `.add()` para agregar elementos.

* Imprime el contenido de la lista.

🧠 *Importante:*
* Los elementos mantienen el orden en el que se agregan.

* Se pueden repetir elementos si quieres.

---

**HashSet**


``` java
HashSet<String> colores = new HashSet<>();
colores.add("Rojo");
colores.add("Azul");
colores.add("Rojo"); // Ignorado (duplicado)
System.out.println("Colores: " + colores);
```

🔍 *¿Qué hace?*

* Crea un `HashSet`, que es una colección que no permite duplicados.

* Intenta agregar dos veces "Rojo" → solo se guarda una.

* El orden de los elementos no está garantizado.

---

**Simulación de JSON usando HashMap**

``` java
HashMap<String, Object> persona = new HashMap<>();
persona.put("nombre", "Carlos");
persona.put("edad", 28);
persona.put("activo", true);
System.out.println("Datos JSON simulados: " + persona);
```

🔍 **¿Qué hace?**

* Usa un `HashMap<String, Object>` para simular una estructura tipo JSON.

* Las claves son strings como "nombre", "edad" y "activo".

* Los valores pueden ser de distintos tipos `(String, int, boolean)` gracias al uso de Object.

 *Esto imita algo así como:*

``` java
 {
  "nombre": "Carlos",
  "edad": 28,
  "activo": true
}
```

---

####  💡Nota Explicación


// Se usan estructuras como ArrayList, HashSet y HashMap para almacenar datos de forma ordenada o estructurada.
// HashMap se puede usar para simular objetos tipo JSON, clave-valor.
// Estas colecciones son fundamentales para manejar listas, catálogos, usuarios, etc.
// Simulación de JSON: se crea un HashMap<String, Object> para representar datos como los de un objeto JSON. Las claves son strings, y los valores pueden ser texto, números o booleanos.

---
**3.** Audio 🎵