RR GARAGE WORKSHOP — GITHUB / PWA v2.2.2

URL DE APPS SCRIPT CONFIGURADA
------------------------------
https://script.google.com/macros/s/AKfycbybNlUFW0yJPejxwKuFhHdEQogrgGvg_JR2GAv_E6OcQ8cydz2-Nn-hclBh6vBhW7B5xw/exec

ARCHIVOS A SUBIR A LA RAÍZ DEL REPOSITORIO "workshop"
------------------------------------------------------
- index.html
- manifest.webmanifest
- apple-touch-icon.png
- icon-192.png
- icon-512.png
- favicon-64.png
- .nojekyll

PASOS
-----
1. En GitHub abre el repositorio:
   rrgarage/workshop

2. Reemplaza los archivos anteriores por los de este paquete.
   Todos deben quedar en la raíz, al mismo nivel.

3. Commit changes.

4. En Settings -> Pages verifica:
   Source: Deploy from a branch
   Branch: main
   Folder: /(root)

5. Espera 1-2 minutos y abre:
   https://rrgarage.github.io/workshop/?v=222

IPHONE
------
1. Abre la URL anterior en Safari.
2. Compartir.
3. Agregar a pantalla de inicio.
4. Nombre: RR Garage.

Si ya existe un acceso directo antiguo:
- elimínalo;
- abre nuevamente la URL;
- vuelve a agregarlo a pantalla de inicio.
iOS suele guardar iconos y nombres en caché.

IMPORTANTE
----------
GitHub NO contiene:
- Código.gs
- Google Sheets
- API keys
- PDFs
- datos de clientes

GitHub solo muestra la Web App de Apps Script dentro de un iframe.

La implementación de Apps Script debe mantener:
.setXFrameOptionsMode(HtmlService.XFrameOptionsMode.ALLOWALL)

No se incluye service worker a propósito, para evitar que iPhone/Chrome
mantengan una versión antigua de RR Garage en caché durante el desarrollo.
