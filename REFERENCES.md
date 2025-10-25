# Referencias y Recursos

Este documento contiene todas las fuentes, estudios y referencias utilizadas para la charla "Código idiomático".

## Feedback Loops y Productividad

### Estudios Académicos y de Industria (2024-2025)

- **Cognitive Load and Developer Productivity (2025)**
  - Estudio sobre patrones de carga cognitiva y diferenciales de productividad entre metodologías Agile y Waterfall
  - Resultados: Agile reduce carga cognitiva durante fases de feedback iterativo, pero la aumenta en planning
  - [ResearchGate Paper](https://www.researchgate.net/publication/395303599)

- **Developer Effectiveness & Feedback Loops**
  - Martin Fowler: "Maximizing Developer Effectiveness"
  - [https://martinfowler.com/articles/developer-effectiveness.html](https://martinfowler.com/articles/developer-effectiveness.html)

- **DevEx: What Actually Drives Productivity (ACM Queue)**
  - Investigación sobre factores que impulsan la productividad de desarrolladores
  - Feedback loops, cognitive load, y flow state como factores clave
  - [https://queue.acm.org/detail.cfm?id=3595878](https://queue.acm.org/detail.cfm?id=3595878)

### Estadísticas Clave

- Los desarrolladores ejecutan ~200 micro-feedback loops por día
- 76% de organizaciones admiten que la carga cognitiva de su arquitectura crea estrés y reduce productividad
- 69% de desarrolladores pierden 8+ horas semanales por ineficiencias (technical debt, documentación insuficiente, procesos de build complejos)
- Estudio DORA 2024: 25% de aumento en uso de IA generativa redujo throughput en 8%

### Casos de Estudio

- **eBay's Velocity Initiative**
  - Enfocada en mejorar feedback loops y reducir cognitive load
  - [https://www.infoq.com/articles/developer-effectiveness-feedback/](https://www.infoq.com/articles/developer-effectiveness-feedback/)

- **Spotify's Infrastructure Research**
  - Infraestructura construida como "islas aisladas" generó context switching y cognitive load
  - Impacto negativo en productividad de ingenieros

## Código Idiomático y Expresividad en Ruby

### Filosofía de Ruby

- **Yukihiro "Matz" Matsumoto**
  - "Ruby is designed to make programmers happy"
  - Lenguaje diseñado conscientemente para ser intuitivo y leer casi como inglés
  - Prioriza expresividad y legibilidad sobre performance raw

### Recursos sobre Idiomatic Ruby

- **Idiomatic Ruby: Writing Beautiful Code**
  - [https://www.bomberbot.com/ruby/idiomatic-ruby-writing-beautiful-code/](https://www.bomberbot.com/ruby/idiomatic-ruby-writing-beautiful-code/)

- **Towards Minimal, Idiomatic, and Performant Ruby Code**
  - Desmitificando idiomas populares de Ruby
  - [https://blog.codeminer42.com/towards-minimal-idiomatic-and-performant-ruby-code-f3fc6aed3c94/](https://blog.codeminer42.com/towards-minimal-idiomatic-and-performant-ruby-code-f3fc6aed3c94/)

- **Expressive Ruby and Rails (AppSignal)**
  - Comunicación efectiva con tu código
  - [https://blog.appsignal.com/2023/10/11/expressive-ruby-and-rails-communicate-effectively-with-your-code.html](https://blog.appsignal.com/2023/10/11/expressive-ruby-and-rails-communicate-effectively-with-your-code.html)

### Principios Clave

- Código se lee más frecuentemente de lo que se escribe → optimizar para comprensión humana
- Código expresivo comunica no solo QUÉ hace, sino POR QUÉ se escribió de esa manera
- Reduce necesidad de comentarios extensivos
- Características idiomáticas: bloques, métodos predicate (`?`), cadenas de métodos naturales

## Divergent & Convergent Thinking

### Teoría y Aplicación

- **The Synergy of Diverge and Converge in Design Thinking**
  - [https://voltagecontrol.com/articles/the-synergy-of-diverge-and-converge-in-design-thinking/](https://voltagecontrol.com/articles/the-synergy-of-diverge-and-converge-in-design-thinking/)

- **Divergent vs Convergent Thinking en Software Design (InformIT)**
  - Sin divergent thinking, los equipos no pueden alcanzar el payoff del convergent thinking
  - Muchas empresas evitan divergent thinking, para su detrimento
  - [https://www.informit.com/articles/article.aspx?p=459616](https://www.informit.com/articles/article.aspx?p=459616)

### Research Sobre Herramientas

- **How Digital Tools Impact Convergent and Divergent Thinking (CHI 2021)**
  - Herramientas digitales generan más convergent thinking comparado con herramientas analógicas
  - Sin impacto discernible en productividad general o divergent thinking
  - [https://dl.acm.org/doi/10.1145/3411764.3445062](https://dl.acm.org/doi/10.1145/3411764.3445062)

### Técnicas

- Sketching como herramienta de divergencia:
  - Los sketches comunican "disposabilidad" → permite cambiar/descartar ideas sin preocupación
  - Ayuda a pensar visualmente
  - Templates: 6-UP to 1-UP para explorar soluciones rápidamente

## Riffing (Kasper Timm Hansen)

### Recursos Oficiales

- **Kasper Timm Hansen**
  - Ex Rails Core Team (6 años, ~1750 commits a Rails)
  - [https://kaspth.com/](https://kaspth.com/)

- **RailsConf 2024: Riffing on Rails**
  - "Sketch your way to better designed code"
  - [Speaker Deck](https://speakerdeck.com/kaspth/railsconf-2024-riffing-on-rails-sketch-your-way-to-better-designed-code)
  - [Ruby Events](https://www.rubyevents.org/talks/riffing-on-rails-sketch-your-way-to-better-designed-code)

- **The Bike Shed Podcast: Episode 433**
  - Discusión sobre Riffing con Kasper
  - [https://bikeshed.thoughtbot.com/433](https://bikeshed.thoughtbot.com/433)

### Qué es Riffing

- Escribir código "casi-ejecutable" en un scratch file
- Usar plain-old Rails/Ruby classes & methods
- Low-fidelity sketching para enfocarse en high-level design
- **"Wireframing para código"**

### Beneficios

- Iterar más rápido y ahorrar tiempo
- Detectar y escalar blockers temprano → deriesgar el trabajo
- Excelente para construir entendimiento compartido (pairing)
- Crea flow state durante el diseño
- Explorar nombres, responsabilidades, y relaciones entre objetos

### Recursos Adicionales

- **Curso: Domain Modeling in Rails**
  - [Gumroad](https://kaspthrb.gumroad.com/l/domain-model-riffing)
- **GitHub Repository**
  - [github.com/kaspth/riffing-on-rails](https://github.com/kaspth/riffing-on-rails)

## Ruby Performance y Memory Bloat

### Enumerable Performance

- **each vs find_each Benchmarks**
  - `each`: más rápido (260ms vs 480ms) pero carga todo en memoria
  - `find_each`: procesa en batches de 1000, permite garbage collection
  - [Mufid's Blog](https://mufid.github.io/blog/2016/rails-batch-performance/)

- **5 Ruby Performance Pitfalls**
  - [MoldStud](https://moldstud.com/articles/p-5-common-ruby-performance-pitfalls-and-how-to-avoid-them)

### ActiveRecord Memory Usage

- **Optimizing Rails for Memory Usage (Part 3)**
  - Pluck y Database Laziness
  - [Collective Idea](https://collectiveidea.com/blog/archives/2015/03/05/optimizing-rails-for-memory-usage-part-3-pluck-and-database-laziness/)

- **Memory Bloat in Ruby on Rails**
  - Troubleshooting performance degradation y RAM usage
  - [Mindful Chase](https://www.mindfulchase.com/explore/troubleshooting-tips/troubleshooting-memory-bloat-in-ruby-on-rails-fixing-performance-degradation-and-excessive-ram-usage.html)

### Técnicas de Optimización

- Usar `.lazy` para evitar generar arrays enormes
- Lazy enumerators (Ruby 2.0+) mejoran significativamente uso de memoria
- ActiveRecord objects son memory hogs: 30 está bien, 3000 consumirá mucha memoria
- `find_each` carga en batches de 1000, permitiendo GC entre batches

## Enumerable#all? y Vacuous Truth

### Documentación y Discusiones

- **Ruby Issue Tracker: Feature #8723**
  - "Array.any? predicate returns true for empty array"
  - [bugs.ruby-lang.org/issues/8723](https://bugs.ruby-lang.org/issues/8723)

- **Stack Overflow: Why does .all? return true on empty array?**
  - [stackoverflow.com/questions/16662727](https://stackoverflow.com/questions/16662727/why-does-all-return-true-on-an-empty-array)

- **Ruby Issue: Feature #12110**
  - "Create a method to avoid vacuous truth?"
  - [bugs.ruby-lang.org/issues/12110](https://bugs.ruby-lang.org/issues/12110)

### Explicación Matemática

- **Vacuous Truth (Verdad Vacua)**
  - Interpretación estándar de cuantificación universal sobre conjunto vacío
  - Elemento neutro de AND lógico (∧) es `true`
  - Paralelismos:
    - Suma de cero elementos = 0 (elemento neutro de +)
    - Producto de cero elementos = 1 (elemento neutro de ×)
    - Logical AND de cero elementos = true (elemento neutro de ∧)

### Map-Reduce Perspective

```ruby
[].all? { |x| predicate(x) }
# equivalente a:
[].inject(true) { |memo, x| memo && predicate(x) }
```

### Lenguaje Natural vs Lógica Formal

- En lenguaje natural: cuantificación universal presupone dominio no-vacío
- En sistemas formales: difiere, haciendo el comportamiento contra-intuitivo inicialmente
- Principio de neutral elements justifica el comportamiento

## Herramientas de Convergencia

### APMs (Application Performance Monitoring)

- New Relic
- Scout APM
- Skylight
- AppSignal

### Linters y Análisis Estático

- RuboCop
- Reek
- Brakeman (seguridad)
- Rails Best Practices

### Testing Frameworks

- RSpec
- Minitest
- Capybara (integration testing)
- rspec-benchmark (performance testing)

## Recursos Adicionales de Reveal.js

- **Documentación oficial**: [https://revealjs.com/](https://revealjs.com/)
- **Fragments (animaciones)**: [https://revealjs.com/fragments/](https://revealjs.com/fragments/)
- **Speaker Notes**: [https://revealjs.com/speaker-view/](https://revealjs.com/speaker-view/)
- **Vertical Slides**: [https://revealjs.com/vertical-slides/](https://revealjs.com/vertical-slides/)

## Cómo usar esta presentación

1. Instalar dependencias:
   ```bash
   npm install
   ```

2. Iniciar servidor de desarrollo:
   ```bash
   npm start
   ```

3. Ver speaker notes durante la presentación:
   - Presionar `S` durante la presentación
   - Se abrirá una ventana con las notas

4. Navegación:
   - Flechas izquierda/derecha: cambiar de columna (sección principal)
   - Flechas arriba/abajo: navegar slides dentro de una columna
   - ESC: vista general de todas las slides
   - `S`: speaker view con notas

## Licencia

Esta charla está bajo licencia MIT. Siéntete libre de usarla, adaptarla y compartirla.
