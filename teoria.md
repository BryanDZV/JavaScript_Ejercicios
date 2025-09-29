

### 1️⃣ Factorial

**Enunciado**: Calcular `n!`.

* Caso base: `n == 0 → 1`
* Recursivo: `n * factorial(n-1)`

---

### 2️⃣ Fibonacci

**Enunciado**: Serie hasta `n`.

* Caso base: `n <= 1 → n`
* Recursivo: `f(n-1) + f(n-2)`

---

### 3️⃣ Potencia `a^b`

**Enunciado**: Elevar un número a otro.

* Caso base: `b == 0 → 1`
* Recursivo: `a * potencia(a, b-1)`

---

### 4️⃣ Suma de los primeros N números

**Enunciado**: `1 + 2 + ... + n`.

* Caso base: `n == 0 → 0`
* Recursivo: `n + suma(n-1)`

---

### 5️⃣ Suma de elementos en un array

**Enunciado**: Dado un array, devolver suma.

* Caso base: índice fuera de rango → `0`
* Recursivo: `arr[i] + suma(arr, i+1)`

---

### 6️⃣ Invertir cadena

**Enunciado**: `"hola" → "aloh"`.

* Caso base: cadena vacía → `""`
* Recursivo: último carácter + invertir(resto)

---

### 7️⃣ Invertir número

**Enunciado**: `123 → 321`.

* Caso base: `n < 10 → n`
* Recursivo: `último dígito + invertir(resto)`

---

### 8️⃣ Contar dígitos de un número

**Enunciado**: `12345 → 5`.

* Caso base: `n < 10 → 1`
* Recursivo: `1 + contar(n/10)`

---

### 9️⃣ Suma de dígitos

**Enunciado**: `123 → 1+2+3=6`.

* Caso base: `n == 0 → 0`
* Recursivo: `(n % 10) + suma(n/10)`

---

### 🔟 Palíndromo

**Enunciado**: Comprobar `"ana"` → true.

* Caso base: cadena <= 1 → true
* Recursivo: comparar extremos + llamar con el interior

---

### 1️⃣1️⃣ MCD (Euclides)

**Enunciado**: Calcular MCD de `a` y `b`.

* Caso base: `b == 0 → a`
* Recursivo: `MCD(b, a % b)`

---

### 1️⃣2️⃣ Buscar en array (lineal)

**Enunciado**: Buscar X en array.

* Caso base: fin de array → -1
* Recursivo: comparar arr[i] + llamada en i+1

---

### 1️⃣3️⃣ Búsqueda binaria

**Enunciado**: Buscar X en array ordenado.

* Caso base: izquierda > derecha → -1
* Recursivo: dividir mitad y decidir lado

---

### 1️⃣4️⃣ Torres de Hanói

**Enunciado**: Mover N discos de torre A a C usando B.

* Caso base: `n == 1 → mover A→C`
* Recursivo:

  1. mover(n-1, A, B, C)
  2. mover disco de A→C
  3. mover(n-1, B, C, A)

---

### 1️⃣5️⃣ Recorrer lista enlazada

**Enunciado**: Imprimir todos los nodos.

* Caso base: nodo == null → return
* Recursivo: imprimir nodo + recorrer(siguiente)

---

### 1️⃣6️⃣ Altura de árbol binario

**Enunciado**: Calcular altura.

* Caso base: nodo == null → 0
* Recursivo: `1 + max(altura(izq), altura(der))`

---

### 1️⃣7️⃣ Contar hojas de un árbol

**Enunciado**: Nodos sin hijos.

* Caso base: nodo == null → 0
* Caso hoja: sin hijos → 1
* Recursivo: hojas(izq) + hojas(der)

---

### 1️⃣8️⃣ Recorridos de árbol

**Inorden**: izq → raíz → der
**Preorden**: raíz → izq → der
**Postorden**: izq → der → raíz

---

### 1️⃣9️⃣ Generar números binarios de N bits

**Enunciado**: Para N=3 → 000,001,…111.

* Caso base: N==0 → imprimir cadena
* Recursivo: añadir "0" y "1" en cada paso

---

### 2️⃣0️⃣ Permutaciones de cadena

**Enunciado**: `"abc" → abc, acb, bac, bca, cab, cba`.

* Caso base: cadena vacía → imprimir acumulado
* Recursivo: elegir letra y permutar el resto

---

# 🔑 Reglas mentales rápidas

* **Siempre** busca el caso base (freno).
* Haz el problema más pequeño en cada llamada.
* Piensa en una **pila**: las llamadas se resuelven al volver atrás.

---
