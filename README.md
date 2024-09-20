## Lenguajes de Programación
### Evaluación Semanal 6

#### 📝 Instrucciones

- El semanal podrá resolverse **en equipos de 3**.
- Se deberá entregar por medio de GitHub Classroom a más tardar a las **23:59:59 del martes 24 de septiembre de 2024**. **No habrán prórrogas**. En caso de requerir más tiempo, se descontará un punto por cada día de entrega tardío.
- Cualquier duda podrá extenarse en la clase, por correo o por medio de Telegram en un horario de 8:00 a 18:00.
- Deberá entregarse en formato LaTeX.
- No es necesario que vuelvan a escribir los ejercicios completos, basta con que los numeren y entreguen **en orden**.

#### 🚀 Ejercicios

1. Evaluar las siguientes expresiones usando a) sustitución, b) ambientes con alcance dinámico y c) ambientes con alcance estático. Es necesario que muestren el ambiente de evaluación final en forma de pila en los casos que corresponda. Para el inciso c) además deberán indicar la cerradura de cada función.

   **Nota:** *En esta ocasión no será necesario que muestren la sintaxis abstracta de las expresiones*

   - *Expresión (a)*

      ```lisp
      (let (a 2)
         (let (b 3)
            (let (foo (lambda (x) (- (+ a b) x)))
               (let (a -2)
                  (let (b -3)
                     (let (foo (lambda (x) (+ (- a b) x)))
                        (foo - 10)))))))
      ```

   - *Expresión (b)*

      ```lisp
      (let (foo (lambda (x) (+ x (foo (- x 1)))))
         (foo 10))
      ```
