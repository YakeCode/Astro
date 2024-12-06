# Crear Layout

- 1 creamos el archivo en este caso llamado Base.astro

- 2 Utilizamos una plantilla html indicándole con la palabra reservada slot donde ira el contenido interno

```HTML
<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Base Layout</title>
  </head>
  <body>
    <h1>Ladrillos Club</h1>
    <slot />
  </body>
</html>
```

- 3 Lo incorporamos en la pagina que deseamos utilizando su import de guiones con su código respectivo

```Astro
---
import Base from "../layouts/Base.astro";
---

<Base>
  <h2>Acerca de piezas lego</h2>
  <p>
    Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ducimus dolores
    maxime tempora iusto sit tenetur architecto facilis numquam nostrum minus
    molestiae, neque debitis, assumenda vero earum, quae eaque necessitatibus
    officia.
  </p>
</Base>

```
