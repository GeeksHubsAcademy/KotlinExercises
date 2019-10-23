# KotlinExercises
Ejercicios de Kotlin
## 1º BLOQUE.
---

### Actividad 1
Escriba un método que imprima la representación de su parámetro entero en números romanos. Por ejemplo, si el parámetro es 1998, la salida debe ser MCMXCVIII

### Actividad 2
Realizar un programa que no pida un unidad en kb y nos haga la conversión a MB

### Actividad 3
Escriba un programa que calcule la media de N numéro enteros introducidos.

### Actividad 4 
Cree un programa que a partir de un entero calcule su serie Fibonacci

### Actividad 5
Escribe un programa que muestre tres apuestas de la quiniela en tres columnas para los 14 partidos y el pleno al quince (15 filas)

### Actividad 6
Realizar la carga de la cantidad de hijos de 10 familias. Contar cuantos tienen 0,1,2 o más hijos. Imprimir dichos contadores.


### Actividad 7
Escribir un programa que solicite ingresar 10 notas de alumnos y nos informe cuántos tienen notas mayores o iguales a 7 y cuántos menores.

### Actividad 8
Realizar un programa que permita cargar dos listas de 5 valores cada una. Informar con un mensaje cual de las dos listas tiene un valor acumulado mayor (mensajes "Lista 1 mayor", "Lista 2 mayor", "Listas iguales")
Tener en cuenta que puede haber dos o más estructuras repetitivas en un algoritmo

### Actividad 9
Desarrollar un programa que permita cargar n números enteros y luego nos informe cuántos valores fueron pares y cuántos impares.
Emplear el operador "%" en la condición de la estructura condicional

### Actividad 10
Crea una aplicación que nos pida la altura de la silla y nos dibuje por pantalla una silla con *. La única restricción que no debe ser menor de 7 ni mayor de 30 y la condición de que el asiento este situado la mitad + 1
```
Indicame la altura? 10
*
*
*
*
*
******
*    *
*    *
*    *
```
### Actividad 11
Crea una aplicación que nos pida la altura del arbol y nos dibuje por pantalla dicho arbol. Tiene que tener una altura mínima de 5
```
Indícame la altura? 5
    *
   *** 
  *****
 *******
*********
```

### Actividad 12
Estructura la aplicación 8 a un patrón MVC(Modelo Vista Controlador) estructurando la misma en diferentes paquetes(Modelo, Vista, Controlador)

## 2º BLOQUE.
**Todas las actividades a continuación se desarrollarán con el patrón MVC y separando en sus distintos "packages"**
---
### Actividad 1
Cree una clase Cuenta que almacena el saldo actual y proporciona los métodos getBalance para obtener el saldo y deposit para depositar fondos, withdrar para reitrar fondos y toString para devolver por pantalla el saldo actual, además de al menos un constructor. Escriba y pruebe la clase.

### Actividad 2
Queremos construir una aplicación que permita almacenar la información relevante sobre empresas y sus empleados:

La clase empresa tendrá como mínimo dos atributos: nombre de tipo String y anyodefundacion de tipo string.
La clase empleado tendrá como mínimo cuatro atributos: nombre de tipo String, apellidos de tipo String, fechanacimiento de tipo String y fechaContrato de tipo String El programa mostrará un menu que tendrá las siguientes opciones:
Crear nueva empresa.
Añadir empleado a empresa existente.
Listado de empresas.
Informacion de una empresa en particular.
Crear empleado.
Listado de empleados.
Información de un empleado en particular.
Salir. Se deberá implementar todo la funcionalidad en las clases para que la aplicación sea funciona.

### Actvidad 3
Declarar una clase abstracta Cuenta y dos subclases CajaAhorra y PlazoFijo. Definir las propiedades y métodos comunes entre una caja de ahorro y un plazo fijo y agruparlos en la clase Cuenta.
Una caja de ahorro y un plazo fijo tienen un nombre de titular y un monto. Un plazo fijo añade un plazo de imposición en días y una tasa de interés. Hacer que la caja de ahorro no genera intereses.
En la función main del programa definir un objeto de la clase CajaAhorro y otro de la clase PlazoFijo.

### Actividad 4
Agregar a la clase String un método imprimir que muestre todos los caracteres que tiene almacenado en una línea.
Codicar la función de extensión llamada "hasta" que debe extender la clase Int y tiene por objetivo mostrar desde el valor entero que almacena el objeto hasta el valor que llega como parámetro:
```
   fun Int.hasta(fin: Int) {
```
### Actividad 5
Plantear un data class llamado Dado con una única propiedad llamada valor. Sobreescribir el método toString para que muestre tantos asteriscos como indica la propiedad valor.

### Actividad 6

Definir un enum class almacenando como constante los nombres de varios países sudamericanos y como propiedad para cada país la cantidad de habitantes que tiene.
Definir una variable de este tipo e imprimir la constante y la cantidad de habitantes de dicha variable.


### Actividad 7
Crearemos una superclase llamada Electrodomestico con las siguientes características:

Sus atributos son precio base, color, consumo energético (letras entre A y F) y peso. Indica que se podran heredar.
Por defecto, el color sera blanco, el consumo energético sera B, el precio Base es de 200€ y el peso de 5 kg.
Los colores disponibles son blanco, metal, rojo, verde y azúl.
Los constructores que se implementarán serán:
Un constructor por defecto.
Un construcor con el precio y peso. El resto por defecto.
Un constructor con todos los atributos.
Los métodos que se implemntarán serán
Los metodos getter/setter de todos los atributos.
comprobarConsumoEnergetico(char letra): comprueba que la letra es correcta, sino es correcta usará la letra por defcto. Se inocará al crear el objeto y no será visible.
comprobarColor(String color): comprueba que el color es correcto sino lo es usa el color por defecto. Se invocará al crar el objeto y no será visible.
precioFinal() Según el consumo energetico, aumentará su prcio y según su tamaño también. Esta son la lista de precios LETRA
A -> 100 €
B -> 85 €
C -> 60 €
D -> 50 €
E -> 30 €
F -> 10 € TAMAÑO
ENTRE 0 Y 19 KG -> 10 €
ENTRE 20 Y 49 KG -> 50 €
ENTRE 50 Y 79 KG -> 80 €
MAYOR QUE 80 KG -> 100€
Crearemos una subclase llamada Lavadora con las siguientes características:

Su atributo es carga, además de los atributos heredados.
Por defecto, la carga es de 5 kg.
Los constructors que se implementarán serán:
Un constructor por defecto.
Un constructor con el precio y el peso. El resto por defecto.
Un constructor con la carga y el resto de atributos heredados. Recurda que debes llamar al constructor de la clase de padre.
Los métodos que implementarán serán:
Método get de carga.
precioFinal() : Si tiene una arga mayor de 30 kg, aumentará el precio 50 €, sino es así no se incrementará el precio. Llama al método padre y añade el código necesario. Recuerda que las condiciones que hemms visto en la clase Electrodoméstico también deben afectar al precio.
Crearmos una subclase llamada Televisión con las siguientes características:

Sus atributos son resolución en pulgadas y sintonizador TDT(booleano), además de los atributos heredados.
Por defecto, la resolución será de 20 pulgadas y el sintonizador será false.
Los constructores que se implemntarán serán
Un constructor por defecto.
Un constructor con el precio y peso. El resto por defecto.
Un constructor con la resolución, sintonizador TDT y el resto de atributos heredados. Recuerda que debes llamar al constructor de la clase padre.
Los métodos que se implemntará serán:
Método get de resolución y sintonizador TDT.
precioFinal() si tiene una resoloución mayor de 40 pulgadas, se incrementará el precio un 30 % y si tiene un sintoniador TDT incorporado, aumentará 50 €. Recuerda que las condiciones que hemos visto en la clase Electrdomestico también deben afectar al precio.
Ahora la clase ejecutable que

Cree un array de Electrodomésticos de 10 posiciones.
Asigna a cada posición un objto de las clases anteriores con los valores qu desees.
Ahora recorre este array y ejecuta el método precioFinal()
Deberás mostrar el precio de cada clase, es decir, el precio de todas las operaciones de todas las televisiones por un lado, el de las lavadoras por otro y la suma de los Electrodomesticos(puedes crear objetos Electrodomestico, pero recuerda que Televisión y Lavadora también son electrodomésticos). Recuerda el uso operador instanceof.
Crea la clase prueba donde lanzemos test de cada clase y método creado. Fucinomanento: Por ejmplo, si tenemos un Electrodoméstico on un precio final de 300, una lavadora de 200 y una televisión de 500, el resultado final será 1000 (300+200+500) 300 para electrodomésticos, 200 para lavadoras y 500 para televisión.

## 3º BLOQUE.
---

### Actividad 1

Se tiene la declaración del siguiente data class:
```
data class Articulo(val codigo: Int, val descripcion: String, var precio: Float)
```
Definir un Array con 4 elmentos de tipo Articulo.
Implementar dos funciones, una que le enviemos el Array y nos muestre todos sus componentes, y otra que también reciba el Array de artículos y proceda a aumentar en 10% a todos los productos.

### Actividad 2

Declarar una clase Dado que tenga como propiedad su valor y dos métodos que permitan tirar el dado e imprimir su valor.
En la main definir un Array con 5 objetos de tipo Dado.
Tirar los 5 dados e imprimir los valores de cada uno.

### Actividad 3

Crear una lista inmutable de 100 elementos enteros con valores aleatorios comprendidos entre 0 y 20.
contar cuantos hay comprendidos entre 1 y 4, 5 y 8 y cuantos entre 10 y 13.
Imprimir si el valor 20 está presente en la lista.

### Actividad 4

Confeccionar una clase que represente un Empleado. Definir como propiedades su nombre y su sueldo.
Definir una lista mutable con tres empleados.
Imprimir los datos de los empleados.
Calcular cuanto gasta la empresa en sueldos.
Agregar un nuevo empleado a la lista y calcular nuevamente el gasto en sueldos.

### Actividad 5

Cargar por teclado y almacenar en una lista inmutable las alturas de 5 personas (valores Float)
Obtener el promedio de las mismas. Contar cuántas personas son más altas que el promedio y cuántas más bajas

### Actividad 6

Confeccionar una agenda. Utilizar un MutableMap cuya clave sea de la clase Fecha:
```
data class Fecha(val dia: Int, val mes: Int, val año: Int)
```
Como valor en el mapa almacenar un String.
Implementar las siguientes funciones:
1) Carga de datos en la agenda.
2) Listado completo de la agenda.
3) Consulta de una fecha.
