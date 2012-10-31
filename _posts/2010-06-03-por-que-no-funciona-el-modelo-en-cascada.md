---
layout: post
title: Por qué no funciona el modelo en cascada
tags:
- agilidad
- desarrollo
- ingeniería del software
- metodologías ágiles
- planificación
- Programación
status: publish
type: post
published: true
meta:
  _edit_last: '10779279'
  jabber_published: '1275523489'
  delicious: a:3:{s:5:"count";s:1:"0";s:9:"post_tags";s:0:"";s:4:"time";s:10:"1284365513";}
  _wp_old_slug: ''
  reddit: a:2:{s:5:"count";s:1:"0";s:4:"time";s:10:"1284365515";}
  _wpas_done_twitter: '1'
  _wpas_skip_yup: '1'
---
<a href="http://www.flickr.com/photos/tonymangan/611780383/" title="Lumsdale Waterfall 1 by ~~Tone~~, on Flickr"><img src="http://farm2.static.flickr.com/1133/611780383_6e7c8d2bc8.jpg" width="363" height="500" alt="Lumsdale Waterfall 1" /></a>

La ingeniería del software es una recién nacida: la humanidad lleva miles de años construyendo edificios, barcos y puentes, pero sólo unas décadas construyendo software.

Cuando nació la ingeniería del software se fijó en sus hermanas para descubrir como se hace *eso* de construir sistemas complejos. Y, básicamente, la ingeniería del software copió los métodos tradicionales en lo que se conoce como *Modelo en Cascada*.

En el Modelo en Cascada, los ingenieros hacen  primero un análisis de los requisitos del proyecto: Si se va a construir un puente, hay que saber qué capacidad de tráfico tiene que atravesar el puente, los vientos, mareas y temblores que debe soportar, etc. Con todos estos requisitos se hace un documento funcional explicando cómo debe funcionar el puente cuando esté acabado. Al documento funcional le sigue un diseño técnico: en una obra serían los planos que modelarían el puente, las instrucciones para construir el puente. Una vez se tiene un plan, hay que construir el puente. Cuando el puente está construido, pasamos a la fase de mantenimiento. Este es, muy resumido, el modelo en cascada.

Este sistema funciona razonablemente bien en las ingenierías tradicionales, pero fracasa estrepitosamente en la ingeniería del software. ¿Por qué? Porque **los requisitos y el proceso de construcción del software son de naturaleza completamente distinta al los de la construcción de un puente**.

Cuando se construye un puente, todos los requisitos y las funciones que debe cumplir **deben estar especificados de antemano**. Hay que hacer un plano que detalle al milímetro cómo va a ser el puente y seguirlo al pie de la letra. Una vez se empieza a construir un puente, no podemos cambiar de opinión a la mitad y decir, "*no nos habíamos dado cuenta, pero necesitamos que los barcos puedan navegar por debajo del puente. Cámbiame el puente que estas haciendo por un puente levadizo*". Por desgracia, una vez hemos puesto los cimientos, el diseño no se puede alterar demasiado.

En cambio, **en el desarrollo de software los requisitos cambian constantemente**. Y eso no es algo malo, sino que es una ventaja que deben aprovechar los buenos desarrolladores.

En vez de planificar todo de antemano, y seguir el plan al pie de la letra, es bueno permitir cierta flexibilidad para que el proyecto vaya creciendo orgánicamente y se vaya definiendo con el tiempo. Puede que el cliente se dé cuenta de que lo que ha pedido no es exactamente lo que necesita, sino que, en realidad, quiere un producto ligeramente diferente. O muy diferente. Eso está bien: **nos hemos dado cuenta y podemos corregirlo antes de que el cliente se quede con un producto que no resuelve sus problemas. Cambiar el diseño a mitad de proyecto hace que el producto final sea más eficiente y, sobre todo, satisfaga mejor las necesidades del cliente**.

Muchos proyectos tremendamente exitosos empezaron siendo siendo una cosa y terminaron siendo otra completamente distinta, pero fue **precisamente este cambio el que les permitió triunfar**. Flickr, por ejemplo, empezó como un juego online, pero los desarrolladores se dieron cuenta de que una inocente funcionalidad que permitía a los jugadores compartir fotos se estaba convirtiendo en la estrella de su servicio. Fueron inteligentes y cambiaron sus requisitos iniciales; acabaron convirtiendo un juego medianamente exitoso, en un servicio para compartir fotos *tremendamente* exitoso.

Flickr no es un caso único. Blogger nació como un servicio de gestión de proyectos; en sus comienzos, Paypal era una plataforma para hacer micropagos con las Palm Pilot... Puede decirse que la mayoría de los proyectos exitosos no lo son por sus ideas originales, sino por la **facilidad que tienen de adaptarse a los cambios y a las nuevas oportunidades**.

Pero -estaréis pensando- ¡cambiar los requisitos a mitad de un proyecto tiene un coste muy grande! Eso no se puede hacer. ¿No?

Sí y no. Cambiar los requisitos tiene un coste muy grande cuando se sigue el modelo en cascada, en el que toda **la planificación se hace de antemano, y cada fase depende muchísimo de que la anterior se haya hecho bien**. En esas circunstancias, cambiar la planificación significa echar por tierra mucho esfuerzo y trabajo.

Pero el modelo en cascada no es la única manera de hacer software.

<a href="http://www.flickr.com/photos/44799719@N00/324947287/" title="Jägala waterfall  part III by fireramsey, on Flickr"><img src="http://farm1.static.flickr.com/144/324947287_feb20f51ea.jpg" width="500" height="375" alt="Jägala waterfall  part III" /></a>
*(Las cascadas son bonitas, pero no para hacer software)*

En los últimos diez años han surgido una variedad de **metodologías ágiles** que apuestan por desarrollar software de forma **iterativa**: se van añadiendo funcionalidades en iteraciones pequeñas, de unas pocas semanas. Tras cada iteración se evalúan los requisitos para ver si siguen siendo las necesidades **reales** del cliente, y en consecuencia se planea la próxima iteración. Es natural posponer los problemas hasta que tengamos más datos, y si necesitamos cambiar la planificación, tampoco perdemos tanto trabajo porque, en realidad, tampoco hemos invertido tanto esfuerzo planificando.

En el desarrollo ágil los cambios de requisitos no se ven como un inconveniente, sino como una ventaja potencial. Como dice <a href="http://agilemanifesto.org/">el Manifiesto Ágil</a>:

<blockquote>Valoramos más la respuesta ante el cambio que el seguir un plan.
...
Aceptamos que los requisitos cambien, incluso en etapas tardías del desarrollo. Los procesos Ágiles aprovechan el cambio para proporcionar ventaja competitiva al cliente.</blockquote>
