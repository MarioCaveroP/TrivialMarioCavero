# Trivial

## Problema 0

Extraemos el codigo duplicado a un unico metodo "nuevaPosicionJugador",
al que llamamos desde ambos sitios.

Creamos test unitario "si_al_principio_saco_un_1_voy_a_casilla_1"

## Problema 1

En el código ya existe un método “esJugable” que comprueba si hay más de 2 jugadores.
Creamos 2 tests para ese método, y desde “tirar dado” hacemos la comprobación y si solo hay 1 jugador
devolvemos una excepción. También hacemos un test para verificar el lanzamiento de la excepción

## Problema 2
Aquí podríamos seguir el mismo enfoque del problema anterior, pero como ahora tenemos un número de
jugadores delimitado entre 2 y 6, y no son muchas combinaciones, lo que haremos será crear tantos
constructores de la clase Game como posibles jugadores.

Esto nos obliga por diseño a tener un número correcto de jugadores, y además evitamos controlar mediante
excepciones el flujo de la ejecución, lo cual se considera un anti-patrón.

Lo hacemos con TDD

##Ejercicio 3

Existia un problema al salir de la carcel. Aunque se indicaba que el jugador estaba "saliendo
de la carcel" en realidad nunca se establecia enCasillaCastigo[[jugadorActual]] = false
Lo corregimos en el caso de sacar un numero impar.
Verificamos el resultado con tests

## Problema 4

Los nombres y contenidos de variables y funciones que indican si un jugador ha ganado
estan incorrecto o retorcidos. Arreglamos el "naming" e invertimos la logica para que se entienda
Verificamos con test.

## Problema 5

El código que sirve para pasar al siguiente jugador está repetido muchas veces. Extráelo a un método común.

## Problema 6 
Simplifica la función “respuestaCorrecta” extrayendo código duplicado.
