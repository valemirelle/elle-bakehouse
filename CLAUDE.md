# Reglas del repositorio (Elle Bakehouse)

## 1. Siempre vista previa antes de publicar
- **Nunca** subir cambios directo a `main`. `main` es el sitio en vivo (ellebakehouse.com).
- Cada cambio va en una rama aparte (`git checkout -b nombre-del-cambio`) y se sube esa rama.
- Cloudflare genera un link de vista previa para la rama. Mandar ese link y preguntar:
  **"¿Publicamos ahora o cambiamos algo?"**
- Solo con un "sí, publica" explícito se junta la rama con `main`.

## 2. Evitar choques con Diego (merge conflicts)
- Antes de empezar cualquier cambio: `git fetch origin` y partir de la versión más reciente de `main`.
- Antes de publicar: volver a traer `main`; si Diego subió algo, integrar sus cambios primero.

## 3. Cómo hablar
- Con Mirelle: español sencillo, paso a paso, sin palabras técnicas.
- Con Diego: puede ser técnico. Si no dicen quién escribe, asumir que es Mirelle.

## 4. Commits
- Subir como `valemirelle <valemirelle@gmail.com>`.

## Dónde está cada cosa
- `src/layouts/Base.astro`: menú, colores de la marca, letras y pie de página de todas las páginas.
- `src/pages/`: una página por archivo (`index`, `menu`, `contact`).
- Los datos de prueba (mock) están marcados con ⚠️ al inicio de cada página.
