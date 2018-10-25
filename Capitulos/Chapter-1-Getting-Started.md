# 1. Gettin Staarted
El primer capitulo contiene una introduccion a lo que es Go, su instalación, editores y un primer programa con el cual se explica brebemente la manera en que Go lee los codigos.

#### 1. What is whitespace?
```
El espacio en blanco es el espacio entre los caracteres (espacios, tabulaciones y lineas nuevas).
```
#### 2. What is a comment? What are the two ways of writing a comment?
Los comentarios son ignorados por el compilador y son usualmente usados como notas para los programadores.  Ejemplos:

```go
//Esto es un comentario de una sola linea
/*Este comentario
puede habarcar mas
de una linea*/
```

#### 3. Our program began with package main. What would the files in the fmt package begin with?
```
En la paqueteria fmt sus archivos empezarian con "package fmt"
```
#### 4. We used the Println function defined in the fmt package. If you wanted to use the Exit function from the os package, what would you need to do?
```go
import "os"

//más líneas de codigo
os.Exit()
```

#### 5. Modify the program we wrote so that instead of printing Hello, World it prints Hello, my name is followed by your name.

```go
package main
import "fmt"

func main() {
	fmt.Println("Hello, my name is Jorge")
}
```

 [Siguiente Capítulo :arrow_right: ](/Capitulos/Chapter-2-Types.md)	
