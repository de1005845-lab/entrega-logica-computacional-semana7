# Herramientas de Logica Computacional - Entrega Semana 7

**Estudiante:** Daniel Eduardo Perez Roberto

### 1. Área de Aplicación: Álgebra Lineal
Esta aplicación se basa en el Álgebra Lineal, específicamente en la teoría de matrices invertibles. Es fundamental para Ingeniería porque la unicidad de la inversa garantiza que sistemas de ecuaciones lineales tengan una única solución.

### 2. Teorema en Lenguaje Natural
Teorema de unicidad de la inversa: Si una matriz cuadrada A tiene inversa, esta es única. Es decir, si B y C son ambas inversas de A, entonces B y C son la misma matriz.

### 3. Traducción a Lenguaje Formal (Proposiciones Cuantificadas)
Definimos el predicado:
Inv(A,B) := (A*B = I y B*A = I) -> "B es inversa de A"

Traducción formal del teorema con cuantificadores universales:
Para todo A, para todo B, para todo C: [(Inv(A,B) y Inv(A,C)) implica (B = C)]

- Cuantificador: Universal (Para todo). Indica que la propiedad es general.
- Conectivos: Conjunción (y) e Implicación (implica).

### 4. Estrategia de Demostración desde el Cálculo de Predicados
Estrategia: Instanciación Universal y Demostración Directa.

Para probar un teorema de la forma "Para todo...", la estrategia en lógica de predicados es tomar elementos arbitrarios pero fijos y demostrar la propiedad.

Pasos:
1. (Instanciación) Sean A, B, C matrices arbitrarias tales que Inv(A,B) y Inv(A,C) son verdaderas. Hipótesis.
2. Por definición, B*A = I y A*C = I.
3. Partimos de B = B*I (propiedad de identidad)
4. Sustituimos I = A*C -> B = B*(A*C)
5. Por asociatividad: B = (B*A)*C
6. Como B*A = I -> B = I*C = C
7. Concluimos B = C. Por Generalización Universal, vale para todas.

### 5. Bibliografías

- Grossman, S. I. (2012). Álgebra lineal (7a ed.). McGraw-Hill. Capítulo 2: Matrices.
- Lay, D. C. (2012). Álgebra lineal y sus aplicaciones (4a ed.). Pearson.
- Rosen, K. H. (2011). Matemática discreta y sus aplicaciones (7a ed.). McGraw-Hill. Capítulo 1: Lógica y demostraciones - Cuantificadores.
- Politécnico Grancolombiano. (2026). Herramientas de Lógica Computacional - Semana 7: Proposiciones cuantificadas.
