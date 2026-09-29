# Publicación online

Este proyecto deja preparada la interfaz pública y el panel de administración.

Para hacerlo realmente multiusuario hay que:
1. Crear un proyecto en Supabase.
2. Ejecutar `supabase_schema.sql` en el SQL Editor.
3. Crear las variables `SUPABASE_URL` y `SUPABASE_SERVICE_ROLE_KEY` en el hosting.
4. Implementar/proteger las rutas `/api/leaderboard` y `/api/admin/*`.
5. Publicar la carpeta en Vercel/otro hosting.

IMPORTANTE: nunca pongas `SUPABASE_SERVICE_ROLE_KEY` en el navegador. Debe vivir solamente en las funciones servidor.

La interfaz ya está separada:
- `/` = clasificación pública.
- `/admin.html` = panel de administrador.

La versión entregada es una base lista para conectar al backend; no incluye credenciales ni una base de datos real.
