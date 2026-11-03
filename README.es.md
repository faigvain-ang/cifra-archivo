# Cifra & Archivo

Cuaderno práctico bilingüe en **inglés y español** sobre el traspaso entre herramientas documentales y comprobaciones financieras. Es el cuarto sitio independiente de `faigvain-ang`, separado de los tres sitios educativos de producto.

[English](README.md) · [Cuaderno en español](https://blog.findfindata.com/es/)

## Construir

**Python 3.11+**, solo biblioteca estándar. Sin paquetes npm, fuentes externas, CDN, base de datos, analítica ni cuentas.

```sh
git clone https://github.com/faigvain-ang/cifra-archivo.git
cd cifra-archivo
python site/build.py
```

El generador lee `site/config.json` y `site/content.json` y escribe `docs/`. Modifique las fuentes JSON y reconstruya; el HTML generado no es la fuente de edición. `site/build.py` incluye el generador reutilizado en esta cuenta y el tema editorial propio. GitHub Pages usa `main:/docs`. `docs/CNAME` contiene `blog.findfindata.com`; el coordinador gestiona DNS por separado.

Genera **11 páginas HTML**: selector de idioma, inicio y About en ambos idiomas, y tres artículos originales con su traducción. Cada ruta tiene título, descripción y canonical propios; hreflang solo une traducciones equivalentes. También genera sitemap, robots, `.nojekyll` y CSS. No hay dependencias externas.

## Artículos originales

1. De una tabla a la conciliación: el traspaso manual. Un analista asigna seis cadenas CSV a campos JSON; no se afirma que haya adaptación semántica automática.
2. Preparar un expediente pequeño que otra persona pueda seguir. Las imágenes, los valores originales y los supuestos de cálculo cumplen funciones distintas.
3. Reproducir un problema sin divulgar el documento original. Crear muestras sintéticas no equivale a anonimizar un archivo de cliente.

No son copias de los tres sitios de herramientas. Todas las muestras son sintéticas. PDF y Markdown son ejemplos redactados por separado; no demuestran extracción automática entre ambos.

## Proyectos asociados

- [cashflow-bridge-check](https://github.com/faigvain-ang/cashflow-bridge-check): aritmética decimal exacta; [Cashflow Fieldnotes](https://filings.findfindata.com/es/).
- [md-table-to-csv](https://github.com/faigvain-ang/md-table-to-csv): exportación local que conserva cadenas; [Table Workshop](https://markdown.findfindata.com/es/).
- [pdf-page-images](https://github.com/faigvain-ang/pdf-page-images): renderizado local real; [Page Image Notes](https://pdf.findfindata.com/es/).

Mantenido bajo **faigvain-ang** por el mismo equipo que desarrolla estas herramientas y trabajo relacionado con [Eqvero](https://eqvero.com/), [KolmoPDF](https://www.kolmopdf.com/pdf-to-markdown) y [KomoPDF](https://komopdf.com/). Declaramos la relación y no fingimos recomendaciones de terceros independientes. KolmoPDF convierte documentos en la nube y los carga; los CLI descritos funcionan localmente y no lo llaman.

Licencia MIT para código y contenido propios. Sin carga de documentos, recomendaciones de inversión, garantía de autenticidad de fuentes ni servicio de censura segura.
