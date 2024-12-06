# Configurar Astro

- 1 Configurar el Editor

```Javascript

# Editor configuration, see https://editorconfig.org
root = true

[*]
charset = utf-8
indent_style = space
indent_size = 2
insert_final_newline = true
trim_trailing_whitespace = true

[*.ts, .js]
quote_type = single

[*.md]
max_line_length = off
trim_trailing_whitespace = false

```

- 2 Instalar

```Bash
npm create astro@latest [Nombre-del-proyecto]
```

### Opcional

- 3 Instalar Tailwind

```Bash
  npx astro add tailwind
```

- 4 Crear una carpeta styles y dentro de esta crear el archivo **base.css** con la siguiente configuración.

```Css
@tailwind base;
@tailwind components;
@tailwind utilities;
```
