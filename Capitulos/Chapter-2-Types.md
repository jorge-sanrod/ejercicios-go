# Types
Este capitulo esta destinado en enseñar los tipos de datos que podemos utilizar en Go, estos pueden ser, booleanos, numericos, cadenas y derivadas.

#### 1. How are integers stored on a computer?
```
Se almacenan utilizando el sistema binario.
```

#### 2. We know that (in base 10) the largest one-digit number is 9 and the largest twodigit number is 99. Given that in binary the largest two-digit number is 11 (3), the largest three-digit number is 111 (7) and the largest four-digit number is 1111 (15), what’s the largest eight-digit number? (Hint: 101−1 = 9 and 102−1 = 99)
```
255.
```

#### 3. Although overpowered for the task, you can use Go as a calculator. Write a program that computes 32,132 × 42,452 and prints it to the terminal (use the * operator for multiplication).
```go
package main
import "fmt"

func main() {
    fmt.Print(32132*42452)
}
```

#### 4. What is a string? How do you find its length?
```
Un string es un arreglo de caracteres y se puede saber su tamaño con la funcion "len".
```

#### 5. What’s the value of the expression (true && false) || (false && true) || ! (false && false)?
```
True.
```

[ :arrow_left: Capítulo Anterior](/Capitulos/Chapter-1-Getting-Started.md) - [Capítulo Siguiente :arrow_right: ](/Capitulos/Chapter-3-Variables.md)
