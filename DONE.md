# Barbería Bruma · completado

Sitio estático multipágina, sin build ni dependencias de ejecución:
- index.html — inicio editorial, hero con bruma CSS y control de pausa.
- servicios.html — corte/fade, barba y combinado.
- galeria.html — cinco imágenes con ampliación modal accesible por teclado.
- contacto.html — WhatsApp demo, datos pendientes y preguntas frecuentes.
- styles.css + main.js compartidos; fuentes locales en assets/fonts/.
- Cinco PNG imagegen en assets/images/ (hero 16:9, restantes 4:3), más WebP para entrega optimizada. Prompts completos y método en assets/images/PROMPTS.md.
- noindex/nofollow en las cuatro páginas y X-Robots-Tag en _headers.
- Footer compartido con “Demo conceptual”. WhatsApp +54 11 5555-0606.

## Uso local
Desde esta carpeta: `python3 -m http.server 8066` y abrir http://localhost:8066.
No se ejecutó git ni se publicó el sitio.

## Verificación realizada
Chrome headless mediante Playwright: cuatro páginas a 390 y 1280 px, un h1 por página, cero imágenes rotas, sin desbordes horizontales, sin page errors ni respuestas 4xx/5xx. Menú móvil abre y cierra con Escape. Modal abre y cierra con Escape. Pausa de niebla verificada. prefers-reduced-motion produce animation-name: none. Enlaces y assets locales comprobados. Capturas completas en .qa/ y script reproducible check.cjs (ruta de Playwright propia del entorno).

Revisión visual de inicio desktop/móvil y contacto móvil: jerarquía, recorte de fotos, contraste y ritmo correctos. Navegación semántica, skip link, foco visible, details/summary nativos y modal nativo. No se afirma auditoría exhaustiva de accesibilidad. Las cabeceras de _headers requieren un hosting que soporte ese formato; el servidor Python no las aplica. No se contactó al número demo ni se verificó una reserva real.

## Contenido pendiente para un negocio real
Dirección exacta, horarios, precios, medios de pago, integrantes e imágenes reales autorizadas. Todos los datos faltantes se indican como pendientes; no hay reseñas, credenciales ni horarios inventados. spec.md registra dirección visual y referencias.
