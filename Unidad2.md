# 📚 **TEMAS PRINCIPALES**

## 🔹 **Tipos de Estructuras Condicionales** 

**Las estructuras condicionales** son las herramientas que permiten a un programa *"tomar decisiones"*. Rompen la ejecución lineal (paso 1, paso 2, paso 3) y crean bifurcaciones en el camino:  
> **"Si pasa X, haz esto; si no, haz lo otro."**

**Los tipos principales** que encontrarás en lenguajes como **C, Java, Python**, etc., son:

### 1. **Condicional Simple (If)** ✅
Es la estructura más básica. Se evalúa una condición; si es verdadera, se ejecuta un bloque de instrucciones. Si es falsa, no pasa nada y el programa sigue su curso. 

**Lógica:** *"Si llueve, llevo paraguas."*  
*(Si no llueve, simplemente sigo caminando).*

**Ejemplo en diagrama de flujo:**  
![Ejemplo de la condicion IF](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/if.png)

**¿Cómo funciona?**  
1. **Declaración de variables**: Se declara `edad` (tipo entero) para almacenar la edad.  
2. **Ingreso de datos**: Muestra "Ingrese su edad: " y usa `Leer` para capturar el valor.  
3. **Estructura condicional**: `Si edad >= 18 Entonces` → `Escribir "Usted es mayor de edad"`.  
4. **Fin del algoritmo**: `FinAlgoritmo`.

**Ejemplo en Lenguaje C:**  
![Ejemplo de la condicion IF](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/ifc.png)

**¿Cómo funciona?**  
1. Pide al usuario ingresar su edad.  
2. Guarda el número en `edad`.  
3. Verifica `if (edad >= 18)`.  
4. Si es verdadero, muestra "Usted es mayor de edad".  
5. Si es menor de 18, no muestra nada más.

> **Programa sencillo para verificar si una persona es mayor de edad.**

---

### 2. **Condicional Doble (If - Else)** 🔄
Aquí definimos qué hacer en **ambos casos**. Si la condición se cumple, se hace una cosa; si no, otra distinta. **Nunca se ejecutan ambas a la vez.**  
**Lógica:** *"Si tengo dinero, compro el juego. Si no (Else), solo miro la demo."*

**Ejemplo en diagrama de flujo:**  
![Ejemplo de la condicion if - else](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/D.%20de%20Flujo%20elseif.png)

**¿Cómo funciona?**  
1. **PSeInt**: Simula `else if` mediante anidación (`SiNo + Si`).  
2. **Evaluación anidada**: Si la condición principal falla, entra al `SiNo`.  
3. **Cierre de bloques**: Múltiples `FinSi` cierran cada nivel.  
4. **I/O simple**: `Leer edad` y `Escribir "Mensaje"`.

**Ejemplo en lenguaje C:**  
![Ejemplo de la condicion IF - Else](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/else-if.png)

**¿Cómo funciona?**  
1. **Cadena secuencial**: `if-else if` como filtro directo.  
2. **Evaluación rápida**: Pasa al siguiente `else if` si el anterior falla.  
3. **Exclusividad**: Al cumplir una condición, **salta fuera** de toda la cadena.

---

### 3. **Condicional Múltiple (If - Else If)** 🪜
Es una **escalera de condiciones**. Si falla la primera, prueba la segunda, luego la tercera, etc.  
**Lógica:** *"¿Es rojo? No. ¿Entonces es verde? No. ¿Entonces es azul? Sí."*

**Ejemplo en diagrama de flujo:**  
![Ejemplo usando C. Múltiple](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/DF%20Condicional%20M%C3%BAltiple.png)

**¿Cómo funciona?**  
1. **Definición**: Dato numérico entero.  
2. **Entrada**: `Leer` dato del usuario.  
3. **Verificación Error** → **Niño** → **Adolescente** → **Adulto** → **Adulto Mayor** (por descarte).  
4. **Cierre**: Múltiples `FinSi`.

**Ejemplo en lenguaje C:**  
![Ejemplo usando C. Múltiple](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/Condicional%20M%C3%BAltiple.png)

**¿Cómo funciona?**  
1. **Entrada**: Pregunta y guarda dato numérico.  
2. **Filtros secuenciales**: `if` → `else if` → `else if` → `else`.  
3. **Salto inmediato**: Al cumplir condición, termina la cadena.

---

### 4. **Selección Múltiple (Switch / Case)** 🎛️
Compara una variable contra **casos específicos (igualdad)**. Más limpio que muchos `else if`.  
**Uso ideal:**  
- ✅ Menús de opciones  
- ✅ Días de la semana  
- ✅ Códigos de error  

**Ejemplo en diagrama de flujo:**  
![Ejemplo con Switch](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/case%20Df.png)

**¿Cómo funciona?**  
1. **Entrada**: `num1`, `num2`, `operador`.  
2. **`Segun operador Hacer`**: Coincidencia exacta (+, -, *, /).  
3. **Validación**: Previene división por cero.  
4. **`De Otro Modo`**: Error si operador inválido.

**Ejemplo en lenguaje C:**  
![Ejemplo con Switch](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/case%20c.png)

**¿Cómo funciona?**  
1. **Variables**: `float num1, num2, resultado; char operador`.  
2. **`switch(operador)`**: Compara con cada `case`.  
3. **`break` esencial**: Sale tras ejecutar caso correcto.  
4. **`default`**: "Operador no válido".

---

## 🔄 **Estructuras repetitivas**  
*(tipos y ejercicios en diagrama de flujo y en C)*

## 🎯 **Ejercicio combinado**  
*(Condicional + Repetitiva en Java/Python)*  
- 📝 **Descripción del problema**  
- 🔄 **Diagrama de flujo**  
- 💻 **Programa**  
- ✅ **Verificación**

## ⚠️ **Dificultades principales**  
## 🤔 **Reflexión crítica**  
## 🗂️ **Tareas entregadas**



