---
layout: post
title: 100% de cobertura del código
tags:
- Programación
- sentido común
- TDD
- test
status: publish
type: post
published: true
meta:
  _edit_last: '10779279'
  jabber_published: '1285361682'
  _wpas_done_twitter: '1'
  _wp_old_slug: ''
  _wpas_skip_yup: '1'
---
Las métricas que se obtienen en un entorno de integración continua son muy útiles para detectar posibles errores en zonas del código. Sin embargo, el que tu código obtenga una buena puntuación en cualquier métrica no garantiza absolutamente nada.

Por ejemplo, la métrica más usada, por su utilidad, es el tanto por ciento de cobertura del código: el tanto por ciento de código que se ejecuta al lanzar los test. El problema con esta métrica es que se puede falsear trivialmente como demuestra el siguiente ejemplo:

```ruby
class Sumador
  def self.suma(op1, op2)
    return op1 - op2 #  Estamos restando, no sumando!
  end
end

class TestSuma < Test::Unit::TestCase
  def test_suma
    Sumador.suma 0, 2
    assert(true)
  end
end
```

Esta es una implementación rota de una clase para sumar - que, en realidad, resta- y que sin embargo tiene un 100% de cobertura de código.

Incluso cuando no hay ningún ánimo de hacer trampas, un 100% de cobertura del código no garantiza que la implementación sea correcta. Para cualquier código no trivial es imposible conseguir un 100% de cobertura de las bifurcaciones del código, o probar una función para todos los valores posibles de entrada.

Entonces, ¿qué sentido tiene esforzarnos por conseguir una alta cobertura del código? Muy sencillo: una baja cobertura indica que el código es defectuoso o, mejor dicho, está incompleto. Si tus test cubren un 0% del código -es decir, no hay tests- entonces tienes un problema. Si tienes una cobertura alta, es **muy probable** que tu código sea de alta calidad y esté poco acoplado.
