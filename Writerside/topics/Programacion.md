# Python 101: For beginners
---
Python es un lenguaje de programación de alto nivel, con una sintaxis simple y según los programadores "tan sencillo como hablar inglés".

Las aplicaciones de Python son muy bastas y muy variadas gracias a la cantidad de librerías y repositorios de la comunidad.

----

Python is a high level language, with an easy syntaxis and like the programmers says "It's simple as speaking English".

Python applications are varied thanks to the number of libraries and community repo's.

----

**For example:** *Web Development, Data Science, Bioinformatics, Image Processing, etc.*

---

![imagen](img2.jpg){thumbnail="true"}{ width=450 height=300}

Dicha facilidad y posibilidad de aplicaciones, han convertido a Python es un lenguaje de programación muy popular.

Its ease of use and applications have made Python a very popular programming language.

# **Características**
----


* Lenguaje interpretado
>Python es un lenguaje interpretado, lo que significa que ejecuta directamente el código línea por línea, de forma que la línea de código siguiente no puede ser ejecutada sino hasta que la línea anterior finalice su ejecución. Si existen errores en el código del programa, su ejecución se detiene.

* Lenguaje de alto nivel
>Esto implica que es más cercano a los idiomas humanos que otros lenguajes de programación. Por lo tanto, los programadores no deben preocuparse sobre sus funcionalidades subyacentes, como la arquitectura y la administración de la memoria.

* Ordenado por jerarquía
>Python no utiliza llaves. En su lugar, utiliza sangría para organizar los bloques

* Case-Sentive
<tip> Tiene la capacidad de diferenciar entre mayúsculas y minúsculas al momento de definir o invocar una variable, función, objeto, etc.</tip>

<note>
Por ejemplo:
 VARIABLE ≠ variable ≠ Variable
</note>

# **Sintaxis**
---
Para usar cualquier lenguaje de programación, es necesario conocer dos cosas, las acciones asociadas a ciertas palabras y la sintaxis que rige la ejecución del lenguaje, básicamente, el léxico y la semántica.

### Variables:
Para definir una variable en Python es necesario tener algunas consideraciones para hacerlo de forma correcta.

La comunidad de Python llegó a la convención de usar el "*snake_case*" como la forma mas popular de nombrar variables, funciones, objetos, etc.

Tener en cuenta que las variables jamas pueden empezar a ser definidad con un numero o simbolo, solo letras.

```python
Por ejemplo:

Formas correctas:

  variable = 1
  new_variable = "Hello World"
  variable1 = "Hola"
  
 ```
```python

Formas incorrectas:

  new variable = 10
  "Hello World" = variable
  1ra_variable = 1

```
---

# Tipos de Datos
----
En el extenso mundo de la programación existen diferentes tipos de datos y el lenguaje Python, no es la excepción, como ya se mencionó estamos trabajando con un lenguaje orientado a objetos, donde cada tipo de dato es una clase de objeto, por lo cual, si usamos numeros, es un dato, si usamos letras, es un dato, si usamos bases de datos, tambien son un dato.

Para introducirnos a los datos, podemos empezar con los tipos de datos principales y los mas usados en los programas básicos

## **int( )**
>El tipo de dato *int* hace referencia los *Integers*, números enteros reales positivos o negativos, de forma que no cuentan con decimales o puntos.

```python
num = 1
num_1 = 2
new_num = 10
```
>Tambien es posible convertir otros tipos de datos en enteros haciendo uso de la función int(*valor*), donde *valor* es el dato que se desea convertir en un número entero.
```python
variable = 10.0  #Este es un dato tipo float( )
number = "2"   #Este es un dato tipo str( )
num = int(variable)  #Se convierte a entero con int( )
number = int(number)  #Se convierte a entero con int( ) y podemos guardar en la misma variable
print(num)
>> 10
print(number + num)
>> 12
```

## **float( )**

>El tipo de dato *float* hace referencia los *Floats*, números decimales reales, estos siempre tienen un punto decimal o".0" después del número

```python
num = 1.0
num_1 = 2.5
new_num = 10.065
```
>También es posible convertir otros tipos de datos en floats haciendo uso de la función float(*valor*), donde *valor* es el dato que se desea convertir en un número decimal.

```python
variable = 5  #Este es un dato tipo int( )
num = float(variable)  #Se convierte a entero con float( )
print(num)
>> 5.0
```
## **str( )**
>El tipo de dato *float* hace referencia los *Floats*, números decimales reales positivos o negativos, estos siempre tienen un punto decimal o ".0" después del número
```python
num = 1.0
num_1 = 2.5
new_num = 10.065
```
>Para convertir datos varios en strings es necesario el uso de la función str(*valor*), donde *valor* es el dato que se desea convertir en una cadena.
```
variable = 5  #Este es un dato tipo int( )
number = 10.5   #Este es un dato tipo float( )
num = str(variable)  #Se convierte a una cadena con str( )
number = str(number)  #Se convierte a una cadena con str( )
print(num)
>> 5.0
print(num + number)  # Las cadenas no se suman, se concatenan (unen)
>> 510.5
```

## **Otros datos**:
Además de los datos mencionados con anterioridad, existen muchos más con características similares y otras particulares para cada tipo, pero que tienen en común es la función de conversión, dada por el nombre del tipo de dato seguido de los paréntesis.

```python
For example:
booleanos: bool( )  # Valores lógicos [1, 0]:[True, False]
listas: list( )  # Colección de datos
tuplas: tuple( )  # Colección de datos
set: set( ) # Conjunto de datos
diccionarios: dict( ) # Conjunto de datos formato {llave : valor}
```
