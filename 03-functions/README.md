### Funciones en Kotlin

## Las funciones son una forma de agrupar partes de codigo que idealmente realizen una tarea, estas se declaran utilizando la palabra fun luego el nombre de la funcion y su valor de retorno si lo tiene.

# **ej**:
```kotlin
fun suma(a: Int, b: Int) Int{
    return a + b
}
```
# Esta funcion se llama suma, recibe 2 parametros a y b que son enteros, y retorna un entero, como se ve en ella esta retornando la suma de a y b.

## En kotlin las funciones son denominadas de **Orden Superior** o (**Higher-Order Functions**), lo que quiere decir que una funcion es tratada como cualquier otro dato, lo que quiere decir que puede ser pasada como valor a otra funcion, retornada por otra funcion o ambas.

```kotlin
fun operar(a: Int, b: Int, operacion: (Int, Int) -> Int): Int {
    return operacion(a, b)
}

fun suma(x: Int, y: Int) = x + y
fun resta(x: Int, y: Int) = x - y

fun main() {
    println(operar(10, 5, ::suma))  // 15
    println(operar(10, 5, ::resta)) // 5
}
