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
**Ejemplo en diagrama de Flujo**

![Ejemplo usando C. Mutiple](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/DF%20Condicional%20M%C3%BAltiple.png)

**¿Como funciona?**
1- Definición: El algoritmo inicia y establece que el dato que va a procesar será de tipo numérico entero.

2- Entrada de Dato: El programa usa Leer para esperar y recibir el dato del usuario.

3- Verificación Error: El primer Si verifica si el dato es negativo. Si es Verdadero, ejecuta el error y salta el resto de los bloques.

4- Verificación Niño: Si el paso 3 fue Falso, el flujo entra al bloque SiNo para encontrar el siguiente Si. Este verifica la categoría "Niño". Si es Verdadero, salta los bloques restantes.

5- Verificación Adolescente: El flujo continúa su camino descendente entrando al siguiente SiNo y verifica la categoría "Adolescente".

6- Verificación Adulto: El flujo continúa bajando en los SiNo anidados y verifica la categoría "Adulto".

7- Caso Final: Si fallaron todas las verificaciones anteriores, la acción del último SiNo se ejecuta por descarte (imprimir "Adulto Mayor").

8- Cierre: El programa cierra cada bloque lógico abierto utilizando los múltiples comandos FinSi y termina el algoritmo.

**Ejemplo aplicado en lenguaje C**

![Ejemplo usando C. Mutiple](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/Condicional%20M%C3%BAltiple.png)

**¿Como funciona?**

1- Entrada de Dato: El programa muestra una pregunta en pantalla y espera que el usuario ingrese el dato numérico, guardándolo en memoria.
2- Filtro Error: Verifica si el dato ingresado es menor a cero (if). Si esta condición es Verdadera, imprime un mensaje de error y el programa ignora todos los pasos siguientes.
3- Filtro Niño: Si el paso 3 falló, el programa verifica la siguiente categoría (else if). Si es Verdadera, imprime "Niño" y salta al final del programa.
4- Filtro Adolescente: Si el paso 4 falló, el programa verifica si el dato entra en la categoría de "Adolescente" (else if). Si es Verdadera, imprime la categoría y salta al final.
5- Filtro Adulto: Si el paso 5 falló, verifica si el dato entra en la categoría de "Adulto" (else if). Si es Verdadera, imprime la categoría y salta al final.
6- Caso Final: Si todos los filtros anteriores fallaron, el programa ejecuta la acción del último else (imprimir "Adulto Mayor") por simple descarte.
7- Cierre: La función principal del programa termina.

### 4. **Selección Múltiple (Switch / Case)** 🎛️
Esta estructura es especial. En lugar de evaluar rangos (mayor que, menor que), compara el valor de una variable contra una **lista de casos específicos (igualdad)**. Es más limpio que escribir muchos `else if` cuando sabes los valores exactos.  
**Uso ideal:**
- ✅ Menús de opciones
- ✅ Días de la semana
- ✅ Códigos de error

**Ejemplo usando diagrama de flujo*** 

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



