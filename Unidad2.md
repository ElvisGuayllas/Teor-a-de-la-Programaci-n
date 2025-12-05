# 📚 **TEMAS PRINCIPALES**

## 🔹 Tipos de Estructuras Condicionales 

Las **estructuras condicionales** son las herramientas que permiten a un programa *"tomar decisiones"*. Rompen la ejecución lineal (paso 1, paso 2, paso 3) y crean bifurcaciones en el camino:  
**"Si pasa X, haz esto; si no, haz lo otro."**

Los **tipos principales** que encontrarás en lenguajes como C, Java, Python, etc., son:

### 1. **Condicional Simple (If)** ✅
Es la estructura más básica. Se evalúa una condición; si es verdadera, se ejecuta un bloque de instrucciones. Si es falsa, no pasa nada y el programa sigue su curso. 

**Lógica:** *"Si llueve, llevo paraguas."*  
*(Si no llueve, simplemente sigo caminando).*

**Ejemplo en diagrama de flujo:**  
![Ejemplo de la condicion IF](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/if.png)

**¿Cómo funciona?**  
🔢 **1.** Se declara una variable llamada `edad` que es del tipo **entero**. Esto significa que se utilizará para almacenar un número entero, que representará la edad de la persona.  
⌨️ **2.** Se despliega un mensaje en pantalla que dice *"Ingrese su edad:"*, solicitando al usuario que introduzca su edad. Luego, se utiliza la instrucción `Leer` para capturar el valor ingresado por el usuario y almacenarlo en la variable `edad`.  
✅ **3.** Se evalúa una condición con la estructura `Si...Entonces`. La condición que se verifica es si la edad es **mayor o igual a 18**. Si la condición es verdadera, se ejecuta la instrucción `Escribir "Usted es mayor de edad"`.  
🏁 **4.** Las instrucciones del algoritmo finalizan con `FinAlgoritmo`, indicando que se ha completado el proceso.

**Ejemplo aplicado en Lenguaje C:**  
![Ejemplo de la condicion IF](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/ifc.png)

**¿Cómo funciona?**  
🔢 **1.** El programa pide al usuario que ingrese su edad.  
💾 **2.** Guarda ese número en la variable `edad`.  
🔍 **3.** Luego verifica si la edad es **mayor o igual a 18**.  
✅ **4.** Si lo es, muestra el mensaje: *"Usted es mayor de edad"*.  
⏭️ **5.** Si es menor de 18, no muestra nada más.

*Programa sencillo para verificar si una persona es mayor de edad a base de la edad ingresada.*

---

### 2. **Condicional Doble (If - Else)** 🔄
Aquí definimos qué hacer en **ambos casos**. Si la condición se cumple, se hace una cosa; si no se cumple, se hace otra distinta. **Nunca se ejecutan ambas a la vez.**  
**Lógica:** *"Si tengo dinero, compro el juego. Si no (Else), solo miro la demo."*

**Ejemplo en diagrama de flujo:**  
![Ejemplo de la condicion if - else](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/D.%20de%20Flujo%20elseif.png)

**¿Cómo funciona?**  
🔢 **1.** PSeInt simula el `else if` mediante la **anidación de bloques** (`SiNo + Si`).  
🔍 **2.** Cuando la condición principal (`Si`) es falsa, el flujo de ejecución entra al bloque `SiNo` para encontrar el siguiente `Si`.  
🔒 **3.** Esta anidación explica por qué se requieren **múltiples `FinSi`** al final. Cada `FinSi` cierra un nivel de la decisión que fue abierto por un `Si` anterior.  
📥 **4.** El proceso de entrada y salida es más directo: `Leer edad` y `Escribir "Mensaje"`.

**Ejemplo aplicado en lenguaje C:**  
![Ejemplo de la condicion IF - Else](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/else-if.png)

**¿Cómo funciona?**  
🔢 **1.** El lenguaje C utiliza el `if-else if` como una **cadena secuencial y plana**.  
⚡ **2.** La estructura `else if` actúa como un **filtro directo**. Si la primera condición (`if`) es falsa, el programa pasa al `else if` y así sucesivamente.  
🚫 **3.** Tan pronto como una condición (`if` o `else if`) se cumple, el programa **salta inmediatamente** fuera de toda la cadena.

---

### 3. **Condicional Múltiple (If - Else If)** 🪜
Es una **escalera de condiciones**. Si falla la primera, prueba la segunda, luego la tercera, etc.  
**Lógica:** *"¿Es rojo? No. ¿Entonces es verde? No. ¿Entonces es azul? Sí."*

**Ejemplo en diagrama de Flujo:**  
![Ejemplo usando C. Mutiple](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/DF%20Condicional%20M%C3%BAltiple.png)

**¿Cómo funciona?**  
🔢 **1.** El algoritmo inicia y establece que el dato que va a procesar será de tipo **numérico entero**.  
⌨️ **2.** El programa usa `Leer` para esperar y recibir el dato del usuario.  
🚨 **3.** El primer `Si` verifica si el dato es **negativo**. Si es Verdadero, ejecuta el error y salta el resto de los bloques.  
👶 **4.** Si el paso 3 fue Falso, el flujo entra al bloque `SiNo` para encontrar el siguiente `Si`. Este verifica la categoría **"Niño"**.  
🧒 **5.** El flujo continúa su camino descendente entrando al siguiente `SiNo` y verifica la categoría **"Adolescente"**.  
🧑 **6.** El flujo continúa bajando en los `SiNo` anidados y verifica la categoría **"Adulto"**.  
👴 **7.** Si fallaron todas las verificaciones anteriores, la acción del último `SiNo` se ejecuta por descarte (**imprimir "Adulto Mayor"**).  
🔒 **8.** El programa cierra cada bloque lógico abierto utilizando los **múltiples comandos `FinSi`** y termina el algoritmo.

**Ejemplo aplicado en lenguaje C:**  

![Ejemplo usando C. Mutiple](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/Condicional%20M%C3%BAltiple.png)

**¿Cómo funciona?**  
🔢 **1.** El programa muestra una pregunta en pantalla y espera que el usuario ingrese el dato numérico, guardándolo en memoria.  
🚨 **2.** Verifica si el dato ingresado es **menor a cero** (`if`). Si esta condición es Verdadera, imprime un mensaje de error.  
👶 **3.** Si el paso 2 falló, el programa verifica la siguiente categoría (`else if`). Si es Verdadera, imprime **"Niño"** y salta al final.  
🧒 **4.** Si el paso 3 falló, el programa verifica si el dato entra en la categoría de **"Adolescente"** (`else if`).  
🧑 **5.** Si el paso 4 falló, verifica si el dato entra en la categoría de **"Adulto"** (`else if`).  
👴 **6.** Si todos los filtros anteriores fallaron, el programa ejecuta la acción del último `else` (**imprimir "Adulto Mayor"**) por simple descarte.  
🏁 **7.** La función principal del programa termina.

---

### 4. **Selección Múltiple (Switch / Case)** 🎛️
Compara una variable contra **casos específicos (igualdad)**. Más limpio que muchos `else if`.  
**Usos ideales:**  
- ✅ Menús de opciones  
- ✅ Días de la semana  
- ✅ Códigos de error  

**Ejemplo usando diagrama de flujo:**  

![Ejemplo con Switch](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/case%20Df.png)

**¿Cómo Funciona?**  
🔢 **1.** Se solicitan y leen tres variables: dos números (`num1`, `num2`) y un carácter (`operador`).  
⚙️ **2.** La ejecución pasa a la instrucción `Segun operador Hacer`.  
🔍 **3.** El programa busca una **coincidencia exacta** con el valor de la variable `operador` (+, -, *, /).  
✅ **4.** Al encontrar la coincidencia (ej., *), ejecuta la operación correspondiente (`resultado <- num1 * num2`), muestra el resultado, e ignora todos los demás casos.  
🛡️ **5.** Se incluye una estructura condicional (`Si/SiNo`) anidada en el caso de la **división** para prevenir la división por cero.  
🚫 **6.** Si el carácter ingresado no coincide con ningún operador válido, se ejecuta el bloque de **error**.

**Ejemplo aplicado en lenguaje C:**  

![Ejemplo con Switch](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/case%20c.png)

**¿Cómo funciona?**  
🔢 **1.** Se preparan tres variables `float` (`num1`, `num2`, `resultado`) y una variable `char` (`operador`).  
⌨️ **2.** El programa solicita y lee secuencialmente los tres datos necesarios del usuario.  
⚙️ **3.** El control pasa a la instrucción `switch(operador)`. El valor de la variable `operador` se compara directamente con los valores definidos en cada `case`.  
✅ **4.** Si encuentra una coincidencia exacta, ejecuta la operación correspondiente. La instrucción `break;` es **esencial**: garantiza que el flujo salga inmediatamente de la estructura `switch`.  
🚫 **5.** Si el carácter ingresado

# ✅ **Estructuras repetitivas (tipos y ejercicios en diagrama de flujo y en C)**
Las estructuras repetitivas, también llamadas bucles o iteraciones, son mecanismos que permiten ejecutar un conjunto de instrucciones varias veces, dependiendo de una condición o de un número fijado de repeticiones.
Sirven para automatizar tareas repetitivas sin tener que escribir las mismas instrucciones muchas veces.
🔁 Tipos principales de estructuras repetitivas

🔁 **1. Estructura Repetitiva “Mientras” (WHILE)**
✅ Definición: Es una estructura que repite un conjunto de instrucciones mientras una condición sea verdadera.
La condición se evalúa antes de ejecutar el bloque.
⚙️ ¿Cómo funciona?
- Evalúa la condición.
- Si es verdadera → ejecuta el bloque.
- Vuelve a evaluar la condición.
- Repite hasta que la condición resulte falsa.
🎯 Para qué sirve:

- Procesos donde no se sabe cuántas repeticiones habrá.

- Repetir hasta que ocurra algo (un valor, un evento o una entrada válida).

- Controlar bucles dependientes de una condición lógica.

**Ejemplo en diagrama de flujo** 

![Ejemplo con WHILE](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/mientras%20DF%20(1).png)

**¿Como funciona?**

1. Inicialización: El algoritmo define ambas variables como Entero. Luego, las inicializa: contador se establece en 0 y acumulador se establece en 0.

2. Condición de Prueba: La instrucción Mientras contador <= 5 Hacer es el punto de control. Antes de cada ciclo, el programa verifica si el valor del contador es menor o igual a 5.Si es Verdadero, el bloque de código interno se ejecuta.Si es Falso, el bucle se detiene y salta a la línea después de FinMientras.
   
3. Proceso (Dentro del Bucle):acumulador <- acumulador + contador: La suma se realiza. El valor actual del contador se añade al acumulador.contador <- contador + El contador se incrementa en 1. Esta acción es esencial para garantizar que el bucle avance hacia su final y no se convierta en un bucle infinito.
   
4. Terminación y Salida:El bucle se repite hasta que el contador se incrementa a 6. En ese momento, la condición $6 \le 5$ es Falsa.El bucle se detiene.La última línea, Escribir "La suma es: ", acumulador, muestra el resultado final en pantalla, que es 15.

**Ejemplo aplicado en lenguaje C**

![Ejemplo con WHILE](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/mientras%20c.png)

**¿Como funciona?**

1. Condición de Prueba: La instrucción while (contador <= 5) verifica la condición al inicio de cada ciclo. Si la condición es Verdadera (V), el código dentro de las llaves se ejecuta. Si es Falsa (F), el bucle se detiene.

2. Acumulación: La línea acumulador = acumulador + contador; toma el valor actual de contador y lo añade al total acumulado.

3. Incremento (Avance): La línea contador = contador + 1; (o contador++;) es crucial. Esta línea asegura que la variable de control avance. Si no existiera, el contador siempre sería 1 y el bucle se ejecutaría infinitamente.

4. Una vez que el contador alcanza el valor de 6, la condición se vuelve falsa y el programa salta a la siguiente línea.
printf ("La suma es: %i\n", acumulador); imprime el resultado final de la suma, que es 15.

5. return 0; indica la finalización exitosa del programa principal.


🔁 **2. Estructura Repetitiva “Repetir…Hasta que” (DO–WHILE)**

✅ Definición: Es una estructura repetitiva que ejecuta las instrucciones primero, y luego evalúa la condición.
El ciclo continúa hasta que la condición se cumpla (o se vuelva verdadera).

⚙️ Cómo funciona:

- Ejecuta el bloque de instrucciones al menos una vez.

- Evalúa la condición.

- Si la condición aún no se cumple → repite el bloque.

- Termina cuando la condición sea verdadera.

🎯 Para qué sirve:

- Validación de datos: obligar al usuario a ingresar algo correctamente.

- Tareas que deben ejecutarse mínimo una vez sin importar la condición.

- Repeticiones basadas en una verificación al final.

**Ejemplo en diagrama de flujo**
El siguiente programa sirve para contar numeros positivos.

![Ejemplo usando DO-WHILE]()


**¿Como funciona?**


**Ejemplo aplicado en lenguaje C**
![Ejemplo usando DO-WHILE]()

**¿Como funciona?**

1. Inicialización: El programa inicializa un contador a cero. Este contador será la variable que acumule la cuenta de los números válidos.

2. Bucle Principal: Dentro del bloque do, el programa solicita y lee un número del usuario.

3. Evaluación Condicional: Inmediatamente después de leer la entrada, una estructura if anidada verifica si el número ingresado es mayor que cero (positivo).

- Si es positivo, se incrementa el contador.

- Si es cero o negativo, el contador se mantiene igual.

4. Control de Flujo: La condición while (numero > 0); se evalúa al final del ciclo.

- Si el último número ingresado fue positivo, el bucle repite el proceso (do).

- Si el usuario ingresa un número negativo o cero, la condición se vuelve falsa y la iteración se detiene.

5. Salida: Una vez terminado el bucle, el programa muestra la cantidad total de números positivos que fueron ingresados.

🔁 **3. Estructura Repetitiva “Para” (FOR)**
✅ Definición: Es una estructura controlada por un contador que repite un bloque de instrucciones un número específico y definido de veces.

⚙️ Cómo funciona:

- Se inicializa una variable (contador).

- El contador se compara con un límite.

- Si no se cumple el límite, ejecuta el bloque.

- Al terminar, el contador cambia automáticamente (incrementa o decrementa).

- Repite hasta alcanzar el límite.

🎯 Para qué sirve:

- Repetir acciones un número conocido de veces.

- Recorrer listas, arreglos o secuencias numéricas.

- Tareas con un inicio, fin y paso definidos.


**Ejemplo en Diagrama de Flujo**

![Ejemplo usando FOR]()

**¿Como funciona?**

1. Inicialización (Se ejecuta solo una vez)
Código: contador = 50;

- Acción: La variable contador se inicializa con el valor 50. Esto ocurre únicamente al comienzo del bucle.

2. Condición (Se verifica al inicio de cada ciclo)
Código: contador >= 1;

- Acción: Antes de que el código dentro de las llaves se ejecute, se verifica si el valor de contador es mayor o igual a 1.

- Si es Verdadero, el bucle continúa.

- Si es Falso (cuando contador llega a 0), el bucle se detiene y el programa salta a return 0;.

3. Incremento/Decremento (Se ejecuta al final de cada ciclo)
Código: contador--

- Acción: Después de que se ha ejecutado el cuerpo del bucle (la impresión del número), el valor de contador se decrementa en 1 (contador-- es equivalente a contador = contador - 1). Esto asegura que el bucle avance hacia su fin.

**Ejemplo aplicado en lenguaje C**

![Ejemplo usando for]()

**¿Como funciona?**
1. Inicialización (Inicio)
Código: contador <- 50

- Acción: La variable contador se inicializa con el valor de 50. Esto marca el punto de partida.

2. Condición (Hasta el Fin)
Código: Hasta 1

- Acción: Esta es la condición de parada. El bucle continuará ejecutándose mientras el valor del contador no supere (en este caso, no sea menor) que el valor final de 1.

3. Incremento/Decremento (Paso)
Código: Con Paso -1

- Acción: Después de cada ciclo de impresión, el valor del contador se decrementa en 1. Esto asegura la cuenta regresiva.

## 🎯 **Ejercicio combinando estructura condicional y repetitiva**  
*(Java o Python)*  
- 📝 **Descripción del problema**  
- 🔄 **Diagrama de flujo simplificado**  
- 💻 **Programa**  
- ✅ **Verificación**  

## ⚠️ **Principales dificultades** *en la aplicación de los contenidos*  
## 🤔 **Reflexión crítica** *de los aprendizajes de la unidad*  
## 🗂️ **Tareas entregadas**
