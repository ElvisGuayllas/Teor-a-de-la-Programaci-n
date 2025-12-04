# 📚 **TEMAS PRINCIPALES**

## 🔹 Tipos de Estructuras Condicionales 

Las **estructuras condicionales** son las herramientas que permiten a un programa *"tomar decisiones"*. Rompen la ejecución lineal (paso 1, paso 2, paso 3) y crean bifurcaciones en el camino:  
> **"Si pasa X, haz esto; si no, haz lo otro."**

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

**Ejemplo en Lenguaje C:**  
![Ejemplo de la condicion IF](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/ifc.png)

**¿Cómo funciona?**  
🔢 **1.** El programa pide al usuario que ingrese su edad.  
💾 **2.** Guarda ese número en la variable `edad`.  
🔍 **3.** Luego verifica si la edad es **mayor o igual a 18**.  
✅ **4.** Si lo es, muestra el mensaje: *"Usted es mayor de edad"*.  
⏭️ **5.** Si es menor de 18, no muestra nada más.

> *Programa sencillo para verificar si una persona es mayor de edad a base de la edad ingresada.*

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

**Ejemplo en lenguaje C:**  
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
**Uso ideal:**  
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

