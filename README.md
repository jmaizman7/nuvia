# NUVIA — Landing page

Sitio estático de una sola página (`index.html`). Todas las imágenes (logo,
fotos de producto, panales y abejas) están incrustadas directamente dentro
del HTML, así que no hay carpetas de imágenes sueltas que configurar: subir
`index.html` es suficiente para que la página se vea completa.

## Opción 1: Subir el .zip directo en la web de Vercel (más fácil)

1. Entra a https://vercel.com y crea una cuenta o inicia sesión.
2. Click en **"Add New..." → "Project"**.
3. Busca la opción **"Deploy without Git"** / arrastra la carpeta del
   proyecto (descomprime el .zip primero, Vercel pide una carpeta o
   arrastras los archivos `index.html` y `vercel.json`).
4. Dale **Deploy**. En menos de un minuto tendrás un link como
   `nuvia.vercel.app`.

## Opción 2: Con la CLI de Vercel (si usas terminal)

```bash
npm i -g vercel        # instalar la CLI (una sola vez)
cd nuvia-vercel         # entra a esta carpeta descomprimida
vercel                  # sigue las instrucciones (login, nombre del proyecto)
vercel --prod           # publica la versión final
```

## Dominio propio

Una vez desplegado, en el panel de Vercel ve a **Project → Settings →
Domains** y agrega tu dominio (ej. `nuviacosmetics.com`) si ya tienes uno
comprado, o deja el que te da Vercel por defecto.

## Actualizar la página más adelante

Cuando quieras cambiar textos, precios o fotos, vuelve a pedírmelo, te paso
el `index.html` actualizado y solo reemplazas ese archivo en tu proyecto de
Vercel (o vuelves a correr `vercel --prod` si usas la CLI).
