# Guida Pratica alla Struttura e Marcatura HTML

Questo documento funge da guida riassuntiva per comprendere l'anatomia di una pagina HTML, dai metadati fondamentali fino alla marcatura dei contenuti testuali e multimediali.

---

## 🏗️ La Struttura di Base del Documento

Ogni pagina HTML segue una gerarchia precisa per garantire che il browser interpreti correttamente il contenuto:

* **`<!doctype html>`**: Preambolo obbligatorio per garantire il corretto funzionamento del documento.
* **`<html>`**: L'elemento radice che racchiude tutto il contenuto. Include l'attributo `lang` per la lingua.
* **`<head>`**: Contenitore per i metadati (CSS, titoli, set di caratteri) non visibili direttamente agli utenti.
    * **`<meta charset="utf-8">`**: Imposta la codifica dei caratteri per gestire quasi tutte le lingue scritte.
    * **`<meta name="viewport">`**: Ottimizza la visualizzazione su dispositivi mobili.
    * **`<title>`**: Definisce il titolo che appare nella scheda del browser.
* **`<body>`**: Contiene tutto il contenuto visibile: testo, immagini, video e link.

---

## 🖼️ Incorporamento delle Immagini

Per inserire immagini si utilizza il tag **vuoto** (o *void*) `<img>`:

```html
<img src="images/nome-file.png" alt="Descrizione accurata dell'immagine" />
```
---

## ✍️ Marcatura del Testo e dei Contenuti

Oltre alle immagini, una pagina web è composta principalmente da testo strutturato e collegamenti.

### 1. Titoli e Paragrafi
L'HTML utilizza tag semantici per dare gerarchia al testo:
* **`<h1>` fino a `<h6>`**: Definiscono i titoli (Headings). L'`<h1>` è il titolo principale della pagina, mentre gli altri servono per i sottotitoli.
* **`<p>`**: Sta per "paragrafo" e si usa per racchiudere i normali blocchi di testo discorsivo.

### 2. Collegamenti Ipertestuali (Link)
Per rendere il web navigabile, si usa il tag **`<a>`** (Anchor):
```html
<a href="https://www.mozilla.org/">Visita Mozilla</a>