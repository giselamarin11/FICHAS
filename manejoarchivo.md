# 📂 FICHA DE ESTUDIO – MANEJO DE ARCHIVOS


### 1. ¿Qué es y para qué se utiliza?
El manejo de archivos en Java permite a los programas leer información desde archivos o escribir información en ellos, como texto, datos o registros.

Esto es útil para:

Guardar información persistente (como notas, configuraciones, logs).

Cargar datos desde archivos externos (como CSV, JSON, etc.).

---

### 2. Clases principales usadas para manejo de archivos
Clase	Función principal
File	Representa un archivo o directorio
FileWriter	Escribe texto en un archivo (modo escritura)
FileReader	Lee texto de un archivo (modo lectura)
BufferedReader	Lee texto línea por línea (más eficiente)
PrintWriter	Escribe texto con formato

---

### 3. Ejemplo en código Java

```java

import java.io.*;

public class ArchivoEjemplo {
    public static void main(String[] args) {
        String nombreArchivo = "ejemplo.txt";

        // Escribir en un archivo
        try {
            FileWriter escritor = new FileWriter(nombreArchivo);
            escritor.write("Hola, este es un archivo.\nSegunda línea.");
            escritor.close();
            System.out.println("Archivo escrito con éxito.");
        } catch (IOException e) {
            System.out.println("Ocurrió un error al escribir.");
        }

        // Leer el archivo
        try {
            BufferedReader lector = new BufferedReader(new FileReader(nombreArchivo));
            String linea;
            System.out.println("Contenido del archivo:");
            while ((linea = lector.readLine()) != null) {
                System.out.println(linea);
            }
            lector.close();
        } catch (IOException e) {
            System.out.println("Ocurrió un error al leer.");
        }
    }
}
```

---

### 4. ¿Cómo funciona esta estructura?


* Se abre el archivo con la clase adecuada (FileWriter, FileReader, etc.).

* Se realiza la operación (leer o escribir).

* Siempre se cierra el archivo (.close()), para liberar recursos.

* Se maneja con try-catch para evitar errores en tiempo de ejecución (por ejemplo, si el archivo no existe).

---

**5.** Audio 🎵