# Dermis · Landing de waitlist e ideas

Página de una sola pantalla con waitlist, formulario de ideas y llamado a dermatología.
Los datos se guardan en un Google Sheet tuyo.

## 1. Conectar el Google Sheet (5 min)

1. Crea un Google Sheet nuevo, por ejemplo "Dermis – Waitlist".
2. Menú **Extensiones → Apps Script**. Borra lo que haya y pega el contenido de `apps-script.gs`. Guarda.
3. **Implementar → Nueva implementación** → engranaje → **Aplicación web**.
   - Ejecutar como: **Yo**
   - Quién tiene acceso: **Cualquier usuario**
4. Autoriza los permisos que pide Google (es tu propio script).
5. Copia la **URL de la aplicación web** (termina en `/exec`).
6. En `index.html`, busca `const ENDPOINT = "";` y pega la URL entre las comillas.

Las pestañas **Waitlist** e **Ideas** se crean solas con el primer envío.
La waitlist ignora correos repetidos.

## 2. Publicar en GitHub Pages (5 min)

1. En GitHub: **New repository** → nombre `dermis` → Public → Create.
2. **Add file → Upload files** → arrastra `index.html` → Commit.
3. **Settings → Pages** → Source: *Deploy from a branch* → Branch: `main` / `(root)` → Save.
4. En 1–2 minutos tu página estará en `https://TU-USUARIO.github.io/dermis/`.

Para cambiar algo después, edita `index.html` en GitHub y haz commit; se actualiza solo.

## Notas

- Si cambias el código de `apps-script.gs`, vuelve a **Implementar → Gestionar implementaciones → Editar → Nueva versión** para que se aplique.
- Los correos son datos personales: compártelos solo con el equipo y bórralos si alguien lo pide.
