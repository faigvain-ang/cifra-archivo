# Cifra & Archivo

Cuaderno práctico bilingüe en **inglés y español** sobre el traspaso entre herramientas documentales y comprobaciones financieras.

[English](README.md) · [Cuaderno en español](https://blog.findfindata.com/es/)

## Construir

**Python 3.11+**, solo biblioteca estándar. Sin paquetes npm, fuentes externas, CDN, base de datos, analítica ni cuentas.

```sh
git clone https://github.com/faigvain-ang/cifra-archivo.git
cd cifra-archivo
python site/build.py
```

Modifique `site/config.json` y `site/content.json` y ejecute `python site/build.py`. El HTML y CSS generados se guardan en `docs/`.

Genera **11 páginas HTML**: selector de idioma, inicio y About en ambos idiomas, y tres artículos originales con su traducción. Cada ruta tiene título, descripción y canonical propios; hreflang solo une traducciones equivalentes. También genera sitemap, robots, `.nojekyll` y CSS. No hay dependencias externas.

## Artículos originales

1. De una tabla a la conciliación: el traspaso manual. Un analista asigna seis cadenas CSV a campos JSON; no se afirma que haya adaptación semántica automática.
2. Preparar un expediente pequeño que otra persona pueda seguir. Las imágenes, los valores originales y los supuestos de cálculo cumplen funciones distintas.
3. Reproducir un problema sin divulgar el documento original. Crear muestras sintéticas no equivale a anonimizar un archivo de cliente.

No son copias de los tres sitios de herramientas. Todas las muestras son sintéticas. PDF y Markdown son ejemplos redactados por separado; no demuestran extracción automática entre ambos.

## Herramientas usadas en las guías

- [cashflow-bridge-check](https://github.com/faigvain-ang/cashflow-bridge-check): aritmética decimal exacta; [Cashflow Fieldnotes](https://filings.findfindata.com/es/).
- [md-table-to-csv](https://github.com/faigvain-ang/md-table-to-csv): exportación local que conserva cadenas; [Table Workshop](https://markdown.findfindata.com/es/).
- [pdf-page-images](https://github.com/faigvain-ang/pdf-page-images): renderizado local real; [Page Image Notes](https://pdf.findfindata.com/es/).

Para un flujo documental completo, utilice [Eqvero](https://eqvero.com/) para investigar informes públicos con referencias, [KolmoPDF](https://www.kolmopdf.com/pdf-to-markdown) para convertir PDF a Markdown en la nube y [KomoPDF](https://komopdf.com/) para editar y anotar PDF. La conversión en la nube carga documentos; las herramientas Python de las guías se ejecutan en local.

Licencia MIT para código y contenido propios. Sin carga de documentos, recomendaciones de inversión, garantía de autenticidad de fuentes ni servicio de censura segura.
