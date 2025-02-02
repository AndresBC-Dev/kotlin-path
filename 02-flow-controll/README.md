# Estructuras de Control en Kotlin

## Las estructuras de control en Kotlin son muy similares a las de otros lenguajes y traen consigo pequeñas facilidades.

### If-Else Utilizada para cambiar la secuencia del programa según una condición.

```kotlin
fun main() {
    val temp: Double = 17.2
    if (temp > 30) {
        println("It's hot 🌅")
    } else if (temp in 20..30) {
        println("It's nice! 🌥️")
    } else {
        println("It's cold! 🌨️")
    }
}


### For. usado para iterar sobre rangos, colecciones, o arrays.

```kotlin
fun main() {
    for (i in 1..5) {
        println("Number: $i")
    }
}

### While. utilizado para iterar sobre datos tambien pero este se basa en una condicion en lugar de decirle cuantas veces explicitas queremos que lo haga y tambien tiene do-while que solo es una forma mas de usarlo.

```kotlin
fun main() {
    var i = 1

    while (i <= 5) {
        println("Number: $i")
        i++
    }

    i = 1
    do {
        println("Number: $i")
        i++
    } while (i <= 5)
}

### When es similar al switch que hay en otros lenguajes, se usa para dar una respuesta segun un rango de posibilidades.

```kotlin
fun main() {
    val day = 3

    val dayOfWeek = when (day) {
        1 -> "Monday"
        2 -> "Tuesday"
        3 -> "Wednesday"
        4 -> "Thursday"
        5 -> "Friday"
        6 -> "Saturday"
        7 -> "Sunday"
        else -> "Invalid day"
    }

    println(dayOfWeek)
}
