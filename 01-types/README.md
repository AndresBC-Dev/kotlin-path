# Tipos en Kotlin

## Los tipos en Kotlin me parecen mucho más sencillos y fáciles de trabajar que en Java, al no haber una gran diferencia entre el primitivo, el wrapper u objeto y demás.

## Algo importante de los tipos en Kotlin es la mutabilidad e inmutabilidad.
La declaración de variables se consigue con **val** para variables inmutables y **var** para mutables.

## Tipos básicos
1. **String**: Los strings son cadenas de texto, como en cualquier otro lenguaje. **Ejemplo**: `val name: String = "Andres"` 📝
2. **Int**: Los Int son números enteros. **Ejemplo**: `var edad: Int = 26` (Nota: no es necesario el `;` en Kotlin, pero para hacer un punto aparte no está mal. Queremos que `edad` sea mutable porque puede cambiar). 🔢
3. **Double**: Los Double son números flotantes o decimales. **Ejemplo**: `var estatura: Double = 1.81` 📏
4. **Boolean**: Los booleanos son valores verdadero o falso. **Ejemplo**: `var vivo: Boolean = true` ✅
5. **Char**: Los char son tipos de un solo carácter. **Ejemplo**: `val firstLetter: Char = 'A'` 🔤

### Comparación con Java
En Java, hay una distinción entre tipos primitivos y sus clases de envoltura (por ejemplo, `int` y `Integer`). Esto puede llevar a problemas de autoboxing y unboxing. En Kotlin, no hay tal distinción, lo que simplifica el manejo de tipos.

### Ejemplo de Código en Kotlin
```kotlin
fun main() {
    val name: String = "Andres"
    var edad: Int = 26
    var estatura: Double = 1.81
    var vivo: Boolean = true
    val firstLetter: Char = 'A'

    println("Nombre: $name")
    println("Edad: $edad")
    println("Estatura: $estatura")
    println("Vivo: $vivo")
    println("Primera letra: $firstLetter")
}

