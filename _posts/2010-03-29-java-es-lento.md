---
layout: post
title: ¿Java es lento?
tags:
- benchmarks
- c++
- java
- jvm
- Programación
- rendimiento
status: publish
type: post
published: true
meta:
  _edit_last: '10779279'
  _wpas_done_twitter: '1'
  delicious: a:3:{s:5:"count";s:1:"0";s:9:"post_tags";s:0:"";s:4:"time";s:10:"1285005679";}
  _wpas_skip_yup: '1'
  reddit: a:2:{s:5:"count";s:1:"0";s:4:"time";s:10:"1282013190";}
---
Lo que voy a decir no es nada muy novedoso. En realidad, lo más llamativo es que en pleno año 2010 haya que seguir repitiendo algunas verdades tan trilladas. Pero me temo que sigue siendo necesario: muchos profesionales de la informática repiten una y otra vez el antiguo mantra de que *Java es demasiado lento*. Y no me refiero sólo al chaval que leyó hace diez años algo sobre Java en una revista de informática. Yo se lo he oído repetir incluso a varios responsables de importantes proyectos, de esos proyectos que cuestan **mucho** dinero, unos profesionales de los que cabría esperar, al menos, algunas nociones básicas de como funciona una plataforma. Y, sin embargo, ahí están repitiendo los mismos clichés que en 1996, como si el mundo no hubiera cambiado.

¿Como surgió el mito de que Java es lento?

Cuando Java nació en el año 1995, las aplicaciones web aún eran ciencia ficción. En esa época <a href="http://www.jcmit.com/memoryprice.htm">un megabyte de memoria costaba 30$</a>  ( &asymp; 30.000 dólares 1GB) y un procesador Pentium a 120Mhz <a href="http://processortimeline.info/proc1995.htm">salía a 935$ a precio de mayorista</a>.

El desarrollo se centraba principalmente en aplicaciones de escritorio y los principales rivales de Java eran C y C++. A diferencia de C o C++, el código fuente de Java no se compila directamente a código máquina, sino que se transforma primero en un formato intermedio, el bytecode, que luego es interpretado por la máquina virtual.

Los primeros benchmarks no tardaron en llegar e indicaban claramente que un programa Java se ejecutaba entre 10 y 30 veces más lento que un programa equivalente en C++.

Esto era Java alrededor de 1996, hace catorce años, es decir, una eternidad en el mundo de la informática.

Hoy día las cosas han cambiado mucho. En primer lugar, la propia máquina virtual de Java (la JVM) ha evolucionado pasmosamente hasta convertirse en una pieza de software altamente optimizada.

La máquina virtual de Java cuenta hoy en día con compiladores JIT (Just In Time) que traducen el bytecode a código nativo de la máquina. Además, la JVM también puede monitorizar qué partes del programa se ejecutan más a menudo y optimizar la compilación para el uso real que se le da a la aplicación. Es lo que se conoce como Optimización Adaptativa, y es una ventaja muy importante con la que no cuentan los compiladores tradicionales.

Esas son las dos principales mejoras de las que se ha beneficiado la máquina virtual de Java, <a href="http://en.wikipedia.org/wiki/Java_performance#Virtual_machine_optimization_techniques">pero no las únicas</a>.

El resultado de todos estos cambios, es que Java, a día de hoy es tan rápido o más que C++. Dependiendo de quién haga el benchmark, Java resulta ser un poco más rápido o un poco más lento.

Por ejemplo, el <a href="http://shootout.alioth.debian.org/u32/which-programming-languages-are-fastest.php">The Computer Language Benchmarks Game </a>es un juego de benchmarks basados en pruebas de cálculo aritmético sencillas donde se comparan distintos lenguajes. En esas pruebas Java, cuando descontamos el tiempo de arranque de la máquina virtual, aparece en los primeros puestos, sólo por detrás de C, C++ y ATS, sacando bastante ventaja a otros lenguajes como C# y barriendo literalmente a los lenguajes dinámicos como Ruby, Python o PHP. Java resulta ser unas 80 veces más rápido que PHP.

No obstante, los benchamarks que miden calculos aritméticos sencillos no se correlacionan demasiado bien con el rendimiento de sistemas complejos, donde la interacción entre distintas partes de la aplicación, las librerías de E/S, o la concurrencia son muy importantes. En benchmarks donde se comparan sistemas complejos, Java se muestra a menudo más rápido que C++. Por ejemplo, algunos <a href="http://www.devshed.com/c/a/BrainDump/Tomcat-Benchmark-Procedure/1/">benchmarks indican que el servidor web Apache Tomcat (escrito en Java) puede ser más rápido que su primo Apache httpd</a> (escrito en C).

Pero todo esto tiene una importancia relativa, porque el mayor cambio que ha habido en el mundo de Java no ha sucedido dentro de la plataforma, sino fuera de ella. **Los principales rivales de Java para crear aplicaciones web ya no son C y C++ sino, más bien, PHP, Ruby o Python**. Y Java es mucho más rápido que cualquiera de estas tres alternativas. Y lo que es peor: tampoco importa. Ruby, por ejemplo, es lo suficientemente rápido para hacer aplicaciones web con un buen rendimiento. <a href="http://codigocomestible.com/2010/03/28/mitos-escalabilidad-aplicaciones-web/">Como ya he explicado en otra ocasión, el hecho de que Ruby sea más lento que Java no lo hace menos escalable</a>.

Pero, me diréis, "*existen muchas aplicaciones en Java leeeentas y pesadas, yo las he visto. Fíjate en Eclipse, me puedo tomar un café mientras arranca.*" Y es cierto. Pero eso no es culpa de la plataforma Java, sino de los programadores que crearon esos engendros. Durante muchos años, J2EE (el entorno en el que se han desarrollado la mayoría de las aplicaciones Java empresariales) ha sido una plataforma sobrecargada de ornamentos inútiles y pesados. No es de extrañar que una aplicación que usa los EJB 2.0 distribuidos vaya lenta. Pero el fallo está en utilizar EJBs distribuidos, no en el lenguaje de programación ni en la máquina virtual.

Y eso nos lleva a la verdadera razón de por qué ha sobrevivido tanto tiempo la monserga de que Java es lento: es una excusa perfecta para hacer software malo. Los desarrolladores pueden hacer un truño de aplicación, y cuando no funcione bien se encogerán de hombros y dirán: '*qué quieres, no es culpa mía, ya sabes que Java es lento*'.
