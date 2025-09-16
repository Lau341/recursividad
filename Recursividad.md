# Recursividad

## Factorial
### ¿Qué es un factorial?
- Un factorial es el producto de todos los números enteros positivos hasta un número dado, denotado por un signo de exclamación (!), y se utiliza para calcular el número de formas en que se pueden ordenar objetos (permutaciones), es decir, n! [3, 5, 9, 11, 15]= n * (n-1) * ... * 1. Por ejemplo, el factorial de 4, o 4!, es 4 × 3 × 2 × 1 = 24. 
### ¿Cómo se calcula?
- Para calcular el factorial de un número entero positivo (n), multiplicas ese número por todos los enteros positivos inferiores a él, hasta llegar a 1.
```
n! = n × (n-1) × (n-2) × ... × 3 × 2 × 1
```
### Ejemplos 
```
5! = 5 × 4 × 3 × 2 × 1 = 120
3! = 3 × 2 × 1 = 6
0! = 1, por definición
```
## Recursividad en KOTLIN
```
fun factorial(n:int) : int {
  if (n==0)
  {
    return 1
  }
  else
  {
    return n* factorial (n-1)
  }
}

fun main ()
{
  println(factorial(5))
}
```
