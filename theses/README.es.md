# Tesis — Gabriel Suárez

[English](README.md) · **Español**

Universidad Politécnica de Madrid · Grado en Matemáticas e Informática · Máster Universitario en Matemáticas Avanzadas

Mis dos trabajos estudian los polinomios ortogonales de Sobolev: primero sus
ceros y después el operador de multiplicación y su representación matricial.
Los repositorios públicos enlazados contienen las fuentes matemáticas y el
material computacional disponible. Esta página resume su alcance para quien
quiera valorar mi trabajo.

## TFM — operadores de multiplicación en espacios de Sobolev discretos

*Análisis espectral y matricial del operador de multiplicación en espacios de
Sobolev discretos* · **9,5/10**

**Problema.** En un producto interno de polinomios con términos discretos de
derivadas, la multiplicación $Dp(z)=zp(z)$ puede no estar acotada. El trabajo
estudia cómo las restricciones de codimensión finita controlan esa dificultad
y cómo se refleja en secciones matriciales finitas.

**Trabajo matemático.** La memoria estudia un índice de tipo Gelfand $Q_k(D)$,
definido mediante el ínfimo de las normas de restricción a subespacios de
polinomios de codimensión a lo sumo $k$, admitiendo el valor $+\infty$.
Es la perspectiva de restricciones utilizada en los números de Gelfand.

Para la configuración formada por la medida normalizada de una circunferencia
de radio $R$ y $N$ átomos distintos de primera derivada con pesos unitarios,
sea $m$ el número de átomos sobre la circunferencia o fuera de ella. La memoria
establece:

- $Q_k(D)=+\infty$ para $0\le k<m$;
- $Q_k(D)$ es finito para $m\le k<N$;
- $Q_k(D)=R$ para $k\ge N$.

El primer índice finito es, por tanto, $Q_m(D)$. El resultado corresponde a
esta configuración; no es un detector universal para cualquier producto
interno de Sobolev. Conviene distinguir la primera finitud de la igualdad
eventual con $R$.

**Trabajo computacional.** Las rutinas de Maple estudian representaciones
finitas de Hessenberg y sus valores singulares. Los autovalores de las secciones
principales proporcionan los ceros de los polinomios ortogonales
correspondientes; la memoria relaciona los límites de los valores singulares
ordenados con $Q_k(D)$. Los cálculos finitos ilustran estos resultados y no
demuestran por sí solos afirmaciones asintóticas.

**Evidencia pública.** [Repositorio y resumen](https://github.com/Gabotelli/sobolev-multiplication-operators) ·
[Fuente de la memoria](https://github.com/Gabotelli/sobolev-multiplication-operators/blob/master/Plantilla%20TFM/main.tex) ·
[Resultados para la circunferencia](https://github.com/Gabotelli/sobolev-multiplication-operators/blob/master/Plantilla%20TFM/chapters/capitulo3-estabilizacion.tex) ·
[Fuente de la defensa](https://github.com/Gabotelli/sobolev-multiplication-operators/blob/master/Plantilla%20TFM/presentacion/defensa.tex).

**Estado de reproducción.** Los worksheets independientes de Maple todavía no
están incluidos. El repositorio contiene fuentes LaTeX y figuras existentes;
no se ha verificado una compilación limpia de la memoria y las diapositivas.

## TFG — ceros de polinomios ortogonales de Sobolev

*Ceros de polinomios ortogonales de Sobolev: visualización y análisis* · **9,4/10**

**Problema.** Los términos de derivadas cambian los argumentos clásicos de
localización de ceros. El trabajo estudia las configuraciones de ceros y su
relación con las normas del operador de multiplicación.

**Aportación computacional.** Los algoritmos de Maple construyen familias de
polinomios, calculan y visualizan sus ceros y comparan su localización con normas
de operadores y valores singulares. Los experimentos incluyen configuraciones
de soporte real y complejo y permiten formular e investigar conjeturas.
La memoria distingue las observaciones numéricas de los resultados demostrados.

**Evidencia pública.** [Repositorio y resumen](https://github.com/Gabotelli/sobolev-orthogonal-polynomials) ·
[Worksheet de Maple](https://github.com/Gabotelli/sobolev-orthogonal-polynomials/blob/main/maple/tfg7.mw) ·
[Fuente de la memoria](https://github.com/Gabotelli/sobolev-orthogonal-polynomials/blob/main/latex/tfg_latex_etsiinf-2023.02.20/tfg_etsiinf_plantilla.tex) ·
[Inventario de Maple](https://github.com/Gabotelli/sobolev-orthogonal-polynomials/blob/main/docs/maple-inventory.md).

**Estado de reproducción.** Se publican cuatro worksheets `.mw` y un workbook
`.maple`. Los 55 archivos `.m` restantes son estados serializados, no programas
independientes. Algunos worksheets utilizan estados guardados o lecturas
externas; no se ha verificado una regeneración portable de todos los experimentos
y figuras.

## Autoría y herramientas

Este trabajo está vinculado a `EGS26`, un artículo todavía no publicado, elaborado conjuntamente con mis tutoras, Carmen Escribano y Raquel Gonzalo. El trabajo asociado a ese artículo es colaborativo; esta página no me atribuye en exclusiva todos sus resultados.

Las tesis son mi trabajo académico. Los trabajos citados, las plantillas de la
universidad y las rutinas incluidas conservan su atribución; este resumen no
afirma que todos los resultados o rutinas sean originales. Maple se utiliza para
los cálculos y LaTeX para las memorias y el material de defensa.

Los repositorios no incluyen actualmente los PDF compilados. Para consultas:
[suarez.gabriel03@gmail.com](mailto:suarez.gabriel03@gmail.com).

---

[← Perfil](../gabriel.es.md)
