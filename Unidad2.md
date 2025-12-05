# 📚 TEMAS PRINCIPALES

## 🔹 Tipos de Estructuras Condicionales 

Las **estructuras condicionales** permiten que un programa *"tome decisiones"*, rompiendo la ejecución lineal (paso 1, paso 2, paso 3) para crear bifurcaciones en el flujo:  
**"Si ocurre X, haz esto; si no, haz lo otro."**

Los **tipos principales** que encontrarás en lenguajes como C, Java, Python, etc., son:

### 1. Condicional Simple (If) ✅

Es la estructura más básica: evalúa una condición y, si es verdadera, ejecuta un bloque de instrucciones; si no, continúa sin hacer nada.

**Lógica:**  
*"Si llueve, llevo paraguas."*  
*(Si no llueve, continúo caminando.)*

**Ejemplo en diagrama de flujo:**  
![Ejemplo de la condición IF](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/if.png)

**¿Cómo funciona?**  
1. Se declara una variable `edad` de tipo **entero** para guardar la edad de la persona.  
2. Se muestra el mensaje *"Ingrese su edad:"* y se captura el valor ingresado en la variable `edad`.  
3. Se evalúa si `edad` es **mayor o igual a 18**. Si es verdadero, se imprime *"Usted es mayor de edad"*.  
4. El algoritmo termina con `FinAlgoritmo`.  

**Ejemplo en lenguaje C:**  
![Ejemplo de la condición IF en C](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/ifc.png)

**Funcionamiento:**  
- Se solicita la edad al usuario y se guarda en `edad`.  
- Se verifica si `edad >= 18`.  
- Si es verdadero, muestra el mensaje: *"Usted es mayor de edad"*.  
- Si es falso, no muestra nada adicional.

---

### 2. Condicional Doble (If - Else) 🔄

Define qué hacer en ambos casos: si la condición se cumple, se ejecuta una acción; si no, otra distinta. **Ambas nunca se ejecutan simultáneamente.**

**Lógica:**  
*"Si tengo dinero, compro el juego. Si no (Else), solo miro la demo."*

**Ejemplo en diagrama de flujo:**  
![Ejemplo de la condición If - Else](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/D.%20de%20Flujo%20elseif.png)

**¿Cómo funciona?**  
1. PSeInt simula el `else if` con anidación de bloques (`SiNo + Si`).  
2. Si la condición principal es falsa, el flujo entra en `SiNo` para evaluar la siguiente condición.  
3. Se requieren múltiples `FinSi` para cerrar cada nivel abierto.  
4. Entrada/salida manejada con `Leer` y `Escribir`.

**Ejemplo en lenguaje C:**  
![Ejemplo en C del If - Else](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/else-if.png)

- El `if-else if` en C funciona como una cadena secuencial.  
- Si la primera condición falla, el programa evalúa la siguiente.  
- Al cumplirse alguna condición, el programa sale inmediatamente del bloque.

---

### 3. Condicional Múltiple (If - Else If) 🪜

Una escalera de condiciones que se prueban secuencialmente hasta encontrar una verdadera.

**Lógica:**  
*"¿Es rojo? No. ¿Entonces verde? No. ¿Entonces azul? Sí."*

**Ejemplo en diagrama de flujo:**  
![Ejemplo condicional múltiple](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/DF%20Condicional%20M%C3%BAltiple.png)

**¿Cómo funciona?**  
1. Se define la variable como **numérico entero**.  
2. Se lee el dato del usuario.  
3. Se verifica si es negativo; si sí, muestra error y termina.  
4. Si no, verifica categorías sucesivas (**Niño**, **Adolescente**, **Adulto**).  
5. Si ninguna coincide, imprime por descarte **"Adulto Mayor"**.  
6. Se cierra cada bloque con `FinSi`.

**Ejemplo en lenguaje C:**  
![Ejemplo condicional múltiple en C](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/Condicional%20M%C3%BAltiple.png)

- Programa espera dato numérico.  
- Verifica si menor que cero (error).  
- Evalúa categorías en orden con `else if`.  
- Imprime la categoría correspondiente o **"Adulto Mayor"**.

---

### 4. Selección Múltiple (Switch / Case) 🎛️

Compara una variable con casos específicos para igualdades; es más limpio que múltiples `else if`.

**Usos ideales:**  
- Menús de opciones  
- Días de la semana  
- Códigos de error  

**Ejemplo en diagrama de flujo:**  
![Ejemplo con Switch](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/case%20Df.png)

**¿Cómo funciona?**  
1. Se leen tres variables: dos números y un operador (carácter).  
2. Ejecuta la instrucción `Segun operador Hacer`.  
3. Busca la coincidencia exacta con el valor del operador.  
4. Ejecuta la operación correspondiente y muestra resultado.  
5. Incluye controles como evitar división por cero con estructura anidada.  
6. Si no hay coincidencia válida, muestra mensaje de error.

**Ejemplo en lenguaje C:**  
![Ejemplo con Switch en C](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/case%20c.png)

- Variables de tipo `float` y `char` definidas.  
- Solicita y lee valores del usuario.  
- Evalúa `switch(operador)`.  
- Ejecuta operación y usa `break;` para salir del `switch`.  
- Controla errores en casos inválidos.

---

# ✅ Estructuras Repetitivas (Tipos y Ejercicios en Diagrama de Flujo y C)

Las estructuras repetitivas, también llamadas bucles o iteraciones, permiten ejecutar un conjunto de instrucciones múltiples veces según una condición o un número fijo.

Sirven para automatizar tareas repetitivas sin escribir código duplicado.

---

### 1. Estructura Repetitiva “Mientras” (WHILE) 🔁

**Definición:** Repite un bloque mientras la condición sea verdadera. Evalúa la condición antes de ejecutar el bloque.

**¿Cómo funciona?**  
- Evalúa la condición.  
- Si es verdadera, ejecuta el bloque.  
- Repite hasta que sea falsa.

**¿Para qué sirve?**  
- Para ciclos con número desconocido de repeticiones.  
- Repetir hasta que ocurra un evento o valor.  
- Controlar bucles con condiciones lógicas.

**Ejemplo diagrama de flujo:**  
![Ejemplo con WHILE](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/mientras%20DF%20(1).png)

**Funcionamiento:**  
- Inicializa variables `contador` y `acumulador` en 0.  
- Mientras `contador <= 5`: suma `contador` a `acumulador` y aumenta `contador` en 1.  
- Al terminar, imprime suma total (15).

**Ejemplo en C:**  
![WHILE en C](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/mientras%20c.png)

---

### 2. Estructura Repetitiva “Repetir…Hasta que” (DO–WHILE) 🔁

**Definición:** Ejecuta instrucciones primero y luego evalúa la condición. Repite hasta que la condición sea verdadera.

**¿Cómo funciona?**  
- Ejecuta bloque al menos una vez.  
- Evalúa condición.  
- Repite si condición es falsa.  
- Termina si condición es verdadera.

**¿Para qué sirve?**  
- Validar datos obligando a ingresar correctamente.  
- Asegurar ejecución mínima de una acción.  
- Repeticiones con evaluación al final.

**Ejemplo diagrama de flujo:**  
![Ejemplo avec DO-WHILE](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/do-while%20DF.png)

**Funcionamiento:**  
- Lee números positivos e incrementa contador.  
- Termina al ingresar número ≤ 0.  
- Imprime cantidad de números positivos.

**Ejemplo en C:**  
![Ejemplo DO-WHILE en C](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/do-while%20C.png)

---

### 3. Estructura Repetitiva “Para” (FOR) 🔁

**Definición:** Controlada por contador, repite un bloque un número definido de veces.

**¿Cómo funciona?**  
- Inicializa contador.  
- Compara con límite.  
- Ejecuta bloque si condición verdadera.  
- Incrementa/decrementa contador.  
- Repite hasta límite.

**¿Para qué sirve?**  
- Repetir un número conocido de veces.  
- Recorrer listas o arreglos.  
- Tareas con inicio, fin y paso definido.

**Ejemplo diagrama de flujo:**  
![Ejemplo FOR](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/FOR%20DI.%20F.png)

**Funcionamiento:**  
- Inicializa `contador = 50`.  
- Mientras `contador >= 1`, imprime valor y decrementa en 1.  
- Termina cuando `contador` es 0.

**Ejemplo en C:**  
![FOR en C](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/FOR%20C.png)

---

## 🎯 Ejercicio combinado: estructura condicional y repetitiva  
*(Java o Python)*

- 📝 Descripción del problema  
- 🔄 Diagrama de flujo simplificado  
- 💻 Programa  
- ✅ Verificación  

---

## ⚠️ Principales dificultades en la aplicación  
## 🤔 Reflexión crítica sobre los aprendizajes  
## 🗂️ Tareas entregadas
¿Quieres que te ayude también con la mejora o creación de algún código o diagrama para acompañar este texto?

agregale emojis, debe ser atractivo y bonito, no cambies el contenido original solo mejoralo en orden y atractivo
Claro, aquí tienes el texto mejorado usando Markdown con emojis para hacerlo más atractivo y ordenado, manteniendo el contenido original:

text
# 📚 **TEMAS PRINCIPALES**

## 🔹 Tipos de Estructuras Condicionales 

Las **estructuras condicionales** permiten que un programa *"tome decisiones"*, rompiendo la ejecución lineal (paso 1, paso 2, paso 3) para crear bifurcaciones en el flujo:  
💡 **"Si ocurre X, haz esto; si no, haz lo otro."**

Los **tipos principales** que encontrarás en lenguajes como C, Java, Python, etc., son:

---

### 1. Condicional Simple (If) ✅

La estructura más básica: evalúa una condición y, si es verdadera, ejecuta un bloque de instrucciones; si no, continúa sin hacer nada.

**Lógica:** ☔  
*"Si llueve, llevo paraguas."*  
*(Si no llueve, continúo caminando.)*

**Ejemplo en diagrama de flujo:**  
![Ejemplo de la condición IF](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/if.png)

**¿Cómo funciona?**  
1. 🔢 Se declara una variable `edad` de tipo **entero** para guardar la edad.  
2. ⌨️ Se muestra el mensaje *"Ingrese su edad:"* y se captura el valor en la variable `edad`.  
3. ✅ Se evalúa si `edad >= 18`. Si es verdadero, se imprime *"Usted es mayor de edad"*.  
4. 🏁 Termina el algoritmo con `FinAlgoritmo`.  

**Ejemplo en lenguaje C:**  
![Ejemplo de la condición IF en C](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/ifc.png)

**Funcionamiento:**  
- 👤 Solicita la edad del usuario.  
- 💾 Guarda el valor en `edad`.  
- 🔍 Verifica si `edad >= 18`.  
- ✅ Si es verdadero, muestra el mensaje.  
- ⏭️ Si no, continúa sin mostrar nada más.

---

### 2. Condicional Doble (If - Else) 🔄

Define acciones para ambos casos: si la condición se cumple, ejecuta una acción; si no, otra distinta. **Ambas nunca se ejecutan a la vez.**

**Lógica:** 💰🎮  
*"Si tengo dinero, compro el juego. Si no (Else), solo miro la demo."*

**Ejemplo en diagrama de flujo:**  
![Ejemplo de la condición If - Else](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/D.%20de%20Flujo%20elseif.png)

**¿Cómo funciona?**  
1. 🔗 PSeInt simula el `else if` con anidación de bloques (`SiNo + Si`).  
2. 🔍 Si la condición principal es falsa, el flujo pasa a `SiNo` para evaluar la siguiente.  
3. 🔒 Se requieren múltiples `FinSi` para cerrar niveles abiertos.  
4. 📥 Entrada y salida se manejan con `Leer` y `Escribir`.

**Ejemplo en lenguaje C:**  
![Ejemplo en C del If - Else](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/else-if.png)

- 🔁 La estructura `if-else if` es una cadena secuencial.  
- ⚡ Si la primera condición falla, evalúa la siguiente.  
- 🚫 Si se cumple una, sale del bloque inmediatamente.

---

### 3. Condicional Múltiple (If - Else If) 🪜

Una escalera de condiciones que se prueban una tras otra hasta encontrar una verdadera.

**Lógica:** 🎨  
*"¿Es rojo? No. ¿Entonces verde? No. ¿Entonces azul? Sí."*

**Ejemplo en diagrama de flujo:**  
![Ejemplo condicional múltiple](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/DF%20Condicional%20M%C3%BAltiple.png)

**¿Cómo funciona?**  
1. 🔢 Define dato como **numérico entero**.  
2. ⌨️ Lee el dato del usuario.  
3. 🚨 Verifica si es negativo; si sí, muestra error y termina.  
4. 👶 Verifica categoría "Niño".  
5. 🧒 Verifica "Adolescente".  
6. 🧑 Verifica "Adulto".  
7. 👴 Por descarte, imprime "Adulto Mayor" si ningún filtro anterior se cumple.  
8. 🔒 Cierra bloques con `FinSi`.

**Ejemplo en lenguaje C:**  
![Ejemplo condicional múltiple en C](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/Condicional%20M%C3%BAltiple.png)

- 🤔 Espera dato numérico.  
- 🚫 Error si dato < 0.  
- 🔄 Evalúa categorías con `else if`.  
- ✅ Imprime categoría o "Adulto Mayor".

---

### 4. Selección Múltiple (Switch / Case) 🎛️

Compara una variable con valores específicos para igualdades, logrando código más limpio que múltiples `else if`.

**Usos ideales:**  
- 📋 Menús de opciones  
- 📅 Días de la semana  
- ❗ Códigos de error  

**Ejemplo en diagrama de flujo:**  
![Ejemplo con Switch](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/case%20Df.png)

**¿Cómo funciona?**  
1. 🔢 Se leen tres variables: dos números y un operador.  
2. ⚙️ Se usa `Segun operador Hacer`.  
3. 🔍 Busca coincidencia exacta con operador.  
4. ✅ Ejecuta operación y muestra resultado.  
5. 🛡️ Controla división por cero con estructura anidada.  
6. 🚫 Si no hay coincidencia, muestra error.

**Ejemplo en lenguaje C:**  
![Ejemplo con Switch en C](https://github.com/ElvisGuayllas/Teor-a-de-la-Programaci-n/blob/main/imagenes/case%20c.png)

- 🔢 Variables definidas (`float` y `char`).  
- ⌨️ Solicita y lee datos.  
- ⚙️ Evalúa `switch(operador)`.  
- ✅ Ejecuta operación y usa `break;` para salir.  
- 🚫 Maneja errores en casos inválidos.

---

# ✅ **Estructuras Repetitivas (Tipos y Ejercicios en Diagrama de Flujo y C)** 🔁

Las estructuras repetitivas permiten ejecutar instrucciones varias veces según una condición o cantidad fija, automatizando tareas sin repetir código.

---

### 1. Estructura Repetitiva “Mientras” (WHILE) 🔄

**¿Para qué sirve?**  
- 🔍 Ciclos con número desconocido de repeticiones  
- ⏳ Esperar hasta que ocurra un evento o condición  
- 🧠 Controlar bucles basados en lógica condicional  

**¿Cómo funciona?**  
- ⚡ Evalúa la condición antes del ciclo  
- ✅ Ejecuta el bloque si la condición es verdadera  
- 🔁 Repite la evaluación y el bloque hasta que la condición sea falsa  

---

### 2. Estructura Repetitiva “Repetir…Hasta que” (DO–WHILE) 🔄

**¿Para qué sirve?**  
- ✅ Validación debido a la ejecución mínima garantizada  
- 📝 Asegurar que se ejecute al menos una vez una acción  
- 🔄 Repeticiones basadas en condición evaluada al final  

**¿Cómo funciona?**  
- 🔁 Ejecuta primero el bloque sin condiciones  
- 🔍 Evalúa la condición tras ejecutar el bloque  
- 🚦 Repite si la condición no se cumple; termina si sí  

---

### 3. Estructura Repetitiva “Para” (FOR) 🔄

**¿Para qué sirve?**  
- 🔢 Repetir un número conocido y fijo de veces  
- 📋 Recorrer listas, arreglos o secuencias numéricas  
- 🛠️ Automatizar tareas con inicio, fin y paso definidos  

**¿Cómo funciona?**  
- 🎬 Inicializa una variable contador  
- 🔎 Evalúa la condición límite antes de ejecutar  
- 🔄 Ejecuta el bloque, luego cambia el contador (incrementa/decrementa)  
- 🛑 Repite hasta cumplir la condición límite  

---

## 🎯 Ejercicio combinado: estructura condicional y repetitiva *(Java o Python)*

- 📝 Descripción del problema  
- 🔄 Diagrama de flujo simplificado  
- 💻 Código del programa  
- ✅ Verificación y validación de resultados  

---

## ⚠️ Principales dificultades en la aplicación  
- 🤔 Entender la evaluación correcta de la condición para evitar bucles infinitos  
- 📊 Controlar correctamente las variables de contador y acumulador  
- 🧩 Combinar estructuras condicionales y repetitivas sin errores lógicos  

---

## 🤔 Reflexión crítica sobre los aprendizajes  
- ✅ Profundización en el control del flujo de ejecución  
- 🔄 Comprensión práctica de la iteración y la toma de decisiones en código  
- 🚀 Aplicación concreta para resolver problemas reales y optimizar código

---

## 🗂️ Tareas entregadas  
- 📚 Informes escritos de ejercicios  
- 💻 Código fuente comentado  
- ✅ Ejercicios de práctica resueltos y verificados  

