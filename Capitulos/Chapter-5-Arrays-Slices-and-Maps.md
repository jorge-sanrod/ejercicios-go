# Arrays, Slices, and Maps
En este capitulo se habla sobre algunos tipos de datos especiales como lo son arrays, slices y maps. Se mira la manera de declararlos y como trabajar con ellos.

#### 1. How do you access the fourth element of an array or slice?
Para acceder al elemento de un array o slice se coloca la posicion-1 entre [] al lado de la varibale, ejemplo:
```go
arreglo[3]
```

#### 2. What is the length of a slice created using make([]int, 3, 9)?
```
el tamaño del slice es 3.
```
#### 3. Given the following array, what would x[2:5] give you?
```go
x := [6]string{"a","b","c","d","e","f"}
```
["c" "d" "e"]

#### 4. Write a program that finds the smallest number in this list:
```go
x := []int{
 48,96,86,68,
 57,82,63,70,
 37,34,83,27,
 19,97, 9,17,
}
```

```go
package main
import "fmt"

func main() {
    x := []int{
    48,96,86,68,
    57,82,63,70,
    37,34,83,27,
    19,97, 9,17,
    }

    small := x[0]
    for i:=;i<=length(x);i++{
        if small>x[i]{
            small=x[i]
        }
    }

    fmt.Println(small)
}
```

[ :arrow_left: Capítulo Anterior](/Capitulos/Chapter-4-Control-Structures.md) - [Capítulo Siguiente :arrow_right: ](/Capitulos/Chapter-6-Functions.md)