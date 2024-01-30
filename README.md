# Librería computación cuántica: Números complejos CNYT

## **Estudiante:** Alexandra Moreno Latorre


Librería diseñada con el propósito de realizar operaciones entre números complejos.

Esta librería soporta las siguientes operaciones:

- Suma
- Producto
- Resta
- División
- Módulo
- Conjugado
- Conversión entre representaciones polar y cartesiano
- Retornar la fase de un número complejo.

## ¿Cómo se utiliza?

Se necesita conocer los números complejos que se desean operar y escoger correctamente las funciones que ya están marcadas y simplificadas para su correcto uso.

## Datos

Denotación

``` txt
(Número Real, Número Complejo)
```

De esta manera se representan los números complejos. Es necesario saber que para denotar números complejos se utiliza la letra **i**.


``` txt
2 + 1i
```
Ejemplo del ingreso de datos para realizar una operación:

(4, 7) , (2, 3)

De este modo el código realiza la operación correspondiente y entrega el resultado así:

2 , 4

## Contenido

### Archivos

En esta librería aparecen 4 archivos que el usuario puede usar

- ***.gitignore*** -> Es el archivo que excluye lo que no se quiere dentro del repositorio GitHub.
- ***README.md*** -> Es el archivo con documentación de software que contiene información acerca de otros archivos relacionados a la librería.
- ***TestCplx.py*** -> Es el archivo de testeo con diversos casos de prueba para corroborar que las funciones se hayan realizado correctamente y se puedan cambiar las variables y las respuestas para poder verificar un ejercicio realizado con otro programa.

### TestCplx.py

Contiene una breve información de los casos de cada operación entre números complejos.

``` Python
    def test_sumacplx(self):
        #Test 1. Suma entre números complejos
        #(3 + 5i) + (-2.6 + 6.8i) = 0.4 + 11.8i
        c1 = (3, 5)
        c2 = (-2.6, 6.8)
        suma = lc.sumacplx(c1, c2)
        self.assertAlmostEqual(suma[0], 0.4)
        self.assertAlmostEqual(suma[1], 11.8)
        # Test 2. Suma entre números complejos
        #(3 + 8i) + (-4 + 10.7i) = -1 + 18.7i
        c1 = (3, 8)
        c2 = (-4, 10.7)
        suma = lc.sumacplx(c1, c2)
        self.assertAlmostEqual(suma[0], -1)
        self.assertAlmostEqual(suma[1],18.7)
```
 
## Requisitos para usar la librería

Debe de poseer una versión ***Python*** superior a 3.5, adicionalmente debe de poseer la librería math instalada.
