# Estructuras de controll en Kotlin

## Las estructuras de controll en Kotlin son muy similares a las de otros lenguajes y traen consigo pequenas facilidades.

### If-Else. utilizada para cambiar la secuencia del programa segun una condicion.

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