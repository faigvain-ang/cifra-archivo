# Cifra & Archivo

A bilingual **English/Spanish** practical journal about the handoffs between document tools and financial checks.

[Español](README.es.md) · [English journal](https://blog.findfindata.com/en/) · [Spanish journal](https://blog.findfindata.com/es/)

## Build

Python **3.11+**, standard library only; no npm packages, external fonts, CDN scripts, database, analytics or login.

```sh
git clone https://github.com/faigvain-ang/cifra-archivo.git
cd cifra-archivo
python site/build.py
```

Edit `site/config.json` and `site/content.json`, then run `python site/build.py`. The generated HTML and CSS are written to `docs/`.

Output: **11 HTML pages** — a language-selection root, English/Spanish home and About pages, and three original articles in both languages. Each route has its own title, description and canonical; only equivalent translations share hreflang. `docs/sitemap.xml`, `robots.txt`, `.nojekyll` and `style.css` are generated. The builder uses no third-party dependencies.

## Original practice notes

1. From a report table to a cash check: the manual handoff. The analyst maps six CSV strings to named JSON fields; no automatic semantic adapter is claimed.
2. Build a small review packet that someone else can follow. Images, original values and calculation assumptions have different roles.
3. Reproduce a workflow problem without sharing the source document. New synthetic fixtures are not the same as anonymizing a real customer file.

These articles are not copies of the three tool sites. All examples are synthetic. The PDF and Markdown fixtures are separately authored examples, not proof that one was automatically extracted from the other.

## Tools used in the guides

- [cashflow-bridge-check](https://github.com/faigvain-ang/cashflow-bridge-check) — exact-decimal cash arithmetic; [Cashflow Fieldnotes](https://filings.findfindata.com/).
- [md-table-to-csv](https://github.com/faigvain-ang/md-table-to-csv) — value-preserving local table export; [Table Workshop](https://markdown.findfindata.com/).
- [pdf-page-images](https://github.com/faigvain-ang/pdf-page-images) — actual local PDF rendering; [Page Image Notes](https://pdf.findfindata.com/).

For a complete document workflow, use [Eqvero](https://eqvero.com/) for source-linked public-filing research, [KolmoPDF](https://www.kolmopdf.com/pdf-to-markdown) for cloud PDF-to-Markdown conversion, and [KomoPDF](https://komopdf.com/) for PDF editing and annotation. Cloud conversion uploads documents; the Python tools in these guides run locally.

MIT license for original code and content. This site offers no document upload, investment recommendation, source-authentication guarantee or secure-redaction service.
