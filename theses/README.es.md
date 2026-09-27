# Tesis — Gabriel Suárez

[English](README.md) · **Español**

`Universidad Politécnica de Madrid` · `Matemática pura` · `TFG + TFM`

Dos trabajos en la misma línea: **polinomios ortogonales de Sobolev**, abordados primero
por sus ceros y después por el operador que los genera. Resumidos aquí para quien no es
especialista. Los enunciados formales, las demostraciones y la bibliografía están en las
propias memorias, que no se publican en este repositorio.

## El escenario, y por qué no es rutinario

Los polinomios ortogonales clásicos vienen de un producto interior que solo pesa valores:

```
⟨f, g⟩ = ∫ f(x) g(x) dμ(x)
```

Un producto interior de **Sobolev** pesa además derivadas. En el caso *discreto*, los
términos de derivada son evaluaciones en un número finito de puntos:

```
⟨f, g⟩ = ∫ f(x) g(x) dμ(x) + Σ  λ_k · f^(j_k)(c_k) · g^(j_k)(c_k)
```

Ese añadido pequeño elimina dos garantías que la teoría clásica regala:

- **Los ceros ya no tienen por qué quedarse dentro del intervalo de ortogonalidad.**
  Pueden salirse de él, y pueden salirse de la recta real. Todo lo construido sobre el
  argumento clásico de localización —reglas de cuadratura, cotas de aproximación— hay que
  rederivarlo en vez de heredarlo.
- **La multiplicación por `x`, el operador `f ↦ x·f`, ya no tiene por qué ser acotada.**
  En el caso clásico es el objeto bien portado sobre el que descansa toda la teoría. Aquí
  su acotación es una pregunta, y la respuesta depende de los puntos `c_k`, de los órdenes
  `j_k` y de las masas `λ_k`.

Las dos preguntas son la misma pregunta. La norma del operador de multiplicación es lo
que confina los ceros; si el operador no es acotado, el argumento de confinamiento
desaparece.

## TFM — el operador de multiplicación en espacios de Sobolev discretos

Un análisis espectral y matricial de ese operador: **acotación, evaluaciones puntuales y
localización de ceros.**

El objeto que lo conecta todo es el funcional de **evaluación puntual**, `f ↦ f^(j)(c)`.
Cuáles de esos funcionales son acotados en el espacio es exactamente lo que decide el
comportamiento del operador, y distinguir los acotados de los no acotados es la parte
difícil: es una propiedad cualitativa de un espacio de dimensión infinita, no algo que
un cálculo finito lea directamente.

La aportación es un **índice que extiende los números de Gelfand a operadores
potencialmente no acotados**, junto con la demostración de que **el punto donde ese
índice se estabiliza identifica las evaluaciones puntuales no acotadas.** Los números de
Gelfand son una forma clásica de medir cuánto dista un operador acotado de poder
aproximarse por operadores de rango finito; la extensión lleva esa medición a un
escenario donde el operador puede no ser acotado en absoluto, y el punto de
estabilización de la sucesión resultante se convierte en un detector. Una pregunta
cualitativa pasa a ser una que responde una sucesión de cantidades computables.

**Parte computacional, en Maple.** En la base polinómica el operador de multiplicación
tiene una representación como matriz de **Hessenberg** —casi triangular, con una sola
subdiagonal— y lo que se puede calcular de verdad son las truncaciones de esa matriz. Sus
**valores singulares** son la evidencia numérica: son las cantidades de dimensión finita
con las que se construye el índice, y observarlas a lo largo de las truncaciones es cómo
se ve la estabilización, no solo cómo se demuestra.

## TFG — ceros de polinomios ortogonales de Sobolev

Los mismos objetos desde el otro extremo: **algoritmos para calcular y visualizar los
conjuntos de ceros**, y la conexión de vuelta con las **normas de operadores**.

Calcular los ceros es un problema numérico que la pérdida de la garantía clásica de
localización vuelve genuinamente incómodo: no puedes partir de "están en el intervalo y
son simples", porque en general no son ni lo uno ni lo otro. Visualizarlos a lo largo de
familias y de los parámetros del producto interior es lo que hace legible el
comportamiento: cómo se mueven los ceros al crecer la masa `λ`, cuándo abandonan el
intervalo, qué ocurre en los puntos donde se evalúan las derivadas. Relacionar esa imagen
con la norma del operador de multiplicación es el puente hacia el trabajo analítico de
arriba.

## Cómo se lee esto fuera de la matemática pura

Lo transferible es el hábito.

- **Enunciar el problema es la mayor parte del trabajo.** "Cuándo es acotado este
  operador" no es la pregunta que te entregan; es a la que llegas después de decidir qué
  gobierna de verdad el comportamiento que te importa.
- **Antes un criterio computable que una descripción correcta.** Un índice cuyo punto de
  estabilización puedes observar vale más que una caracterización exacta que no puedes
  evaluar.
- **La parte numérica es evidencia, no adorno.** Las truncaciones de Hessenberg y sus
  valores singulares son donde una afirmación sobre un operador de dimensión infinita se
  convierte en algo que puedes mirar.

## Herramientas

Maple para el trabajo simbólico y numérico sobre operadores, representaciones matriciales
y polinomios ortogonales. Python (NumPy) en lo demás.

## Texto completo

No se publica aquí. Disponible a petición — [suarez.gabriel03@gmail.com](mailto:suarez.gabriel03@gmail.com).

---

[← Perfil](../gabriel.es.md)
