# GRZ

Un sitio de una sola página con una colección de textos escritos para GRZ.

👉 **Ver el sitio:** https://lucasvicente-com-ar.github.io/grz/

## Qué contiene

- Seis textos (poemas y prosa poética), cada uno con su fecha original de escritura.
- Un espacio reservado para una imagen por texto — se van agregando a medida que están listas.
- Mismo diseño editorial oscuro usado en [el-amenazado](https://github.com/lucasvicente-com-ar/el-amenazado) (tipografía Cormorant Garamond + Cinzel, acentos dorados, animaciones de aparición al hacer scroll). Totalmente responsive.

## Estructura

```
.
├── index.html      # el sitio completo: HTML + CSS + JS inline, sin build ni dependencias
├── escritos.txt    # textos en bruto, fuente original
└── README.md
```

## Agregar una imagen a un texto

En `index.html`, cada poema tiene un bloque:

```html
<div class="img-slot" aria-hidden="true">Imagen próximamente</div>
```

Reemplazarlo por:

```html
<img class="poem-image" src="nombre-de-la-imagen.png" alt="descripción breve">
```

y subir el archivo de imagen a la raíz del repositorio.

## Publicación

El sitio se sirve con **GitHub Pages** desde la rama `main`, raíz del repositorio (`/`). Cualquier `git push` a `main` se refleja automáticamente en unos minutos en:

https://lucasvicente-com-ar.github.io/grz/
