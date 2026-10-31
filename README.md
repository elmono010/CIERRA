# CIERRA — Seguimiento de cotizaciones para técnicos independientes

CIERRA ayuda a técnicos independientes (electricistas, plomeros, técnicos de aire, carpinteros, pintores) a no perder trabajos por olvido.

Un técnico visita, cotiza, el cliente dice "lo pienso" y el trabajo se pierde porque nadie hace seguimiento al día 1, 3 y 7. Cada trabajo perdido es ganancia perdida.

## Qué hace (MVP, versión gratuita)

- Crear cotizaciones: cliente, trabajo, precio, costo de materiales, ganancia estimada, fecha.
- Seguimiento: qué toca hoy (día 1, 3 y 7).
- Seguimiento por WhatsApp en 1 clic: abre el mensaje listo para enviar. CIERRA no envía nada por sí mismo y no usa APIs de pago.
- Estados: pendiente, aceptada, perdida con motivo.
- Resumen: cotizaciones totales, valor pendiente, tasa de cierre, ganancia de trabajos cerrados.
- Cotización en PDF: vista imprimible desde el navegador.
- Exportar / importar respaldo JSON.

## Qué NO hace (a propósito)

No es un ERP genérico, no es agenda completa, no es inventario, no es facturación completa, no es CRM para empresas. Cada función debe ayudar a cerrar una cotización, recuperar un trabajo perdido o mostrar la ganancia real.

## Arquitectura con 0 dólares

- PWA en HTML, CSS y JavaScript, sin dependencias externas.
- Datos en el dispositivo del usuario (localStorage en este MVP; la hoja de ruta es IndexedDB).
- Sin servidor, sin VPS, sin base de datos en la nube, sin APIs de pago.
- Publicación: GitHub Pages (gratuita).
- Los datos de pago nunca se publican en este repositorio. La activación Pro se coordina por mensaje privado.

## Modelo freemium

- Free: hasta 5 cotizaciones activas.
- Pro mensual: 6,99 USD
- Pro anual: 49 USD
- Licencia de por vida: 79 USD

Precios de lanzamiento. La activación Pro se coordina por mensaje privado desde la publicación oficial. No se deben publicar datos de pago en comentarios públicos.

## Uso

Abre `index.html` o la página de GitHub Pages, crea una cotización y usa el resumen "Toca hoy". Haz respaldo con Exportar JSON con regularidad, porque los datos viven en tu dispositivo.

## Límites honestos

- Sin sincronización entre dispositivos en el MVP.
- Sin envío automático de mensajes: el técnico envía el seguimiento.
- Sin verificación bancaria automática.
- No se garantizan clientes ni ingresos. Las simulaciones de ingresos son hipotéticas.

## Regla del producto

No se añade una función que no ayude a cerrar una cotización, recuperar un trabajo perdido o mostrar la ganancia real de un trabajo.
