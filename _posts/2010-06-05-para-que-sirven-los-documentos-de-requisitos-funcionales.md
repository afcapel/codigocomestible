---
layout: post
title: Para qué sirven los documentos de requisitos funcionales
tags:
- excusas
- modelo en cascada
- Programación
status: publish
type: post
published: true
meta:
  _edit_last: '10779279'
  jabber_published: '1275750440'
  _wp_old_slug: ''
  _wpas_done_twitter: '1'
  _wpas_skip_yup: '1'
  delicious: a:3:{s:5:"count";s:1:"0";s:9:"post_tags";s:0:"";s:4:"time";s:10:"1284365495";}
  reddit: a:2:{s:5:"count";s:1:"0";s:4:"time";s:10:"1284365497";}
---
El sello que certifica que se está siguiendo el modelo en cascada es el documento de requisitos funcionales. El documento funcional especifica, antes que se empiece a programar, como debe ser el software y qué es lo que debe hacer. En teoría, el desarrollador puede consultarlo para aclarar cualquier duda que tenga sobre cómo funciona el software.

Digo en teoría, porque en la práctica esto no suele suceder. Yo mismo he tenido mi buena ración de documentos funcionales, me ha tocado escribirlos y corregirlos, pero nunca los he utilizado para lo que se supone que están hechos: para aclarar mis dudas sobre como debe funcionar un programa.

Los documentos funcionales no parecen muy útiles. Algunos expertos en hacer buen software, como la gente de 37 Signals, <a href="http://gettingreal.37signals.com/ch11_Theres_Nothing_Functional_about_a_Functional_Spec.php">incluso piensan que no sirven de nada</a>. Pero, entonces, ¿por qué seguimos haciendo documentos funcionales?

La respuesta, como casi siempre que se reincide en un error claro, no es tanto técnica como psicológica.

A muchos desarrolladores o responsables de proyectos** les gustan los documentos de requisitos funcionales porque limitan su responsabilidad**. Hacer buen software que contente al cliente es algo complicado; cumplir un documento de requisitos funcionales es algo mucho más sencillo. El documento funcional es una especie de contrato de lo que el desarrollador se compromete a hacer: en vez de comprometerse a hacer un software de calidad que resuelva problemas reales, el desarrollador se compromete **sólo** a implementar lo que está escrito en el funcional.

Si el producto no funciona bien, o no resuelve los problemas del cliente, el desarrollador se siente eximido de responsabilidad: "*Mi programa cumple el funcional -dice-, si querían otra cosa, tenían que haberlo dicho en el documento funcional*". La culpa no es mía, sino del cliente, que no ha sabido escribir un buen documento funcional.

**Los documentos funcionales son la excusa perfecta para hacer software chapucero y luego echarle la culpa al cliente.**
