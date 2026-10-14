# Herramientas de Logica Computacional - Entrega Semana 7

### Traduccion a lenguaje formal
Inv(A,B) := A*B = I y B*A = I

Teorema: Para todo A, para todo B, para todo C: [(Inv(A,B) y Inv(A,C)) implica (B = C)]

### Estrategia de Demostracion
Demostracion Directa + Instanciacion Universal

1. Tomemos B y C inversas de A. Hipotesis: A*B = I y A*C = I
2. B = B*I
3. I = A*C -> B = B*(A*C)
4. Por asociatividad: B = (B*A)*C
5. Como B*A = I -> B = I*C = C
6. Por tanto B = C.

### Ejemplo cotidiano
"No es posible que haya dos claves maestras diferentes"
Formal: Para todo A, B, C ((P(A,B) y P(A,C)) implica B=C)

### Referencias POLI
1. Villamil, M., & Torres, L. (2019). Fundamentos de logica.
2. Castro, R. (2021). Estructuras discretas.
3. Grossman, S. I. (2019). Algebra lineal.
