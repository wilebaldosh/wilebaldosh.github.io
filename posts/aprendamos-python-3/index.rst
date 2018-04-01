.. title: Aprendamos Python 3
.. slug: aprendamos-python-3
.. date: 2018-03-31 14:10:43 UTC-06:00
.. tags: Python3
.. category: Python3
.. link: 
.. description: Aprendamos a programar en Python 3
.. type: text

**Artículo en proceso**
=======================

Vamos a ver algunos aspectos de este gran lenguaje de programación Python 3

Introducción
============

Este es un pequeño tutorial de Python que no debería tomar mucho tiempo en completarlo.
Asumo que ya tienes instalado Python, sino instálalo antes de comenzar.

Python interactivo
==================

Python incluye un programa que mostrará el resultado de cualquier comando Python que le introduzcas.
Jugar con código Python en una sesión interactiva como ésta es una manera estupenda de aprender el
lenguaje.

Arranca el intérprete.

* Si estás usando Mac OS X abre una Terminal y escribe *python3*, después presiona enter.

* Si estás usando Linux, abre una Terminal y escribe *python3*, después presiona enter.

* Si estás usando Windows, abre una consola y escribe python ó ve al menú de python y
  da clic sobre la opción del *IDLE (Python GUI)* de tu menú de Inicio.

Yo estoy utilizando Mac:
::

  $ python3
  Python 3.6.4 (default, Jan  6 2018, 11:51:59) 
  [GCC 4.2.1 Compatible Apple LLVM 9.0.0 (clang-900.0.39.2)] on darwin
  Type "help", "copyright", "credits" or "license" for more information.
  >>> 

Bien, ahora está corriendo y, ¿ahora qué?

Escribe esto: "Hola mundo!"
::

  >>> "Hola mundo!"
  'Hola mundo!'

¡Está vivo, vivo!
=================

¿Qué fue lo que pasó? ¿Acaso acabamos de escribir el programa “Hola Mundo” más corto
del mundo? No exactamente. La segunda linea sólo es la forma que tiene Python para
decirnos el resultado de la última expresión evaluada. Si queremos que el programa
escriba “Hola Mundo” necesitamos un poco más:
::

  >>> print("Hola mundo!")
  Hola mundo!
