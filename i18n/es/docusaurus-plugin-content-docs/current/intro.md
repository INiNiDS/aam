l
---
sidebar_position: 1
title: "Introducción"
---

# AAM (Abstract Alias Mapping)
## Presentando AAM
Los ficheros de configuración tienen tendencia a crecer de forma descontrolada. Se vuelven voluminosos, difíciles de leer y aún más difíciles de mantener. Dividirlos en múltiples ficheros ayuda, pero no resuelve la complejidad subyacente de gestionar relaciones de datos. Necesitábamos una forma más intuitiva de manejar los mapeos — necesitábamos AAM.
### El problema - Mapeo Verboso
Imagina que necesitas gestionar un gran conjunto de aliases bidireccionales (donde puedes buscar una clave por su valor y viceversa). En formatos como TOML, te ves obligado a escribir mucho código repetitivo:
```toml
[alias]
a = "b"
b = "a"
```
Son tres líneas para un solo mapeo. Multiplica eso por cien, y tu configuración se convierte en una pesadilla.
### La solución - AAM
AAM es una sintaxis simple y elegante que te permite definir mapeos bidireccionales en una sola línea. Con AAM, puedes escribir:
```aam
a = b
```
Esta única línea crea un mapeo bidireccional entre `a` y `b`. Puedes buscar `a` para obtener `b`, y buscar `b` para obtener `a`. Es conciso, claro y elimina el código repetitivo.
AAM está diseñado para ser conciso, legible y fácil de usar, eliminando el boilerplate para que puedas concentrarte en la lógica de tu configuración.
## Cómo nació la idea
Estaba trabajando en un proyecto que me requería gestionar un gran número de aliases. Estaba usando TOML para mis ficheros de configuración, y me di cuenta de que era muy difícil gestionar mis aliases. Tenía que escribir mucho código repetitivo para gestionarlos, y era muy fácil cometer errores. Quería una mejor forma de gestionar mis aliases, y así fue como se me ocurrió la idea de AAM.
## Empezar
¿Listo para simplificar tus configuraciones? Consulta la [Guía de inicio rápido](using/getting-started) para aprender a usar AAM en tus proyectos.
