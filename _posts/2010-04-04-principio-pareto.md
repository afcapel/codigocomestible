---
layout: post
title: El principio de Pareto
tags:
- desarrollo
- ingeniería del software
- planificación
- Programación
status: publish
type: post
published: true
meta:
  _edit_last: '10779279'
  _wpas_done_twitter: '1'
  delicious: a:3:{s:5:"count";s:1:"2";s:9:"post_tags";s:0:"";s:4:"time";s:10:"1283620664";}
  _wpas_skip_yup: '1'
  reddit: a:2:{s:5:"count";s:1:"0";s:4:"time";s:10:"1279795869";}
---
El Principio de Pareto dice **que el 80% de los resultados se producen por el 20% de las causas**. Fue formulado en 1906 por el economista italiano Wilfredo Pareto, quién observó que el 80% de la tierra en Italia era propiedad del 20% de la población. En el mundo de los negocios a menudo sirve como regla heurística, es decir, para calcular a ojo de buen cubero, por ejemplo, que el 80% de los beneficios suele venir del 20% de los clientes.

Es un principio general que puede servir como aproximación en muchos campos y que es muy importante en ingeniería del software, dónde suele ocurrir que **el 80% de la funcionalidad del software se puede desarrollar con un 20% del esfuerzo**.

Parece una afirmación peregrina, y evidentemente los porcentajes no son exactos, sino que sólo pretenden ser una mera aproximación. Sin embargo, al evaluar cualquier proyecto que conozcas o en el que hayas trabajado, imagina cual sería el coste y el beneficio de hacer sólo las partes más sencillas de la aplicación: obviar los casos complicados, no hacer un sistema de control de errores sofisticado, no validar las entradas de los usuarios y no preocuparse por si una de cada 10 veces la aplicación puede fallar. Así, ciertamente, se puede hacer una aplicación que parece funcionar, digamos un 80% del tiempo, y con un esfuerzo mucho inferior al que costaría desarrollar una aplicación completa.

Otras aplicaciones interesantes del Principio de Pareto a la ingeniería del software podrían ser:

<ul>
<li>Testar el 20% del código sirve para eliminar el 80% de los bugs.</li>
<li>El 80% del tiempo una aplicación sólo ejecuta un 20% del código y utiliza un 20% del conjunto de datos.</li>
<li>Por eso mismo, optimizar el 20% del código o cachear el 20% de los datos puede dar lugar a un 80% de mejora del rendimiento.</li>
</ul>

Este principio también explica por qué las aplicaciones que parecen casi terminadas suelen demorarse al final del proyecto, cuando sólo falta por resolver la infinidad de cabos sueltos que siempre se dejan para el final: **lo que más cuesta en una aplicación no es construir el esqueleto, sino pulir los detalles**.

Pero el principio de Pareto sirve especialmente para minimizar el riesgo que se corre al desarrollar una aplicación y se utiliza sobre todo en las metodologías ágiles de desarrollo de software. Según esta escuela de la ingeniería del software, **es muy importante que los desarrolladores tengan cuanto antes feedback de cómo funciona el producto que están desarrollando y si satisface, o no, las necesidades del cliente**.

Si desarrollamos primero las partes más complicadas de un producto, sin tener nada que enseñar hasta que todas las piezas estén completas, y esperamos hasta el último momento para desplegarlo y enseñárselo al cliente, nos podemos encontrar con la situación, tan común como desagradable, de que el producto cumple los requisitos funcionales que pidió el cliente, pero no es exactamente lo que el cliente necesita. No obstante, esto no lo saben ni el cliente ni los desarrolladores hasta que ven el software funcionando e intentan probarlo. El cliente acaba insatisfecho con el software que ha comprado y el desarrollador se siente frustrado porque ha trabajo duro para cumplir todos los requisitos funcionales pero el cliente no parece apreciar el software que tanto trabajo le ha costado construir.

En cambio, si desarrollamos primero las partes más útiles del sistema, **con un 20% del esfuerzo ya se puede ver si el diseño está bien hecho y si la aplicación es realmente lo que el cliente necesita.** Si hay que hacer cambios en el diseño o en los requisitos, cuanto antes se definan esos cambios más útiles serán y menos costará implementarlos.

El principio de Pareto no es una ley matemática exacta y no puede utilizarse como dogma, sino más bien como una regla del sentido común, pero aplicado con moderación puede servir para planificar correctamente un proyecto y evitar el riesgo de malgastar recursos en esfuerzos inútiles.

Como escriben Kent Beck y Martin Fowler en *<a href="http://www.amazon.com/Planning-Extreme-Programming-Kent-Beck/dp/0201710919">Planning Extreme Programming</a>*:

<blockquote>Los programadores de software están acostumbrados a tratar con la regla del 20-80 -el 80% de los beneficios provienen del 20% del trabajo. La programación XP hace uso de está regla -pon el 20% más valioso de la funcionalidad en producción, haz el 20% más valioso del diseño, confía en la regla del 20-80 para postergar la optimización. </blockquote>


