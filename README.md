# Código expresivo

## Tema principal

Como en el lenguaje natural, en el código, poder decir lo mismo de muchas maneras es valioso.
Y también, en ambos casos, tener que elegir la correcta puede ser crucial.

## Párrafo para la venta

Un problema de consumo de memoria en producción es el punto de partida de lo que casi fue una charla sobre performance.
En el camino, luego de explorar otros problemas causados por lo idiomático, se convirtió en una charla sobre el valor de la expresividad.
Vamos a ver porque vale la pena escribir código como se nos cante, o incluso de muchas maneras en paralelo.
Todo esto para cerrar con los recursos que nos permiten elegir la correcta.

## Estructura de la charla

Los `###` son columnas

Los `####` son grupos de slides. En muchos de ellos faltan detalles.

### Título y bajada

#### Presentador

Usar las tres formas de presentarse.

### Los casos problemáticos que dieron origen a la charla

#### El que le dio origen a la charla

El recordatorio de pagos con each.

Usar varias slides para esto:

- Idealmente en la que presenta el problema debería poder tener animaciones o _fragments_ que primero muestren unos pocos usuarios y luego muchos. Los usuarios pueden ser representados con iconos de usuarios. Y deberían estar _scattered_ en la pantalla.
- Incluir gráficos de como se vería el consumo de memoria.

Dije, ya está, con esto puedo hacer una charla sobre los costos de lo idiomatico. Una charla sobre performance.

#### El segundo _input_ de la charla

Mencionar el episodio de **On Rails podcast** donde, entre otras cosas, hablan de performance.

https://youtu.be/GpaSq6xW8wQ

Cuando habla de "The performance differences between size, length, and count" menciona que a veces los problemas de performance surgen porque hay muchas maneras de hacer lo mismo.

Poner el ejemplo de size? vs length? vs count?.

Mencionar que a pesar de que me entusiasmo este segundo input, me di cuenta de que si quería hablar de los costos de lo idiomatico, los _take aways_ eran los mismos:

- El cómo es tan importante como el qué. En los dos casos vemos que los _outputs_ son los mismos, pero el cómo se llega a ellos es diferente.
- El contexto es importante. En los dos casos vemos que el usar el método "incorrecto" solo tiene costo si la cantidad de datos es grande.

#### Un esfuercito más

Pensé que si encontraba algún ejemplo de algún método que detrás de su nombre esconda algo que pueda tener un impacto negativo, podría hablar de los costos de lo idiomatico.

Se me ocurrió el ejemplo de all?.

https://stackoverflow.com/a/16662982

Pero sentía que todavía no tenía su madera como para hablar de los costos de lo idiomatico.

#### Y al mirarlo un poco más de lejos

Pensando en los problemas que pueden causar lo idiomatico y lo expresivo, sin quererlo, empecé a pensar en lo valioso de la expresividad.

### Lo valioso de la expresividad - Prototipaje rápido

#### Francis Bacon

Francis Bacon dijo que primero hay que manchar el lienzo y que el cuadro empieza a emerger.
Con el código a veces es lo mismo.

Entonces, que le lenguaje de programación permita tanta expresividad hace que sea más fácil manchar el lienzo del IDE.

#### Más allá de la primera mancha

Riffing

https://www.rubyevents.org/talks/riffing-on-rails-sketch-your-way-to-better-designed-code

### Lo valioso de la expresividad - Reducción de la carga cognitiva

#### Qué es la carga cognitiva

https://github.com/zakirullin/cognitive-load

Copiar imagen de ...

Incluir definiciones de carga cognitiva intrinseca y extrinseca.

#### Hace a la eficiencia

https://martinfowler.com/articles/developer-effectiveness.html

#### Hace a la productividad

https://queue.acm.org/detail.cfm?id=3595878

#### Cómo el cerebro interpreta el código

https://news.mit.edu/2020/brain-reading-computer-code-1215

pero podemos hacer que el código se parezca más al lenguaje natural. Poner ejemplo de https://world.hey.com/dhh/a-writer-s-ruby-2050b634

### Cómo elegir la correcta

Nuestro código puede tener expresividad en detrimento de:

- Uniformidad: Mayores costos de mantenimiento.
- Confiabilidad: Bugs ocasionados por _edge cases_.
- Performance: UX degradada y mayores costos de infraestructura.

Para elegir la correcta, podemos apoyarnos en las charlas de:

- Julio sobre Refactoring en Ruby: Elevating Code Quality Through Community And Practice https://ruby.com.ar/meetup/2024_08.html
- Wacko sobre Testing: Buenas prácticas y performance https://ruby.com.ar/meetup/2024_11.html
- Patricio sobre Instrumentación y Observabilidad https://ruby.com.ar/meetup/2025_03.html

## Conclusions and Takeaways

Escriban código como se les cante.
Pero sepan que hay maneras de hacerlo que son más costosas que otras.
