# Variables
En este capitulo se exponen las diferentes maneras de declarar variables, los ejercicios estan orientados a su declaracion y la anera en que estos cambian durante la ejecución del codigo.

#### 1. What are two ways to create a new variable?
```go
//var (nombre de la variable) (tipo o inicializacion)
var ejemplo = 5
//(nombre de la variable) := (inicializacion)
ejemplo := 5
```

#### 2. What is the value of x after running x := 5; x += 1?
```
Su valor seria 6.
```

#### 3. What is scope? How do you determine the scope of a variable in Go?
```
Se utilizan entre los bloques de codigos dividos por {}
```

#### 4. What is the difference between var and const?
```
El valor de una constante no cambia y el de una varible puede cambiar mientras el codigo se ejecuta.
```

#### 5. Using the example program as a starting point, write a program that converts from Fahrenheit into Celsius (C = (F − 32) * 5/9).
```go
package main
import "fmt"

func main() {
    var fahr float32
    fmt.Print("Temperatura en Fahrenheit:")
    fmt.Scanf("%f",&fahr)

    cel := (fahr-31)*(5/9)
    
    fmt.Println(cel)
}
```

#### 6. Write another program that converts from feet into meters (1 ft = 0.3048 m).
```go
package main
import "fmt"

func main() {
    var feet float32
    fmt.Print("Feet: ")
    fmt.Scanf("%f",&feet)

    metros:= feet*0.3048

    fmt.Println(metros)
}
```
[ :arrow_left: Capítulo Anterior](/Capitulos/Chapter-2-Types.md) - [Capítulo Siguiente :arrow_right: ](/Capitulos/Chapter-4-Control-Structures.md)