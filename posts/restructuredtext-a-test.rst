.. title: reStructuredText a Test
.. slug: restructuredtext-a-test
.. date: 2018-02-11 17:29:13 UTC-06:00
.. tags: rst, mathjax
.. category: general, rst
.. link: 
.. description: 
.. type: text

.. contents:: Tabla de contenidos
.. section-numbering::



Este post está destinado a la práctica y aprendizaje del uso de ReStructuredText, veamos como nos va.

Párrafos
========

| Este es un párrafo corto.
|   Este es otro párrafo, está identado.
|
| Este es un tercer párrafo que contiene más texto. Se utiliza para ejemplificar el identado y la longitud, en pantalla, de los textos que aparecen en la página. Obviamente, habrá un salto de texto en el editor, más no en el resultado final
  ya que no habrá línea en blanco con respecto del cuarto párrafo.
| Aquí está el cuarto párrafo.

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


Definiciones
============

Igualdad
    Principio que reconoce la equiparación de todos los ciudadanos en derechos y obligaciones.

*Equidad*
    Justicia natural, por oposición a la letra de la ley positiva.

Field Lists
-----------

:what:
    Field lists map field names to field bodies, like database
    records.  They are often part of an extension syntax.  They are
    an unambiguous variant of RFC 2822 fields.

:how arg1 arg2:

    The field marker is a colon, the field name, and a colon.

    The field body may contain one or more body elements, indented
    relative to the field marker.

Block Quotes
------------

Block quotes consist of indented body elements:

    Mi teoría sobre la vida es que, ésta es una desmadre. Pero no dejes
    que te impresione... Jajajaja

    -- Will Santana


Preformato
==========

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


Secciones
=========

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


Media
=====


Imágenes
--------

De una tortuga, por ejemplo.

.. image:: /galleries/tortuga.jpg
   :height: 480
   :width: 640


Vídeos
------

Youtube:

.. youtube:: yYY06G4R7zY
   :width: 700
   :align: center

Vimeo:

.. vimeo:: 61620799
   :height: 300
   :align: left


Código
======

Código en Python, *con* números de línea.

.. code-block:: python
   :number-lines:

   def sieve_of_eratosthenes():
       factors = defaultdict(set)
       for n in count(2):
           if factors[n]:
               for m in factors.pop(n):
                   factors[n+m].add(m)
           else:
               factors[n*n].add(n)
               yield n

Código en Python, *sin* números de línea.

.. code-block:: python

   def sieve_of_eratosthenes():
       factors = defaultdict(set)
       for n in count(2):
           if factors[n]:
               for m in factors.pop(n):
                   factors[n+m].add(m)
           else:
               factors[n*n].add(n)
               yield n



Fórmulas
========

Para poder usar esta extensión, es necesario agregsar 'mathjax' a la sección tags
del documento. Recuerda que si agregas varios tags, deberán ir separados por comas.

Una identidad de Ramanujan
--------------------------

.. math::

   \frac{1}{(\sqrt{\phi \sqrt{5}}-\phi) e^{\frac25 \pi}} =
   1+\frac{e^{-2\pi}} {1+\frac{e^{-4\pi}} {1+\frac{e^{-6\pi}}
   {1+\frac{e^{-8\pi}} {1+\ldots} } } }


Ecuación de Maxwell's
---------------------

.. math::

   \nabla \times \vec{\mathbf{B}} -\, \frac1c\, \frac{\partial\vec{\mathbf{E}}}{\partial t} & = \frac{4\pi}{c}\vec{\mathbf{j}} \\
   \nabla \cdot \vec{\mathbf{E}} & = 4 \pi \rho \\
   \nabla \times \vec{\mathbf{E}}\, +\, \frac1c\, \frac{\partial\vec{\mathbf{B}}}{\partial t} & = \vec{\mathbf{0}} \\
   \nabla \cdot \vec{\mathbf{B}} & = 0


While displaying equations look good for a page of samples, the
ability to mix math and text in a paragraph is also important.
This expression :math:`\sqrt{3x-1}+(1+x)^2` is an example of an
inline equation. As you see, MathJax equations can be used this
way as well, without unduly disturbing the spacing between lines.


Fin del post.