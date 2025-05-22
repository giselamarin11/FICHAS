#  🔁 *CONTROL DE FLUJO*

---

### 1. **¿Por qué y para qué se utiliza?**

El **control de flujo** permite que un programa **tome decisiones** o **ejecute instrucciones dependiendo de condiciones**. Gracias a estas estructuras, el código puede comportarse de manera diferente según los valores que se estén manejando.

En Java, las estructuras principales son:

- `if` / `else`: ejecuta un bloque si se cumple una condición.
- `else if`: permite evaluar múltiples condiciones.
- `switch`: evalúa una variable contra varios valores posibles.



 ## if / else

Sirve para tomar decisiones en el código. Evalúa si una condición es verdadera (true) y, si lo es, ejecuta un bloque de código.

**Ejemplo:**

``` java 
int edad = 20;

if (edad >= 18) {
    System.out.println("Eres mayor de edad");
} else {
    System.out.println("Eres menor de edad");
}
```

🔍 **¿Qué pasa aquí?**
Si edad es mayor o igual a 18, se imprime "*Eres mayor de edad*".

Si no (es decir, false), se ejecuta lo que está dentro de else "*Eres menor de edad*".

---

## else if

Se usa cuando quieres evaluar varias condiciones diferentes, una tras otra.


**Ejemplo:**


``` java 
int nota = 75;

if (nota >= 90) {
    System.out.println("Excelente");
} else if (nota >= 70) {
    System.out.println("Aprobado");
} else {
    System.out.println("Reprobado");
}
```

🔍 **¿Qué pasa aquí?**

* Si la nota es 90 o más → imprime "*Excelente*".

* Si la nota no es 90 pero sí 70 o más → imprime "*Aprobado*".

* Si no se cumple ninguna → imprime "*Reprobado*".

---

## switch

Es útil cuando una variable puede tener varios valores posibles, y quieres ejecutar una acción distinta para cada uno.


``` java 
int dia = 2;

switch (dia) {
    case 1:
        System.out.println("Lunes");
        break;
    case 2:
        System.out.println("Martes");
        break;
    case 3:
        System.out.println("Miércoles");
        break;
    default:
        System.out.println("Otro día");
}
```

🔍 **¿Qué pasa aquí?**

La variable dia se compara con cada case.

* Si dia == 2, se ejecuta el bloque que imprime *"Martes".*

* El break detiene el switch después de ejecutar un case.

* Si no coincide con ningún case, se ejecuta el bloque default.


---

####  💡Nota Explicación

// El programa toma decisiones según el valor de las variables.
// if-else permite evaluar condiciones booleanas.
// switch permite ejecutar bloques según el valor de una variable.

 
Estructura ¿Cuándo usarla?

**if / else**	Para condiciones simples (verdadero/falso)
**else if**	Para evaluar varias condiciones diferentes
**switch**	Para comparar un valor específico contra varios casos

---

**3.** Audio 🎵