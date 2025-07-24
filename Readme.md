# Proyecto: QR de Contacto Personal

Este proyecto contiene los archivos para crear una URL que, al ser visitada desde un celular, permite guardar un contacto directamente en la agenda del teléfono.

## ¿Cómo Funciona?

Un código QR apunta a una URL. Esa URL contiene una página web (un archivo `index.html`) que le entrega al navegador un archivo de contacto virtual (`.vcf`). Los sistemas operativos móviles (iOS y Android) reconocen este archivo y abren la aplicación de "Contactos" con toda la información precargada.

## Opciones Disponibles

En este repositorio encontrarás dos métodos para lograr el mismo resultado.

### Opción 1: Archivo Único (Recomendado)

* **Archivo:** `index.html`
* **Descripción:** Es la solución más limpia y moderna. Toda la información del contacto está incrustada dentro del propio archivo HTML. No necesitas nada más.
* **Ventaja:** Solo tienes que gestionar, editar y subir un único archivo.

### Opción 2: Archivos Separados

* **Archivos:** `index.html` y `contacto.vcf`
* **Descripción:** Es el método tradicional. La página `index.html` es muy simple y su única función es redirigir inmediatamente al navegador para que descargue el archivo `contacto.vcf`.
* **Ventaja:** La información del contacto está en un archivo `.vcf` limpio, que puedes compartir o usar para otros fines si lo necesitas.

## Pasos para Ponerlo en Marcha

1.  **Elige una opción.** Para la mayoría, la **Opción 1** es la mejor.
2.  **Edita los datos.** Abre el archivo (`index.html` en la Opción 1, o `contacto.vcf` en la Opción 2) con un editor de texto y reemplaza los datos de ejemplo de "Diego Rojas" con los tuyos.
3.  **Sube los archivos a un hosting.** Para que el QR funcione, los archivos deben estar en internet. Puedes usar servicios gratuitos:
    * **GitHub Pages:** Ideal si ya usas GitHub.
    * **Netlify:** Muy fácil de usar, simplemente arrastra y suelta la carpeta con tus archivos.
    * **Vercel** o **Cloudflare Pages** son otras excelentes alternativas.
4.  **Obtén tu URL pública.** Una vez subido, el servicio te dará una URL pública (ej: `https://mi-nombre.netlify.app`).
5.  **Crea tu Código QR.** Usa cualquier generador de códigos QR online. Cuando te pida la URL, introduce la que obtuviste en el paso anterior.
6.  **¡Prueba!** Escanea el QR con tu celular para confirmar que todo funciona como esperas.
