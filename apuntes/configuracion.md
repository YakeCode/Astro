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

- 5 Complemento de tailwind

  Es un plugin oficial de Tailwind CSS diseñado para proporcionar estilos predefinidos y altamente configurables para contenido HTML enriquecido, como artículos, blogs, documentación, y más.

```Bash
npm install -D @tailwindcss/typography
```

- Importarlo en ka configuración de tailwind

```Javascript
/** @type {import('tailwindcss').Config} */
export default {
	content: ['./src/**/*.{astro,html,js,jsx,md,mdx,svelte,ts,tsx,vue}'],
	theme: {
		extend: {},
	},
	plugins: [require('@tailwindcss/typography')],
}
```

- Incluir la palabra reservada **prose** donde se renderiza

### Instalar react

```Bash
npx astro add react
```
