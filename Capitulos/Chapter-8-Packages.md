# Packages
En este capitulo se habla sobre los paquetes, diferentes paquetes que podemos utilizar, sus declaraciones y sus usos.

#### 1. Why do we use packages?
```
Los utilizamos para dividir programas grandes en programas mas pequeños, que son mas faciles de entender y mas faciles de dar mantenimiento. Es una buena practica de ingeniería de software.
```
#### 2. What is the difference between an identifier that starts with a capital letter and one that doesn’t (e.g., Average versus average)?
```
Los identificadores que comienzan con una letra mayúscula se exportan (es decir, accesibles desde otros paquetes), mientras que los identificadores que comienzan con una letra minúscula no se exportan.
```
#### 3. What is a package alias? How do you make one?
```
Un alias de paquete es un nombre alternativo para un paquete que puede especificar cuando importa el paquete: import f "fmt".
```
#### 4. We copied the average function from Chapter 6 to our new package. Create Min and Max functions that find the minimum and maximum values in a slice of float64s.
```go
func Max(xs []float64) float64 {
    var max float64
    for i, x := range xs {
        if i == 0 || x > max {
            max = x
        }
    }
    return max
}

func Min(xs []float64) float64 {
    var min float64
    for i, x := range xs {
        if i == 0 || x < min {
            min = x
        }
    }
 return min
}
```

#### 5. How would you document the functions you created in #4?
```
Para documentar las funciones creadas en # 4, agregue comentarios antes de las funciones. Esos comentarios se mostrarán como documentación para la herramienta godoc.
```
[ :arrow_left: Capítulo Anterior](/Capitulos/Chapter-7-Structs-and-Interfaces.md) - [Capítulo Siguiente :arrow_right: ](/Capitulos/Chapter-9-Testing.md)