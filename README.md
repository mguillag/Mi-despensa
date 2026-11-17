# Mi despensa — primera versión

## Qué incluye
- Inventario por zonas: Despensa, Nevera, Congelador y Despensa emergencia.
- Cantidades y unidades.
- Registro por lote con fecha de caducidad, consumo preferente o fecha orientativa tras apertura.
- Orden de prioridad por fecha.
- Búsqueda de productos por código de barras mediante Open Food Facts.
- Escáner con `BarcodeDetector` cuando el navegador lo soporta; introducción manual como alternativa.
- Datos guardados localmente en el navegador y exportación JSON.
- Diseño adaptable a iPhone y Android, con manifiesto PWA y service worker.

## Limitaciones de esta versión
Esta es una primera versión local: cada navegador/dispositivo tiene su propia despensa. Todavía no hay cuentas familiares, sincronización entre móviles ni notificaciones push programadas. Esas funciones requieren añadir autenticación y una base de datos compartida (por ejemplo, Supabase) y configurar permisos/avisos.

Las notificaciones programadas en segundo plano no se garantizan en una PWA, especialmente en iOS. En una siguiente fase podemos implementar avisos dentro de la app y estudiar push web con un servicio compatible.

## Probar
Abre `index.html` para probar el inventario. La cámara y la instalación PWA requieren servir la carpeta desde HTTPS o `localhost`. Para compartirla online, publica estos archivos en un hosting estático HTTPS, como GitHub Pages.

## Privacidad
Los productos se guardan en `localStorage` del navegador. La consulta de códigos de barras envía el código a Open Food Facts para buscar los datos del producto. No introduzcas información sensible.
