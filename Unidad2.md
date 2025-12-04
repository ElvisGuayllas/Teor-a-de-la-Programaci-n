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

**¿Como funciona?**
1. Declaración de variables: Se declara una variable llamada edad que es del tipo entero (Entero). Esto significa que se utilizará para almacenar un número entero, que representará la edad de la persona.
Ingreso de datos:

2. Se despliega un mensaje en pantalla que dice "Ingrese su edad: ", solicitando al usuario que introduzca su edad.
Luego, se utiliza la instrucción Leer para capturar el valor ingresado por el usuario y almacenarlo en la variable edad.
Estructura condicional:

3. Se evalúa una condición con la estructura Si...Entonces. La condición que se verifica es si la edad es mayor o igual a 18.
Si la condición es verdadera (es decir, si la edad ingresada es 18 años o más), se ejecuta la instrucción que sigue, que es Escribir "Usted es mayor de edad". Esto significa que se informa al usuario que es mayor de edad.

5. Fin del algoritmo:
Las instrucciones del algoritmo finalizan con FinAlgoritmo, indicando que se ha completado el proceso.

**Ejemplo en aplicado en Lenguaje C:**

![Ejemplo de la condicion IF](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/ifc.png)

**¿Como funciona?**
1. El programa pide al usuario que ingrese su edad.
2. Guarda ese número en la variable edad.
3. Luego verifica si la edad es mayor o igual a 18.
4. Si lo es, muestra el mensaje: "Usted es mayor de edad".
5. Si es menor de 18, no muestra nada más.

El programa es sencillo sirve para verificar si una persona es mayor de edad a base de la edad ingresada.

### 2. **Condicional Doble (If - Else)** 🔄
Aquí definimos qué hacer en ambos casos. Si la condición se cumple, se hace una cosa; si no se cumple, se hace otra distinta. **Nunca se ejecutan ambas a la vez.**  
**Lógica:** *"Si tengo dinero, compro el juego. Si no (Else), solo miro la demo."*

**Ejemplo en diagrama de flujo**
![Ejemplo de la condicion if - else](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/D.%20de%20Flujo%20elseif.png)

**¿Como funciona?**

1- PSeInt simula el else if mediante la anidación de bloques (SiNo + Si).
2- Evaluación Anidada: Cuando la condición principal (Si) es falsa, el flujo de ejecución entra al bloque SiNo para encontrar el siguiente Si.
3- Cierre de Bloques: Esta anidación explica por qué se requieren múltiples FinSi al final. Cada FinSi cierra un nivel de la decisión que fue abierto por un Si anterior.
4- I/O Simple: El proceso de entrada y salida es más directo: Leer edad y Escribir "Mensaje".

**Ejemplo en aplicado en lenguaje C**

![Ejemplo de la condicion IF - Else](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/else-if.png)

**¿Como funciona?**
1- El lenguaje C utiliza el if-else if como una cadena secuencial y plana.

2- Evaluación Rápida: La estructura else if actúa como un filtro directo. Si la primera condición (if) es falsa, el programa pasa al else if y así sucesivamente.

3- Exclusividad: Tan pronto como una condición (if o else if) se cumple, el programa salta inmediatamente fuera de toda la cadena (sin mirar los else if restantes).

### 3. **Condicional Múltiple o Anidada (If - Else If)** 🪜
Es lo que usamos en tu ejercicio de la bonificación. Es una **escalera de condiciones**. Si falla la primera, prueba la segunda, luego la tercera, etc.  
**Lógica:** *"¿Es rojo? No. ¿Entonces es verde? No. ¿Entonces es azul? Sí."*

### 4. **Selección Múltiple (Switch / Case)** 🎛️
Esta estructura es especial. En lugar de evaluar rangos (mayor que, menor que), compara el valor de una variable contra una **lista de casos específicos (igualdad)**. Es más limpio que escribir muchos `else if` cuando sabes los valores exactos.  
**Uso ideal:**
- ✅ Menús de opciones
- ✅ Días de la semana
- ✅ Códigos de error

---

## 📊 **Ejercicios en diagrama de flujo y en C**
En la siguiente secion se muestrara digrama de flujo del uso de los tipos de condicionales antes mencionados






---

## 🔄 **Estructuras repetitivas** 
*(tipos y ejercicios en diagrama de flujo y en C)*

---

## 🎯 **Ejercicio combinando estructura condicional y repetitiva** 
*(Java o Python)*

- 📝 **Descripción del problema**
- 🔄 **Diagrama de flujo simplificado**
- 💻 **Programa**
- ✅ **Verificación**

---

## ⚠️ **Principales dificultades**  
*en la aplicación de los contenidos.*

---

## 🤔 **Reflexión crítica**  
*de los aprendizajes de la unidad.*

---

## 🗂️ **Tareas entregadas**



