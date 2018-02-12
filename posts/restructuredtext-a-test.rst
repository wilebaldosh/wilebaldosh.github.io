.. title: reStructuredText a Test
.. slug: restructuredtext-a-test
.. date: 2018-02-11 17:29:13 UTC-06:00
.. tags: rst
.. category: General, rst
.. link: 
.. description: 
.. type: text


Este post está destinado a la práctica y aprendizaje del uso de ReStructuredText, veamos como nos va.

Párrafos:
=========

Este es un párrafo corto.

  Este es otro párrafo, está identado.

Este es un tercer párrafo que contiene más texto. Se utiliza para ejemplificar el identado y la longitud, en pantalla, de los textos que aparecen en la página. Obviamente, habrá un salto de texto en el editor, más no en el resultado final ya
que no habrá línea en blanco con respecto del cuarto párrafo.

Aquí está el cuarto párrafo.

Estilos de texto
================

*Itálica*

**Negrita**

``Monoespacio``


Listas
======

1. Primer elemento del primer nivel.
2. Segundo elemento del primer nivel.

  a) Primer elemento del segundo nivel.
  b) Segundo elemento del segundo nivel.

    i) Primer elemento en el tercer nivel.
    ii) Segundo elemento en el tercer nivel.

  c) Tercer elemento del segundo nivel.

    i) Tercer elemento en el tercer nivel, pero depende del inciso 'c' en el segundo nivel.

3. Tercer elemento del primer nivel.

Lista nueva:

* Primer nivel, con asterisco.

  - Segundo nivel, con guión.

    + Tercer nivel, con signo de suma.

  - Regresamos al segundo nivel, con otro guión.


Definiciones:
=============

Igualdad
    Principio que reconoce la equiparación de todos los ciudadanos en derechos y obligaciones.

*Equidad*
    Justicia natural, por oposición a la letra de la ley positiva.


Preformato:
===========

Ahora, por ejemplo, veremos un texto dentro de un recuadro::

    Espacios, líneas nuevas, líneas en blanco y toda clase de markup
      (como *esto* o \esto) se muestra tal cual.
  Vean, dejé un nivel identado
  (pero no mucho)

Este texto ya está fuera del recuadro porque no tiene identación, como en el texto dentro de la caja.

::

  Este es otro texto dentro de otra caja y el par de dos puntos `::` fueron removidos automáticamente

  Al parecer

Este otro texto está fuera de la caja.


Secciones:
==========

Capítulo I
==========

Sección 1.1.
------------

Subsección 1.1.1.
~~~~~~~~~~~~~~~~~

Sección 1.2.
------------

Capítulo II
===========


