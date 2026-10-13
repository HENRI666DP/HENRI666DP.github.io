GUÍA DE INSTALACIÓN — HENRI IA REAL (CLOUDFLARE GRATIS)

1. Regístrate o inicia sesión en https://dash.cloudflare.com/ y mantén el plan Workers Free.
2. Ve a Workers & Pages > Create > Worker y crea el Worker "henri-guia-ia".
3. Edita su código y reemplázalo por el contenido de worker.js. Pulsa Deploy.
4. En Settings > Bindings > Add binding, selecciona Workers AI y pon el nombre EXACTO AI. Guarda y despliega de nuevo.
5. Copia la URL pública de tu Worker, que tendrá forma https://henri-guia-ia.TU-SUBDOMINIO.workers.dev/ .
6. Abre index.html y reemplaza https://REEMPLAZAR-CON-TU-WORKER.workers.dev/ por la URL real. NO agregues claves ni tokens al HTML.
7. Sube los archivos actualizados de la página a tu repositorio GitHub Pages. Prueba desde https://henri666dp.github.io/ .

ATENCIÓN: el asistente solo está conectado a IA real después de configurar y publicar el Worker. En vista previa local responde con el motor anterior. El Worker acepta peticiones desde el dominio público de tu página, no desde file://. No es una protección contra uso automatizado: para alto tráfico añade Turnstile, controles de cuota/rate limiting y supervisión de consumo.

Cloudflare Workers AI tiene una asignación gratuita diaria con límites; si se agota, el asistente utiliza las respuestas locales de respaldo. Revisa los límites y los términos actuales en https://developers.cloudflare.com/workers-ai/platform/pricing/ .

REVISION: El frontend envia historial; el Worker de este ZIP admite historial y history.
El Worker publicado en Cloudflare no se modifica al subir el sitio a GitHub Pages.

ACTUALIZACION 2026-10-13: El Worker ahora permite hasta 1400 tokens de salida y 2400 caracteres por mensaje de historial. Para aplicar estos cambios debes publicar worker.js en Cloudflare; cambiar solo index.html NO actualiza el modelo. La cuota gratuita y limites de modelo pueden variar. Verifica el uso en tu cuenta.
