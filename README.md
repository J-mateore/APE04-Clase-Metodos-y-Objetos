# APE-04-POO-JAVA

![](https://img.shields.io/badge/JAVA-orange?style=for-the-badge&logo=java&logoColor=white) ![](https://img.shields.io/badge/GITHUB-black?style=for-the-badge&logo=github&logoColor=white)

Este repositorio contiene la resolución de los 18 ejercicios prácticos propuestos en la **Guía APE 4** para la asignatura de **Algoritmos y Lógica de Programación**.

---

## 📋 Datos Informativos

| Campo | Detalle |
| :--- | :--- |
| **Estudiante** | Mateo Salazar |
| **Carrera** | Ingeniería de Software |
| **Semestre** | Primer Semestre |
| **Materia** | Algoritmos y Lógica de Programación |
| **Lenguaje** | Java |
| **Entorno de Desarrollo** | Visual Studio Code |

---

## Resolución de Ejercicios

---

### Ejercicio 1: Notas del curso

#### Enunciado:
Crear la clase Estudiante con los atributos nombre, nota1, nota2, nota3 y promedio. En main, crear 5 instancias, calcular el promedio de cada una e imprimirlas una debajo de otra con el formato nombre : promedio, agregando Aprobado (7 o más), Supletorio (de 5 a 6.99) o Reprobado (menos de 5). Al final, imprimir cuántos estudiantes aprobaron.

#### Descripción de la solución:
Se creó la clase Estudiante calculando el promedio automáticamente desde el constructor. En la clase principal se instanciaron 5 estudiantes en un arreglo, evaluando su rendimiento mediante un bucle e identificando el estado académico de cada uno junto con el conteo final de aprobados.

#### Evidencia de codificación:
*<img width="421" height="383" alt="image" src="https://github.com/user-attachments/assets/5c4d2f7d-92e9-4002-8376-9c97f129d079" />
*

---

### Ejercicio 2: Inventario de una tienda

#### Enunciado:
Crear la clase Producto con nombre, precio y stock. Crear 4 productos e imprimirlos con el formato nombre : precio. Simular la venta de 3 unidades de dos de ellos, mostrar “Reponer” junto a cada producto que quede con menos de 5 unidades e imprimir el valor total del inventario (suma de precio por stock).

#### Descripción de la solución:
Se definió la clase Producto con un método para reducir el stock tras cada venta y calcular el valor total. En el método principal se imprimió el catálogo inicial, se simularon las ventas indicadas y se recorrió el arreglo para alertar los productos con bajo stock y calcular la suma global del inventario.

#### Evidencia de codificación:
*<img width="478" height="484" alt="image" src="https://github.com/user-attachments/assets/c5d9d328-8433-491e-814b-71ed48014ee7" />
*

---

### Ejercicio 3: Veterinaria

#### Enunciado:
Crear la clase Mascota con nombre, especie, edad y peso. Crear 3 mascotas e imprimirlas con el formato nombre : especie : peso, mostrando “Revisar peso” si pesan más de 20 kg. Luego escribir Mascota m4 = m1;, sumar 1 a m4.edad, imprimir m1.edad y explicar en un comentario por qué cambió.

#### Descripción de la solución:
Se implementó la clase Mascota filtrando mediante condiciones los casos que superan los 20 kg. Adicionalmente, se demostró el concepto de asignación de referencias en memoria igualando `m4 = m1`, evidenciando que al alterar la edad desde `m4`, la variable `m1` se modifica por apuntar al mismo objeto en el Heap.

#### Evidencia de codificación:
*<img width="453" height="294" alt="image" src="https://github.com/user-attachments/assets/3301764d-a9c6-41f3-8351-ec7f3e57512a" />
*

---

### Ejercicio 4: Cuenta de ahorro

#### Enunciado:
Crear la clase Cuenta con titular y saldo. Crear 2 cuentas, una con 200 y otra con 350. Con un while, depositar 50 por mes en cada cuenta hasta que llegue a 500, imprimiendo cada mes con el formato titular : saldo, y al final cuántos meses necesitó cada una (6 y 3).

#### Descripción de la solución:
Se creó la clase Cuenta almacenando el saldo inicial de cada titular. Mediante un bucle `while`, se realizaron depósitos mensuales de $50 incrementando un contador de meses de manera independiente hasta alcanzar la meta de $500, imprimiendo el desglose mes a mes de los saldos.

#### Evidencia de codificación:
*<img width="465" height="603" alt="image" src="https://github.com/user-attachments/assets/ba15834d-baef-4e88-a0ad-05b7139a3a79" />
*

---

### Ejercicio 5: Biblioteca

#### Enunciado:
Crear las clases Libro (titulo, autor, disponible) y Socio (nombre, librosPrestados). Crear 4 libros y 2 socios, registrar que el primer socio presta 2 libros y el segundo presta 1 (disponible = false y aumentar librosPrestados), y al final imprimir cada libro con el formato titulo : Disponible o titulo : Prestado, cada socio con el formato nombre : librosPrestados y cuántos libros quedan disponibles.

#### Descripción de la solución:
Se modeló la relación entre las clases Libro y Socio mediante un método de préstamo que actualiza el estado de disponibilidad e incrementa los préstamos del socio. Al final, se recorren las colecciones para imprimir el catálogo actualizado, los registros por socio y el total de libros disponibles.

#### Evidencia de codificación:
*<img width="445" height="440" alt="image" src="https://github.com/user-attachments/assets/06827e45-d554-423e-86b9-65a5df910b61" />
*

---

### Ejercicio 6: Identificación de tipos de retorno

#### Enunciado:
Dado el siguiente método, explica por qué genera un error de compilación en Java y cómo lo corregirías:
public int calcularArea(double base, double altura) {
    double area = base * altura;
    System.out.println("El área es: " + area);
}

#### Descripción de la solución:
Se identificó y diagnosticó el error de compilación por la ausencia de la sentencia return requerida por el tipo de retorno int de la firma, además de la incompatibilidad de tipos entre double e int. Se indicó la corrección modificando el tipo de retorno a double y agregando la instrucción de retorno en la clase Main6.

#### Evidencia de codificación:
<img width="1098" height="195" alt="image" src="https://github.com/user-attachments/assets/01319197-4511-4aae-aedb-4a466762f620" />
*

---

### Ejercicio 7: Métodos void para acciones directas

#### Enunciado:
Crea un método dentro de una clase llamada Bienvenida que reciba como parámetro un nombre de usuario (String nombre) y un número entero (int edad), y que imprima directamente en consola: "Hola [nombre], tienes [edad] años. ¡Bienvenido al sistema!". ¿Qué tipo de retorno debe llevar este método y por qué?

#### Descripción de la solución:
Se diseñó el método implementando el tipo de retorno void debido a que su responsabilidad exclusiva es la ejecución de una acción directa de impresión por consola sin devolver valores numéricos o de texto. Se estructuró la clase Main7 para recibir los parámetros correspondientes y mostrar el mensaje formateado.

#### Evidencia de codificación:
<img width="1095" height="205" alt="image" src="https://github.com/user-attachments/assets/cc5d5b5e-919b-4235-9990-391a743863d7" />
*

---

### Ejercicio 8: Parámetros vs. Argumentos

#### Enunciado:
En el siguiente fragmento de código, identifica claramente cuáles son los parámetros y cuáles son los argumentos, explicando brevemente la diferencia entre ambos:
public double multiplicar(double x, double y) {
    return x * y;
}
// Llamada:
double res = miObjeto.multiplicar(4.0, 5.5);

#### Descripción de la solución:
Se documentó la diferencia conceptual detallando que los parámetros (x, y) son variables locales definidas en la firma del método dentro de la clase Main8, mientras que los argumentos (4.0, 5.5) son los valores reales suministrados al momento de realizar la llamada de ejecución.

#### Evidencia de codificación:
<img width="1103" height="205" alt="image" src="https://github.com/user-attachments/assets/2a5fbb76-d753-496c-b3ee-f9fe92d60378" />
*

---

### Ejercicio 9: El comportamiento del paso por valor

#### Enunciado:
Analiza el siguiente bloque de código. Si la variable numero original en el main vale 10 antes de llamar al método, ¿cuál será su valor impreso en consola después de ejecutar el método? Explica por qué.
public void incrementar(int n) {
    n = n + 5;
}

#### Descripción de la solución:
Se explicó el comportamiento del paso por valor en Java para tipos de datos primitivos, demostrando que al enviar una variable a un método se crea únicamente una copia temporal, por lo que la variable original en el método principal Main9 permanece inalterada con un valor de 10.

#### Evidencia de codificación:
<img width="1097" height="241" alt="image" src="https://github.com/user-attachments/assets/76022d31-6535-43f3-9737-737cfcbbb171" />
*

---

### Ejercicio 10: Creación de un método con múltiples parámetros

#### Enunciado:
Agrega un nuevo método a la clase Calculadora llamado calcularPromedio que reciba tres notas de tipo double (n1, n2, n3), calcule el promedio sumándolas y dividiéndolas entre 3, y retorne el resultado final.

#### Descripción de la solución:
Se implementó un método dentro de la clase Main10 con tipo de retorno double, configurando tres parámetros de entrada y utilizando la precedencia de operadores mediante paréntesis para asegurar la correcta división de la sumatoria total de las notas.

#### Evidencia de codificación:
<img width="1126" height="222" alt="image" src="https://github.com/user-attachments/assets/c22c1103-9832-4a49-bb33-122b641e3a13" />
*

---

### Ejercicio 11: Validación de datos (Control de errores)

#### Enunciado:
Modifica el método de la potencia o crea un método verificarEdad que reciba una edad (int edad). Si la edad es menor a 0 o mayor a 120, debe imprimir "Edad inválida" y retornar false. Si es correcta, debe retornar true.

#### Descripción de la solución:
Se desarrolló un método con tipo de retorno booleano (boolean) en la clase Main11 incorporando una estructura condicional if-else para establecer los límites lógicos permitidos de edad, controlando los errores de ingreso e imprimiendo el mensaje de advertencia correspondiente.

#### Evidencia de codificación:
<img width="1106" height="257" alt="image" src="https://github.com/user-attachments/assets/83175d61-d2dd-48ec-9837-91ce8f1e8bf4" />
*

---

### Ejercicio 12: Completar la Clase Producto

#### Enunciado:
Rellena los espacios vacíos (___) en la siguiente clase para que cumpla con calcular el valor total del inventario de un producto:
public class Producto {
String nombre;
int stock;
double precioUnitario;
public __ calcularValorTotal() {
__ stock * precioUnitario;
}
}

#### Descripción de la solución:
Se completaron los espacios vacíos asignando el tipo de retorno double en la firma del método debido a la multiplicación de datos decimales e enteros, y utilizando la palabra reservada return para devolver el cálculo global del inventario dentro de la clase Main12.

#### Evidencia de codificación:
<img width="1111" height="250" alt="image" src="https://github.com/user-attachments/assets/872c828e-864a-41c8-b8c5-73eaff9bbd23" />
*

---

### Ejercicio 13: Instanciación e Invocación en el Main

#### Enunciado:
Escribe el código necesario dentro del método main de una clase principal para:
a. Instanciar un objeto de la clase Producto llamado p.
b. Asignarle un stock = 10 y un precioUnitario = 25.5.
c. Llamar al método calcularValorTotal(), guardar el resultado en una variable llamada totalInventario e imprimirla en consola.

#### Descripción de la solución:
Se programó el flujo de instanciación formal del objeto p mediante el operador new en la clase principal Main13, realizando la asignación directa de atributos y la posterior invocación del método de cálculo para almacenar y desplegar el resultado en la consola.

#### Evidencia de codificación:
<img width="1096" height="263" alt="image" src="https://github.com/user-attachments/assets/a98c4f45-9472-4e45-9c87-7862554fc1ad" />
*
