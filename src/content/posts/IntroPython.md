---
title: "Introducción Python"
date: 2022-09-08T12:28:00+02:00
draft: false
author: Blitty
year: "2022"
month: "2022/09"
categories:
- Competitiva
tags:
- Tutorial
- python
---

¿Cómo leer de la entrada estándar y escribir en la salida estándar en C?

Antes que nada, debéis de saber que python es un lenguaje de programación de alto nivel, con tipado dinámico esto quiere decir que una variable puede adquirir diferentes tipos de valores.
<!--more-->

En los problemas que vamos a ver a lo largo de la rama siempre nos van a pedir que leamos datos de la **entrada estándar (stdin)** y que una vez hayamos hecho los cálculos pertinentes los imprimamos en la **salida estándar (stdout)**.

Para poder leer de la entrada estándar en python usaremos la función `input(prompt)`. *prompt* es un argumento que sirve para mostrar por pantalla algo específico al usuario. En el caso de Programación competitiva esto no es tan importante ya que es el propio ordenador el que te manda unos datos de forma estructurada, algo que tienes que tener en cuenta.

```py
x = input('¿Cuantos años tienes?')
```

Si ejecutamos esa instrucción veremos que aparece por pantalla `¿Cuantos años tienes?`  y espera a que tu respondas.

Una cosa a tener en cuenta siempre, es que `input` nos devuelve siempre un valor de tipo string aunque insertemos un valor numérico. Por lo tanto, para poder hacer esta conversión, usaremos la función `type()`.

```py
x = input()
print(type(x))
```

Se usa la función `print` para imprimir por pantalla, esto es lo que le llama **salida estándar**.

Como podréis observar, por salida tendrémos `<class 'str'>` aunque insertemos un valor numérico.

En caso de querer obtener el valor numérico de la entrada, podemos usar las funciones `int()` o `float()`. En caso de insertar un valor no numérico e intentar hacer la conversión a entero o con coma flotante, veréis que dará un error.

```python
x = input()
i = int(x)
f = float(x)
print(type(x))
```

Si x es un valor numérico las funciones funcionan sin ningún error. Sin embargo, si se mete un valor con coma flotante y se intenta obtener el valor entero, no se puede usar `int()`, ya que dará un error similar al del string. Ya que primero tendrás que pasar el valor cogido por la entrada (x) a coma flotante con `float()` y luego convertirlo a `int()`.

Por último y para curiosidad del expectador, mostraremos cómo imprimir por pantalla con una variable y strings. Hay diferentes formas de hacerlo, pero la favorita personal es usando `f` de **formating**. Os dejo un ejemplo:

```py
x = 15
y = 3.0

print(f'{x} + {y} = {x + y}\nChulo :D')
```

Más información:
- [Built in functions](https://docs.python.org/3/library/functions.html)
- [Input, Output](https://docs.python.org/3/tutorial/inputoutput.html)
