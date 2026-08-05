# ConectaECU — Landing

Landing page estática de ConectaECU. Un solo archivo HTML, sin dependencias ni build. Lista para GitHub Pages y para migrar después a cualquier hosting.

## Estructura

```
conectaecu-web/
├── index.html          # La landing completa (HTML + CSS embebido)
├── BRAND.md            # Manual de marca
├── assets/
│   ├── logo.svg        # Logotipo (símbolo + wordmark)
│   └── favicon.svg     # Favicon
├── .nojekyll           # Evita que GitHub Pages ignore los assets
└── README.md
```

## Ver en local

No necesita servidor. Abre `index.html` en el navegador. Si prefieres un servidor local:

```bash
python3 -m http.server 8000
# abre http://localhost:8000
```

## Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub (ej. `conectaecu-web`).
2. Sube estos archivos:
   ```bash
   git init
   git add .
   git commit -m "Landing inicial ConectaECU"
   git branch -M main
   git remote add origin https://github.com/TU_USUARIO/conectaecu-web.git
   git push -u origin main
   ```
3. En GitHub: **Settings → Pages → Source → Branch: `main` / root** y guarda.
4. En un par de minutos estará en `https://TU_USUARIO.github.io/conectaecu-web/`.

## Migrar a tu dominio o a otro hosting

Al ser estático funciona en cualquier lado sin cambios:

- **Vercel / Netlify:** arrastra la carpeta o conecta el repo. Detecta el sitio estático automáticamente.
- **Dominio propio (`conectaecu.site`):** en GitHub Pages usa **Settings → Pages → Custom domain**, o sube los archivos a tu VPS Nginx en la raíz que sirvas.

## Editar

- **Textos y secciones:** todo está en `index.html`, en español y bien comentado por secciones (`HERO`, `CÓMO FUNCIONA`, `BENEFICIOS`, etc.).
- **Colores y tipografía:** en el bloque `:root` al inicio del `<style>`. Cambiar un color ahí lo actualiza en todo el sitio.
- **Botón principal:** apunta a `https://www.conectaecu.site`. Búscalo con Ctrl+F para cambiar el destino.

Ver `BRAND.md` para las reglas de marca (paleta, tipografía, voz, uso del logo).
