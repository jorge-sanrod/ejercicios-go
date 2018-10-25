# Functions
En este capitulo se habla sobre las funciones, su estructura, su uso y la manera en que se declaran.

#### 1. sum is a function that takes a slice of numbers and adds them together. What would its function signature look like in Go?

#### 2. Write a function that takes an integer and halves it and returns true if it was even or false if it was odd. For example, half(1) should return (0, false) and half(2) should return (1, true).
```go
func half(x int) (int, bool) {
    return x/2, x%2==0
}
```

#### 3. Write a function with one variadic parameter that finds the greatest number in a list of numbers.
```go
func max(xs ...int) int {
    var max int
    for i, x := range xs {
        if i == 0 || x > max {
            max = x
        }
    }
 return max
}
```

#### 4. Using makeEvenGenerator as an example, write a makeOddGenerator function that generates odd numbers.
```go
func makeOddGenerator() func() uint {
    i := uint(1)
    return func() (ret uint) {
        ret = i
        i += 2
        return
    }
}
```

#### 5. The Fibonacci sequence is defined as: fib(0) = 0, fib(1) = 1, fib(n) = fib(n-1) + fib(n-2). Write a recursive function that can find fib(n)
```go
func fibonacci(n int) int {
    switch n {
        case 0:
            return 0
        case 1:
            return 1
        default:
            return fibonacci(n-1) + fibonacci (n-2)
    }
}
```

#### 6. How do you get the memory address of a variable?
Para obtener la direccion de memoria de una variable se utiliza el operador &, ejemplo:
```go
//memoria guarda la direccion de memoria que tiene x.
memoria=&x
```

#### 7. How do you assign a value to a pointer?
Para asignar el valor a un puntero es necesario agregar un * antes de la variable, ejemplo:
```go
*operador=5
```

#### 8. How do you create a new pointer?
Los apuntadores se crean de la siguiente manera: nombre = new(tipo)
```go
x=new(int)
```

#### 9. What is the value of x after running this program:
```go
func square(x *float64) {
 *x = *x * *x
}
func main() {
 x := 1.5
 square(&x)
}
```
El valor de x sera de 2.25

#### 10. Write a program that can swap two integers (x := 1; y := 2; swap(&x, &y) should give you x=2 and y=1).
```go
func swap(x, y *int) {
    *x, *y = *y, *x
}
```

[ :arrow_left: Capítulo Anterior](/Capitulos/Chapter-5-Arrays-Slices-and-Maps.md) - [Capítulo Siguiente :arrow_right: ](/Capitulos/Chapter-7-Structs-and-Interfaces.md)