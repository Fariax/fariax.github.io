---
layout: post
title:  "Intro a Python"
subtitle: Una muy breve introducción a python (.zip)
tags: [Python]
date:   2019-09-09 18:00:00
last_modified_at: 2019-09-22 16:00:00
comments: true
---
Este tutorial pretende ser un _manual del cortapalos_ respecto a los conceptos mas básicos del lenguaje de programación [__Python__](https://www.python.org/).  Principalmente la idea es poder resumir de una forma muy rápida lo básico y fundamental del lenguaje para después ir adentrándonos en los conceptos clave que nos permitirán avanzar en el mundo de la ciencia de datos.

# ¿Que es python?

[__Python__](https://www.python.org/) es un lenguaje de programación interpretado cuya filosofía hace hincapié en una sintaxis que favorezca un código legible.

Se trata de un lenguaje de programación multiparadigma, ya que soporta orientación a objetos, programación imperativa y, en menor medida, programación funcional. Es un lenguaje interpretado, usa tipado dinámico y es multiplataforma.

Es administrado por la [__Python__](https://www.python.org/) Software Foundation. Posee una licencia de código abierto, denominada Python Software Foundation License, que es compatible con la GNU General Public License a partir de la versión 2.1.1, e incompatible en ciertas versiones anteriores.

>_Colaboradores de Wikipedia. Python [en línea]. Wikipedia, La enciclopedia libre, 2018 [fecha de consulta: 1 de julio del 2018]. Disponible en <https://es.wikipedia.org/w/index.php?title=Python&oldid=109027303>._

# ¿Como obtengo python?

[__Python__](https://www.python.org/) se puede obtener de varias maneras:

1. La primera y la mas común es ir al sitio web y descargarlo para tu sistema operativo favorito.
2. Si usas Linux o MAC ya viene instalado en el sistema, sin embargo hay que tener cuidado por que la versión que usaremos en este tutorial sera la 3.7 y normalmente viene instalada la versión 2.7.
3. La tercera forma es a través de de alguna distribución de [__Python__](https://www.python.org/) como:
    - [Anaconda](https://www.anaconda.com/distribution/)
    - [Winpython](https://winpython.github.io/)
    - [Portable Python](https://sourceforge.net/projects/portable-python/)
    
    
>__ATENCION__: [__Python__](https://www.python.org/) tiene una versión 2 y una 3 que cambian mucho desde el punto de vista sintáctico.  Una de los cambios mas significativos es el uso de `print` que en la versión 3 se utiliza con paréntesis y en la versión 2 se utiliza sin paréntesis.

En este tutorial usaremos la versión 3.7 en un sistema operativo Linux con python3 instalado a través de nuestro gestor de paquetes que puede ser yum, dnf, zypper, apt, etc...

# El primer programa

Vamos a imprimir algo por pantalla y para eso vamos a ejecutar [__Python__](https://www.python.org/), en una consola de comandos, vamos a escribir lo siguiente y debería entregar una salida como se detalla a continuación:

``` bash
~$ python3
Python 3.7.3 (default, Apr  3 2019, 05:39:12) 
[GCC 8.3.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> 
```

Ahora mostramos un mensaje por pantalla:

``` bash
>>> # Vamos a imprimir un mensaje en pantalla
>>> print("Hola, esto es un resumen de python...")
Hola, esto es un resumen de python...
>>> _
```

# Pongamonos un poco mas serios: variables

Las variables son contenedores en memoria que nos permiten almacenar valores que vamos utilizando en nuestros programas, el contenido de estas puede ser modificadas en cualquier momento (osea, puede _variar_, de ahí su nombre de "variable") y se asignan mediante el operador _igual_ `=`.

``` python
>>> variable = 20
```

Si invocamos a la variable por su nombre nos devuelve el valor 20

``` python
>>> variable
20
```

## Algunos datos a tener en cuenta sobre las variables:

- Por convención las variables en [__Python__](https://www.python.org/) se deben escribir en notación snake case: __esta_es_una_variable__.

- Las variables pueden llamarse de cualquier forma con caracteres alfanuméricos y guiones bajos.

- No se pueden utilizar las siguientes 28 palabras reservadas:

<table align="center" width="60%">
    <tr>
        <td>and</td><td>del</td><td>is</td><td>for</td><td>raise</td><td>assert</td><td>if</td>
    </tr>
    <tr>
        <td>else</td><td>elif</td><td>from</td><td>lamda</td><td>return</td><td>break</td><td>global</td>
    </tr>
    <tr>
        <td>not</td><td>try</td><td>class</td><td>except</td><td>or</td><td>while</td><td>continue</td>
    </tr>
    <tr>
        <td>exec</td><td>import</td><td>yield</td><td>def</td><td>finally</td><td>in</td><td>print</td>
    </tr>
</table>

# Python como calculadora:

[__Python__](https://www.python.org/), desde su linea de comandos se puede utilizar como una buena calculadora, esto gracias a que posee una serie de operadores matemáticos que nos permiten realizar operaciones.

Los _Operadores Matemáticos_ en [__Python__](https://www.python.org/) son:

Operación | Símbolo
-- | --
Operador Suma | `+` 
Operador Resta | `-` 
Operador Multiplicación | `*`
Operador División | `/`
Operador División entera | `//`
Operador Modulo | `%`
Operador Exponente | `**`

Revisemos como se usan estos operadores:


## Operador Suma: `+`

Corresponde a la operación de suma entre dos o mas números o variables.

``` python
>>> # Suma de numeros
>>> suma = 2 + 2
>>> print("La suma de los dos numeros es: ", suma)
La suma de los dos numeros es: 4

>>> # Suma de variables
>>> var_1 = 2
>>> var_2 = 5
>>> suma = var_1 + var_2
>>> print("La suma de las dos variables es: ", suma)
La suma de las dos variables es: 7 
```


## Operador Resta: `-`

Corresponde a la operación resta entre dos o mas números o variables

``` python
>>> # Resta de numeros
>>> resta = 7 - 3
>>> print("La resta de los dos numeros es: ", resta)
La resta de los dos numeros es: 4

>>> # Resta de variables
>>> var_1 = 2
>>> var_2 = 5
>>> resta = var_1 - var_2
>>> print("La resta de las dos variables es: ", resta)
La resta de las dos variables es: -3
```

## Operador Multiplicación: `*`

Corresponde a la operación multiplicación entre dos o mas números o variables.

``` python
>>> # Multiplicacion de numeros
>>> producto = 5 * 2
>>> print("El producto de los dos numeros es: ", producto)
El producto de los dos numeros es: 10

>>> # Resta de variables
>>> var_1 = 3
>>> var_2 = 5
>>> producto = var_1 * var_2
>>> print("El producto de las dos variables es: ", producto)
El producto de las dos variables es: 15
```

## Operador división: `/`

Corresponde a la operación división entre dos números o variables, y siempre entrega un numero flotante (float) o decimal.

``` python
>>> # Division de numeros
>>> cociente = 6 / 2
>>> print("El cociente de los dos numeros es: ", cociente)
El cociente de los dos numeros es: 3.0

>>> # Division de variables
>>> var_1 = 3
>>> var_2 = 5
>>> cociente = var_1 / var_2
>>> print("El cociente de las dos variables es: ", cociente)
El cociente de las dos variables es: 0.6
```

## Operador división entera: `//`

Se representa por dos signos de barra o slash: `//`, entrega la parte entera de la división obviando la parte decimal y siempre entrega un numero entero (int).

``` python
>>> # Division entera de numeros
>>> cociente = 6 // 2
>>> print("El cociente de los dos numeros es: ", cociente)
El cociente de los dos numeros es: 3

>>> # Division entera de variables
>>> var_1 = 3
>>> var_2 = 5
>>> cociente = var_1 // var_2
>>> print("El cociente de las dos variables es: ", cociente)
El cociente de las dos variables es: 0
```

## Operador modulo: `%`

Se representa por el signo porcentaje: `%`, entrega el resto de una división entre dos números o variables y siempre entrega un numero entero (int).

``` python
>>> # Modulo de numeros
>>> resto = 6 % 2
>>> print("El resto de la división de los dos numeros es: ", resto)
El resto de la division de los dos numeros es: 0

>>> # Modulo de variables
>>> var_1 = 3
>>> var_2 = 5
>>> resto = var_1 % var_2
>>> print("El resto de la división de las dos variables es: ", cociente)
El resto de la division de las dos variables es: 3
```

## Operador exponente: `**`

Se representa por dos asteriscos: `**` y entrega el resultado de la enésima potencia.

``` python
>>> # Potencia de numeros
>>> potencia = 6**2
>>> print("Seis elevado a dos es: ", potencia)
Seis elevado a dos es: 36

>>> # Potencia de variables
>>> var_1 = 3
>>> var_2 = 5
>>> potencia = var_1**var_2
>>> print("var_1 elevada a var_2 es: ", potencia)
var_1 elevada a var_2 es: 243
```

# Tipos de datos básicos

Las diferentes operaciones que podemos hacer con las variables dependen directamente del tipo de dato que estas almacenan, por ejemplo, cuando sumamos dos números, obtenemos un resultado numérico, pero ¿que pasa si sumáramos dos letras?, ¿o una letra con un numero?

[__Python__](https://www.python.org/) maneja automáticamente los tipos de datos que pasamos a nuestras variables, sin embargo es muy necesario conocer los tipos que existen para poder responder las preguntas que hicimos hace un momento.

- En [__Python__](https://www.python.org/) tenemos cuatro tipos de datos base: strings, enteros, de coma flotante y booleanos.  
- Podemos conocer el tipo de dato llamando a la función: `type()`

## Strings 

Son secuencias alfanuméricas que permiten almacenar valores de forma literal, son el tipo de datos que permite almacenar oraciones o nombres.

```python
>>> string = "Eso es un string"
>>> cadena = "Esto es otro string pero ahora tiene un par de números como el 3 y 7"
>>> type(string)
<class 'str'>
>>>type(cadena)
<class 'str'>
```

## Integers 

Son datos numéricos enteros que pueden ser positivos, negativos o un cero.

```python
>>> un_entero = 10
>>> type(un_entero)
<class 'int'>
>>> otro_entero = -1
>>> type(otro_entero)
<class 'int'>
```
## Floats

Son números que tienen una componente entera y otra decimal, también se le conoce como "_números con coma flotante_" y la parte decimal se separa por un __punto__ `.`.

```python
>>> un_float = 6.5
>>> type(un_float)
<class 'float'>
```
## Booleanos

Representan a los dos valores posibles en el álgebra booleana, `True` o `False`, son ademas, el resultado de una expresión lógica.

```python
>>> true_var = True
>>> type(true_var)
<class 'bool'>
>>> false_var = False
>>> type(false_var)
<class 'bool'>
```

# Respondamos las preguntas:

## ¿que pasa si sumáramos dos letras?

``` python
>>> # Suma de letras
>>> suma = 'a' + 'b'
>>> print("La suma es: ", suma)
El producto de los dos numeros es: 'ab'
```

## ¿o una letra con un numero?

``` python
>>> # Multiplicacion de letras por numeros
>>> producto = x * 3
>>> print("El resultado es: ", producto)
El producto de los dos numeros es: 'xxx'
```

