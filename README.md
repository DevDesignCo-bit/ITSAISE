# ITSAI Sverige
Abre index.html en un navegador. Frontend local sin instalación ni dependencias externas.

## Páginas
- index.html: móvil, sueco por defecto.
- index.html?lang=en: móvil en inglés.
- pin.html: PIN en sueco.
- pin.html?lang=en: PIN en inglés.
- terms.html: términos en sueco.
- privacy.html: privacidad en sueco.

Las landings conservan los diseños locales: fondo negro, imagen del robot, logo, formulario gris y botones verdes. El layout pasa a dos columnas en desktop desde 900 px. Se mantiene el selector SE/EN, el precio de 100 SEK por semana, +18, STOP ITSAI+ al 72300 y el proveedor Next Move Digital LTD.
El PIN sueco usa la etiqueta sueca «Ange PIN-koden» en vez del texto inglés que conserva el mock.
Todos los enlaces del footer funcionan localmente. La vuelta desde las páginas legales conserva paso e idioma. Las páginas legales se muestran en sueco también desde la landing inglesa.
Las etiquetas dentro de img.png forman parte de la imagen original.
Se mantienen todos los PNG de referencia sin modificarlos. logo.png es una copia del logo local.
El teléfono [XXXXXXXXX] se conserva de la referencia. Sustituir en index.html y pin.html cuando exista el número real.

## Modo de prueba
Cualquier número de móvil y cualquier PIN funcionan; no hay validación de país, formato o longitud.
Fortsätt/Continue abre el paso PIN. Bekräfta/Confirm muestra la confirmación de prueba.
No se envían SMS, no se verifica un PIN real, no se activa ninguna suscripción y no se realizan cobros.
Los números y PIN no se incluyen en URL, logs ni almacenamiento.
El parpadeo de botones es suave y respeta la preferencia de movimiento reducido.

## Fuentes y adaptaciones legales
Consultado el 28 de octubre de 2026.
El enlace proporcionado https://itsai-online.com/terms-and-conditions carga título y navegación, pero no muestra el cuerpo legal. Ya ocurría en la recreación local itsai-customer-care.
Se ha usado como base el texto de ItsAI indexado en https://stage.itsai-online.com/terms-and-conditions. No se presenta como una traducción verificada del cuerpo actualmente publicado en producción.
Se han concretado los marcadores del país, precio, divisa y periodo usando el diseño: Suecia, 100 SEK, semanal; se ha aplicado el requisito +18 de la landing y su instrucción de cancelación por SMS.
Se conserva identificada como referencia del original la mención histórica a Data Protection Act 1998.
Los datos societarios corresponden a Next Move Digital LTD, no a Playwing.
La privacidad se traduce de la política oficial de la empresa https://www.nextmove.digital/privacy, leída directamente en navegador: fecha 2 de julio de 2025 y siete apartados. Se añade el correo support@itsai-online.com del diseño como contacto del servicio.
No se han reutilizado políticas de Mind+ ni el contenido de otro servicio para la versión final.

## Comprobación
JavaScript: sintaxis verificada con node --check app.js y node --check legal.js.
HTML y recursos: 32 referencias locales, identificadores, etiquetas de campos, idioma, identidad del servicio y UTF-8 comprobados sin errores. Campos sin restricciones de formato ni longitud.
La revisión visual local en navegador no está disponible en este entorno. No se ha realizado ninguna publicación.
