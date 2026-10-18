# TBOX PDF Redact

Censura destructiva, unión y revisión de documentos PDF para Windows. Todo el procesamiento ocurre en el equipo: los documentos no se suben a ningún servidor.

- Sitio oficial: https://tbox.cl/sitio/pdf-redact/
- Versión vigente: 2.2.1
- Requisitos: Windows 10 x64 o superior

## Qué hace

- Censura irreversible de datos sensibles: RUT, nombres y correos.
- División de expedientes pesados por peso real en MB.
- OCR local en español para documentos escaneados.
- Unión, reordenamiento, borrado y extracción de páginas.
- Inspector de firmas electrónicas X.509 y PKCS#7.
- Impresión a PDF y trabajo con varias pestañas en la misma ventana.

## Descarga e instalación

El instalador se obtiene desde el sitio oficial o desde la sección de publicaciones de este repositorio:

https://tbox.cl/sitio/download.php?format=exe

La versión 1.6.0 se conserva en las publicaciones anteriores como cadena heredada, en formato portable.

## Verificación de la descarga

Cada publicación incluye el archivo `.sha256` con la huella del instalador. En Windows, con PowerShell:

```
Get-FileHash .\TBOX-PDF-Redact-Instalador-2.2.1.exe -Algorithm SHA256
```

El valor obtenido debe coincidir con el de la publicación y con el que aparece en la página del producto. La aplicación no se ejecuta sola al descargar y no envía información a internet.

## Actualizaciones

El programa consulta el canal oficial en este orden: las publicaciones de este repositorio y, si no responde, el manifiesto `https://tbox.cl/sitio/version.json`. Cuando hay una versión posterior, la muestra junto con sus notas y abre la página de descarga en el navegador. No instala nada por su cuenta.

## Firma digital

Los instaladores no están firmados con un certificado de firma de código. Por esa razón algunos navegadores muestran una advertencia al descargar el ejecutable. La alternativa es el archivo `.zip` de la misma publicación. En cualquier caso, verificar la huella SHA-256 antes de ejecutar el programa.

La firma de código es el único mecanismo que elimina esa advertencia de forma definitiva; su tramitación está pendiente.

## Aviso legal

TBOX PDF Redact es software propietario de TBOX Chile. Este repositorio se publica únicamente como canal de distribución de los instaladores y de sus huellas de verificación. No se distribuye el código fuente ni se concede licencia de uso sobre él.

Las capturas, los textos y la marca pertenecen a TBOX Chile. Para consultas comerciales, usar el formulario del sitio oficial.
