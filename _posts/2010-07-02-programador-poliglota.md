---
layout: post
title: El programador políglota
tags:
- java
- Lenguajes
- Máquina Virtual
- Programación
- Ruby
status: publish
type: post
published: true
meta:
  _edit_last: '10779279'
  jabber_published: '1278073991'
  _wp_old_slug: ''
  delicious: a:3:{s:5:"count";s:1:"0";s:9:"post_tags";s:0:"";s:4:"time";s:10:"1284408499";}
  _wpas_done_twitter: '1'
  _wpas_skip_yup: '1'
  reddit: a:2:{s:5:"count";s:1:"0";s:4:"time";s:10:"1284408500";}
---
Cada vez que programadores que provienen de distintos entornos se juntan para crear un nuevo proyecto surge la cuestión de qué lenguaje se va a utilizar, a la que suele seguir el inevitable flamewar sobre qué lenguaje es mejor. En seguida aparecen los viejos tópicos: java es lento, php sólo sirve para hacer aplicaciones sencillas, ruby no escala, erlang... ¿qué es eso de erlang?, etcétera.

 Estas discusiones rara vez llegan a un resultado provechoso, y no sólo porque los argumentos utilizados muchas veces no tienen ningún fundamento, sino porque la pregunta -¿qué lenguaje es mejor?- está mal planteada: **Los lenguajes no suelen ser mejores o peores por sí mismos, sino solamente más o menos adecuados para ciertas tareas**.

Los lenguajes son herramientas. ¿Qué herramienta es mejor, un destornillador o una llave inglesa? Depende de si quieres atornillar un tornillo o enroscar una tuerca. Dice el proverbio chino: *al que tiene un martillo todo le parecen clavos*. Yo digo que antes de utilizar ese martillo para desenroscar una tuerca, el desarrollador debería plantearse si no habrá  alguna herramienta más adecuada para lo que quiere hacer.

Nos guste o no, la realidad de la web nos ha enfrentado con el hecho de que **un sólo lenguaje ya no basta**. Antiguamente era posible hacer una aplicación de escritorio completa usando sólo C, C++ o Java. En cambio, para hacer una aplicación web medianamente decente, hay que conocer el lenguaje en el que se programe el backend -ya sea ruby, php, java o c#-, pero además es inevitable tener conocimientos de SQL, javascript, css, html... Eso como mínimo. Repito: **en el mundo web un sólo lenguaje ya no nos basta**.

Y este punto no sólo se aplica a la diferencia entre el backend y el frontend de una aplicación web que, al fin y al cabo, son ámbitos distintos y por lo tanto parece natural que utilicemos lenguajes distintos. También dentro del servidor puede tener sus ventajas que utilicemos varios lenguajes de programación.

Los entornos de ejecución modernos, como la máquina virtual de Java o el CLR de .NET, hacen que los distintos lenguajes puedan convivir y entenderse entre ellos. Por ejemplo, la máquina virtual de Java puede ejecutar código escrito en Java, Ruby, Scala, Groovy, Clojure, Python, PHP, Javascript, Ada, Cobol, etcétera. <a href="http://en.wikipedia.org/wiki/List_of_JVM_languages">La lista es larga.</a> Y no sólo eso: yo puedo utilizar JRuby, por ejemplo, para llamar a código escrito en Java o en Scala desde mi programa escrito en Ruby.** Gracias a la máquina virtual, las barreras entre lenguajes son cada vez más pequeñas** y Ruby puede entenderse perfectamente con Java.

Un ejemplo claro es el <a href="http://www.grails.org/">framework web Grails</a>. Está pensado para utilizarse en Groovy, pero su núcleo está construido sobre Spring e Hibernate. Es decir, tenemos un framework web escrito en Groovy que se apoya en librerías escritas en Java. Y el resultado funciona muy bien.

En su libro <a href="http://oreilly.com/catalog/9780596519544">*The Productive Programmer*</a>, <a href="http://www.nealford.com/">Neal Ford</a> llama a este enfoque **programación políglota**. ¿Qué es la programación políglota? Muy sencillo: se trata de utilizar en cada momento el lenguaje más adecuado para la tarea que haya que llevar a cabo. El programador políglota es aquel que tiene en su repertorio gran cantidad de herramientas -lenguajes-, conoce bien sus puntos fuertes y sus limitaciones, y sabe qué herramienta hay que utilizar para cada tarea.
