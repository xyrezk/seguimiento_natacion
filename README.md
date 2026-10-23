# Nado

Registro personal de natación: día, metros, largos y tiempo. Es una PWA (app web instalable). Funciona sin internet y guarda los datos solo en tu celular.

## Publicar en GitHub Pages

1. Crea un repositorio en GitHub, por ejemplo `nado`. Puede ser público; tus datos no se suben, solo la app.
2. Sube estos archivos a la raíz del repo:
   ```
   index.html
   manifest.webmanifest
   sw.js
   icons/
   ```
   Puedes hacerlo con git:
   ```bash
   git init
   git add .
   git commit -m "Nado v1"
   git branch -M main
   git remote add origin https://github.com/TU_USUARIO/nado.git
   git push -u origin main
   ```
3. En el repo ve a **Settings → Pages**. En *Source* elige **Deploy from a branch**, rama `main`, carpeta `/ (root)` y guarda.
4. En uno o dos minutos queda en `https://TU_USUARIO.github.io/nado/`.

## Instalar en el celular (Android)

1. Abre el link en **Chrome**.
2. Abre el menú ⋮ y toca **Instalar app** (o *Agregar a pantalla de inicio*).
3. Queda con su ícono, abre a pantalla completa y funciona sin conexión.

## Datos

- Se guardan en el almacenamiento del navegador del celular. No salen de ahí.
- Si desinstalas la app o borras los datos de Chrome, **se pierden**. Usa **Respaldo** de vez en cuando: descarga un `.json`. Con **Restaurar** lo recuperas en cualquier celular.
- **Exportar CSV** sirve para abrir tus sesiones en Excel o Google Sheets.

## Actualizar la app

Si cambias el código, sube el cambio y en `sw.js` sube la versión (`nado-v1` → `nado-v2`). El celular toma la nueva versión la siguiente vez que abras la app (a veces hace falta abrirla dos veces).
