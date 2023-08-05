# Summary Fisica 1Q

Este es sitio fue elaborado a partir de las notas tomadas en el curso de Física 1Q del departamento de Física de la Facultad de Ciencias Exactas y Naturales de la Universidad de Buenos Aires durante el primer cuatrimestre del año 2023.

El material de lectura de este espacio no pretende reemplazar a las fuentes principales que inspiraron su construcción y que se encuentran anexadas en cada uno de los artículos. Se ínsita al lector a complementar estos resúmenes con la bibliografía recomendada en el sitio principal de la materia, guías de ejercicios y apuntes personales.

Vale la pena aclarar que esta página no tiene relación alguna con la Universidad de Buenos Aires. No se trata de un sitio oficial y queda bajo criterio del lector adoptar o no, las definiciones o conceptos aquí mencionados.

## 🚀 Estructura del proyecto

Dentro del repositorio vas a poder ver los siguientes archivos y carpetas

```
├── public/
├── src/
│   ├── components/
│   ├── content/
│   ├── layouts/
│   └── pages/
├── astro.config.mjs
├── README.md
├── package.json
└── tsconfig.json
```

Este proyecto fue construido basado en [Astro](https://astro.build/) por lo que archivos con extensión `.astro` y `.md` que se encuentren dentro de la carpeta `src/pages/` serán expuestos como rutas basadas en el nombre del archivo.

En la carpeta `src/components` se encuentran los componentes generales para la construcción del sitio, nada especial. 

En la carpeta `src/content/blog` se encuentran los archivos `.md` de cada uno de los artículos que se muestran en el sitio. Notar que en la carpeta `public` existe una carpeta por cada archivo `.md` que contiene una serie de imágenes que claramente están relacionados con el articulo en cuestión. Esto es así por cuestiones técnicas y de organización.

## 🧞 Comandos

Todos los comandos deben ejecutarse desde la carpeta raíz del proyecto

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:3000`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 😀 Características:

- ✅ Si bien se pueden implementar estilos propios para cada articulo, el proyecto ya cuenta con `tailwind.css` . Aprovecharlo
- ✅ 100/100 Lighthouse performance
- ✅ SEO-friendly with canonical URLs and OpenGraph data
- ✅ Soporte para Sitemap
- ✅ Soporte para RSS Feed
- ✅ Soporte para Markdown & MDX.
- ✅ Soporte para expresiones matemáticas escritas en Latex

## 👀 Lista de tareas para publicar un nuevo articulo

- Colocar el articulo con extensión `.md` en la carpeta `src/content/blog`. 
- Crear o colocar la carpeta de imágenes relacionadas con el articulo en la carpeta `public/` . Tanto la carpeta como el documento `.md` deben tener el mismo nombre.
- Las imágenes que se muestren en cada articulo, deben tener como `path` el siguiente formato: `/fisica1q/<NombreDelArticulo>/<NombreDeLaImagen>`.
- Cada articulo debe tener un encabezado en donde figuren los siguientes datos
  - `title` : Titulo del articulo.
  - `description`: Descripción del articulo.
  - `pubDate`: Fecha de publicación.
  - `heroImage`: Dirección de una imagen representativa del articulo en cuestión.
  - `notes`: Dirección de la fuente del articulo. En general, son las notas de clase.
  - `vclass`: Dirección a la clase virtual. En general, son las clases subidas por la catedra. 
