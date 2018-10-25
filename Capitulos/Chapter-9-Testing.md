# Testing
La programación no es fácil; incluso los mejores programadores son incapaces de escribir programas que funcionen exactamente como se pretende cada vez. Por lo tanto, una parte importante del proceso de desarrollo de software es el testing. Escribir pruebas para nuestro código es una buena manera de garantizar la calidad y mejorar la confiabilidad.

#### 1. Writing a good suite of tests is not always easy, but the process of writing tests often reveals more about a problem than you may at first realize. For example, with our Average function, what happens if you pass in an empty list ([]float64{})? How could the function be modified to return 0 in this case?
```go
func Average(xs []float64) float64 {
    if len(xs) == 0 {
        return 0
    }
    total := float64(0)
    for _, x := range xs {
        total += x
    }
    return total / float64(len(xs))
}
```

#### 2. Write a series of tests for the Min and Max functions you wrote in the previous chapter. 
```go
package math
import "testing"

func TestMath(t *testing.T) {
    cases := []struct {
        xs []float64
        max, min float64
    }{
        {
            xs: []float64{3, 5, 2, 1, 7, 9},
            max: 9,
            min: 1,
        },
        {
            xs: []float64{},
            max: 0,
            min: 0,
        },
    }

    for _, c := range cases {
        max := Max(c.xs)
        if max != c.max {
            t.Errorf("expected %f got %f", c.max, max)
        }
        min := Min(c.xs)
        if min != c.min {
            t.Errorf("expected %f got %f", c.min, min)
        }
    }
}
```

[ :arrow_left: Capítulo Anterior](/Capitulos/Chapter-8-Packages.md) - [Capítulo Siguiente :arrow_right: ](/Capitulos/Chapter-10-Concurrency.md)