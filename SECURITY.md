# Política de seguridad

## Alcance

Esta política cubre las páginas estáticas, el código JavaScript incluido y los archivos publicados por este repositorio. El sitio no debe recibir credenciales, datos personales ni secretos en el navegador o en el repositorio.

## Reportar una vulnerabilidad

No publiques credenciales, tokens, datos personales ni detalles de explotación en un issue público. Cuando esté disponible, utiliza **Report a vulnerability** en la pestaña **Security** de GitHub para enviar el aviso privado al mantenedor. Si esa opción no está disponible, solicita un canal privado desde el perfil del mantenedor antes de compartir los detalles.

Incluye el archivo o URL afectado, el commit o versión, pasos mínimos de reproducción, impacto y una mitigación sugerida. Redacta cualquier registro o dato personal. No subas claves, archivos `.env`, contraseñas o tokens como parte de una corrección.

## Límites conocidos

El sitio es contenido estático y carga fuentes desde Google Fonts. La CSP declarada permite scripts y estilos inline porque la página actual los contiene; cualquier cambio futuro debe conservar `frame-ancestors 'none'`, `object-src 'none'` y la política Referrer salvo una justificación revisada.
