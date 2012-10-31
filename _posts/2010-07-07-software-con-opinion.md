---
layout: post
title: Software con opinión
tags:
- Convention over Configuration
- Opinionated Software
- Programación
- rails
- Rails
- Ruby
status: publish
type: post
published: true
meta:
  _edit_last: '10779279'
  jabber_published: '1278485369'
  delicious: a:3:{s:5:"count";s:1:"0";s:9:"post_tags";s:0:"";s:4:"time";s:10:"1284704958";}
  _wpas_done_twitter: '1'
  _wpas_skip_yup: '1'
  reddit: a:2:{s:5:"count";s:1:"0";s:4:"time";s:10:"1284704959";}
---
En el desarrollo de software tener muchas opciones entre las que elegir puede ser algo positivo, sin embargo <a href="http://codigocomestible.com/2010/07/06/paralisis-por-analisis/">a veces tener demasiadas opciones también puede ser un problema</a>.

Pensemos, por ejemplo, en los frameworks de javascript. Existen docenas de ellos: jQuery, Prototype, Yahoo UI, Dojo, ExtJs,  GWT, MooTools... Todos son buenos y elegir la mejor opción es algo muy complicado: para encontrarla deberíamos pasar un tiempo considerable evaluando cada uno de ellos, sus ventajas y sus inconvenientes, y como solucionan los problemas que tenemos.

Pero, ¿merece la pena tanto esfuerzo? Probablemente no. Aunque haya un framework que sea inherentemente mejor que los demás, vamos a perder más tiempo buscándolo y evaluando posibles opciones, que si utilizásemos directamente el segundo o el tercer mejor framework, porque, entre los más conocidos todos son *suficientemente* buenos.

En mi opinión, la mejor solución para este problema es la que toma Ruby on Rails. Rails es *<a href="http://gettingreal.37signals.com/ch04_Make_Opinionated_Software.php">Opinionated Software</a>*, **software con opinión**. Cuando creamos una aplicación nueva con Rails, la aplicación viene ya **"con las pilas incluidas"**: ya tiene un framework javascript -prototype- una librería de testing, librería para fixtures , un motor de plantillas, un librería de ORM; la aplicación ya tiene una estructura: los controladores van en este directorio, las vistas en este otro; Rails utiliza *<a href="http://es.wikipedia.org/wiki/Convención_sobre_Configuración">Convention Over Configuration</a>* para darle nombre a las tablas en la base de datos, a las vistas y a los controladores; todas las tablas utilizan como clave principal un id autonumérico. Nada más empezar, el equipo de Rails ya ha tomado un montón de decisiones difíciles por ti.

Todas estas decisiones son discutibles, pero en la práctica resulta que en la inmensa mayoría de los casos, las decisiones que ha tomado el equipo de rails son *suficientemente* buenas. **Rails es software con opinión, dice: yo hago las cosas así. Si luego quieres cambiar cualquier cosa, puedes hacerlo**. Ruby es un lenguaje tan dinámico que eso no suele ser problema: aunque rails venga, por ejemplo, con su ORM -ActiveRecord- o su motor de plantillas -ERB-, se puede sustituir ActiveRecord por DataMapper o ERB por Haml. Yo, por ejemplo, cuando programo con Rails suelo utilizar jQuery en vez de Prototype, el framework javasacript que trae Rails por defecto.

Si lo hago es porque tengo claro lo que quiero y sé lo que estoy haciendo. Pero si no lo tienes claro, Rails ya te da un stack que funciona muy bien y te ahorrará muchas indecisiones y quebraderos de cabeza.
