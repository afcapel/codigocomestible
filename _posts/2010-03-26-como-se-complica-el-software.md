---
layout: post
title: Cómo se complica el software
tags:
- ágil
- complejidad
- Programación
- software
status: publish
type: post
published: true
meta:
  _edit_last: '10779279'
  delicious: a:3:{s:5:"count";s:1:"0";s:9:"post_tags";s:0:"";s:4:"time";s:10:"1283620664";}
  _wpas_done_twitter: '1'
  reddit: a:2:{s:5:"count";s:1:"0";s:4:"time";s:10:"1282012434";}
  _wpas_skip_yup: '1'
---
Cuando se inicia el diseño de una aplicación los desarrolladores siempre piensan que todo saldrá bien. En la imaginación del desarrollador el sistema es claro y sencillo, cada pieza encaja en su sitio y todo funciona como una máquina perfectamente engranada.

Sin embargo, el software lioso y mal diseñado, en el que todo es más complicado de lo que debería, también existe. ¡Y tanto qué existe!  Cualquier desarrollador conoce al menos una aplicación compleja y confusa, un verdadero lío inmantenible. En cambio, lo contrario es una rareza desconocida: una aplicación que peque de ser más sencilla de lo que debería. ¿Quién ha visto algo así?

Si los desarrolladores de software aspiran a la sencillez, ¿qué es lo que acaba convirtiendo al software en un embrollo pegajoso y sucio? ¿Qué pasa durante el proceso de desarrollo de software para que el hermoso y sencillo diseño inicial acabe convertido en un nudo gordiano? ¿Cuales son los pasos que desencadenan la catástrofe?

Para entenderlo, podemos fijarnos en otros campos donde la calidad del producto se degrada imperceptiblemente.

Imaginemos, por ejemplo, una empresa de reparto a domicilio de pizzas. La empresa hace unas pizzas de muy buena calidad que gustan al público y aumenta cada año sus beneficios hasta que toca un techo que es difícil superar (simplemente, porque la mayoría de sus clientes potenciales ya están comprando el producto). Entonces puede surgir algún ejecutivo listillo -y **siempre** aparecerá un ejecutivo listillo- que, armado de gráficos con colores llamativos y de un powerpoint con muchos puntos con bolitas, exponga algo como lo siguiente:

*"Hemos hecho un estudio de mercado y hemos comprobado que podemos hacer las pizzas medio centímetro más pequeñas sin que los consumidores noten nada. Como nuestra empresa vende tropecientos millones de pizzas al año, el ahorro en los materias primas y costes de producción nos puede generar unos beneficios de un porrón y medio de millones al año".*

Y el ejecutivo listillo puede que tenga razón: una diferencia de medio centímetro no es nada tan grave como para que el consumidor deje de comprar la pizza. Sin embargo, al seguir este camino se abre un precedente peligroso: dentro de unos meses, otro ejecutivo listillo, celoso del primer ejecutivo listillo, propondrá utilizar un queso más barato y así ahorrar otro puñado de millones. También se pueden abaratar los precios de cada uno de los demás ingredientes, y reducir el tiempo que se tarda en hacer una pizza, simplemente amasando menos la masa; ahorrar un poco más en las condiciones laborales de los trabajadores, aunque eso haga que estén menos contentos y rindan menos y trabajen peor. Y unos meses más tarde se le puede quitar otro centímetro al tamaño de la pizza.

Son cambios pequeños que, por separado, no tendrían demasiada repercusión en la calidad de la pizza. Pero **si los juntamos todos**, al final obtenemos una verdadera porquería de pizza. **Pequeños cambios que individualmente no son importantes, al sumarse pueden crear una gran diferencia**.

Con el desarrollo de software ocurre lo mismo. Nadie quiere hacer un sistema complicado, pero invariablemente el desarrollador quiere mejorar su programa y va introduciendo pequeñas complejidades en el código. Un poquito aquí y un poquito allá. Al fin y al cabo, no son cosas tan complejas, se dice, no pueden hacer demasiado daño. **Pero sumando docenas de pequeñas complejidades se puede obtener un sistema muy complicado**. Y una vez que el sistema se ha complicado, volver atrás y simplificarlo es mucho más difícil de lo que hubiera sido hacerlo sencillo desde el principio.

La única manera de evitar que el software acabe siendo un lío monumental es siendo muy exigente con cualquier cosa que complique el código. <a href="http://gettingreal.37signals.com/ch10_Less_Software.php">¿Realmente necesita el programa esta funcionalidad?</a> Un error al que tenemos tendencia los desarrolladores es solucionar problemas que no existen. Hacer un software que podría resolver casos muy generales, que en teoría podrían presentarse, pero que en la práctica nunca se presentan. Y, sin embargo, <a href="http://blogs.oreilly.com/digitalmedia/2002/11/martin-fowler-on-flexibility-a.html">todo este código que resuelve casos imaginarios tiene un coste en complejidad</a>.

El consejo más sencillo que se puede seguir al respecto es centrarse siempre en resolver problemas reales.  Como se suele decir:
*no code is simpler than no code.*
