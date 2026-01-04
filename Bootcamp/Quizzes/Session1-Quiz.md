# HTML Basics — Pyetje & Përgjigje

Përmbledhje e koncepteve kryesore të **HTML (HyperText Markup Language)**.  

---

## Përmbajtja

1. [Çka është HTML?](#1-çka-është-html)
2. [Llojet e tag-eve](#2-llojët-e-tag-eve)
3. [Struktura e dokumentit HTML](#3-struktura-e-dokumentit-html)
4. [Çka vendoset në `<head>`](#4-çka-vendoset-në-head)
5. [Çka vendoset në `<body>`](#5-çka-vendoset-në-body)
6. [Si renderohen elementet](#6-si-renderohen-elementet)
7. [Block vs Inline](#7-block-vs-inline)
8. [Comments në HTML](#8-comments-në-html)
9. [Etiketa të tekstit](#9-etiketa-të-tekstit)
10. [Etiketat semantike](#10-etiketat-semantike)
11. [Semantike vs të zakonshme](#11-semantike-vs-të-zakonshme)
12. [4 etiketa semantike](#12-4-etiketa-semantike)
13. [Llojet e listave](#13-llojët-e-listave)
14. [Tags e secilës listë](#14-tags-e-secilës-listë)
15. [Linket dhe atributet](#15-linket-dhe-atributet)
16. [Llojet e linkeve](#16-llojët-e-linkeve)
17. [`img` vs `figure`](#17-img-vs-figure)
18. [Tags për imazhe dhe figura](#18-tags-për-imazhe-dhe-figura)

---

 ## 1. Cka eshte HTML


HTML është një gjuhë përshkruese që përdoret për të ndërtuar **strukturën e faqeve web**.  
Nuk është gjuhë programimi. HTML i tregon browser-it se si organizohet dhe shfaqet përmbajtja e faqes.

---

## 2. Llojët e tag-eve

### 2.1 Tags hapëse dhe mbyllëse
Kanë një tag hapës dhe një tag mbyllës.

```html
<p>Tekst</p>

### 2.2 Tags vetë-mbyllëse (self-closing)

Këto tag-e nuk kanë nevojë për tag mbyllës.

```html
<img />
<br />
<hr />
```
---
## 3. Struktura e dokumentit HTML

Çdo dokument HTML ka një strukturë bazë që i tregon browser-it
si të lexojë dhe shfaqë faqen.

```html
<!DOCTYPE html>
<html>
  <head>
    <!-- Meta tags, title, CSS -->
  </head>
  <body>
    <!-- Përmbajtja e dukshme e faqes -->
  </body>
</html>
```
---
## 4. Çka vendoset në `<head>`?

Pjesa `<head>` e dokumentit HTML përmban informacione që **nuk shfaqen direkt**
në faqen web, por janë të rëndësishme për browser-in dhe motorët e kërkimit.

Elementet kryesore që vendosen në `<head>` janë:

- `<meta>` – përcakton charset, viewport, description, keywords
- `<title>` – titulli i faqes që shfaqet në tab-in e browser-it
- `<link>` – përdoret për të lidhur stylesheet-et (CSS)
- Metadata për SEO dhe identitetin e faqes (favicon, etj.)

---

## 5. Çka vendoset në `<body>`?

Pjesa `<body>` përmban **përmbajtjen e dukshme** të faqes web,
e cila shfaqet direkt në browser.

Në `<body>` zakonisht vendosen:

- Tekste (tituj, paragrafë, citime)
- Imazhe (`<img>`)
- Linke (`<a>`)
- Lista (`<ul>`, `<ol>`)
- Tabela (`<table>`)
- Forma (`<form>`)
## 6. Si renderohen elementet në browser?

Në HTML, elementet shfaqen në browser sipas mënyrës se si janë të
përcaktuara për t’u renderuar. Më së shpeshti, ato ndahen në dy grupe:

- **Block elements**
- **Inline elements**

Kjo ndarje ndikon në mënyrën se si elementet pozicionohen dhe
si sillen ndaj elementeve të tjerë në faqe.

---

## 7. Block vs Inline

### Block elements
- Zënë gjithë gjerësinë e rreshtit (full-width)
- Fillojnë gjithmonë në rresht të ri
- Mund të përmbajnë elemente të tjerë brenda tyre

Shembuj të zakonshëm:
`<div>`, `<p>`, `<h1>` – `<h6>`, `<section>`

### Inline elements
- Zënë vetëm hapësirën e përmbajtjes së tyre
- Nuk fillojnë rresht të ri
- Shfaqen brenda rreshtit me elemente të tjerë

Shembuj të zakonshëm:
`<span>`, `<a>`, `<strong>`, `<em>`

---


## 8. Comments në HTML

Comments në HTML përdoren për **shpjegim, dokumentim dhe mirëmbajtje**
të kodit, pa u shfaqur në faqen web.

Ato ndihmojnë zhvilluesit të kuptojnë më lehtë strukturën dhe logjikën
e kodit, sidomos në projekte më të mëdha.

Browser-i **nuk i shfaq comments**.

```html
<!-- Ky është një comment në HTML 
```

---

## 9. Etiketa të tekstit në HTML

HTML përdor etiketa të ndryshme për **formatimin dhe organizimin e tekstit**
brenda faqes web. Këto etiketa ndihmojnë në theksimin e përmbajtjes
dhe përmirësojnë lexueshmërinë.

Etiketa më të përdorura të tekstit janë:

- **Bold / Trashë:** `<b>`, `<strong>`
- **Italic / Pjerrët:** `<i>`, `<em>`
- **Underline / Nënvizim:** `<u>`
- **Subscript / Superscript:** `<sub>`, `<sup>`
- **Tituj / Headers:** `<h1>` deri `<h6>`

---

## 10. Etiketat semantike

Etiketat semantike janë etiketa HTML që tregojnë **kuptimin dhe rolin**
e përmbajtjes në strukturën e faqes web.

Ato ndihmojnë:
- Browser-in dhe motorët e kërkimit (SEO)
- Accessibility për përdoruesit
- Strukturë më të pastër dhe më të kuptueshme të kodit

Shembuj të etiketave semantike:
`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`

---

## 11. Semantike vs të zakonshme

Në HTML ekziston dallim mes **etiketave të zakonshme** dhe **etiketave semantike**.

- **Etiketat e zakonshme** (p.sh. `<div>`, `<span>`)  
  Nuk tregojnë kuptim logjik për përmbajtjen; përdoren kryesisht për strukturë ose stilim.

- **Etiketat semantike** (p.sh. `<header>`, `<nav>`, `<main>`, `<footer>`)  
  Tregojnë qartë rolin e përmbajtjes në faqe dhe ndihmojnë në:
  - përmirësimin e SEO
  - accessibility
  - strukturë më të lexueshme të kodit

---

## 12. 4 etiketa semantike

Disa nga etiketat semantike më të përdorura në HTML janë:

- `<header>` – për pjesën e sipërme të faqes (titull, logo, menu)
- `<nav>` – për navigacionin e faqes
- `<main>` – për përmbajtjen kryesore të faqes
- `<footer>` – për pjesën e poshtme të faqes (copyright, linke)

---

## 13. Llojët e listave

Në HTML ekzistojnë tre lloje kryesore listash, të cilat përdoren për të
organizuar përmbajtjen në mënyrë të strukturuar.

- **Ordered list** – listë e renditur me numra
- **Unordered list** – listë e parenditur me pika
- **Description list** – listë përshkruese për terma dhe shpjegime

---

## 14. Tags e secilës listë

Çdo lloj liste në HTML përdor tag-et e veta karakteristike.

- **Ordered list:** `<ol>` dhe `<li>`
- **Unordered list:** `<ul>` dhe `<li>`
- **Description list:** `<dl>`, `<dt>` dhe `<dd>`

---

## 15. Linket dhe atributet

Tagu për krijimin e linkeve në HTML është `<a>`.

Atributet kryesore të këtij tagu janë:
- **`href`** – specifikon adresën (URL) ku çon linku
- **`target`** – përcakton ku hapet linku (p.sh. `_blank` për dritare të re)
- **`title`** – shton një përshkrim të shkurtër që shfaqet si tooltip

Shembull:
```html
<a href="https://example.com" target="_blank" title="Example">Example</a>
```

----

## 16. Llojët e linkeve

Në HTML, linket përdoren për të lidhur faqe dhe burime të ndryshme.
Ekzistojnë dy lloje kryesore linkesh:

- **Linke të brendshme (Internal links)**  
  Përdoren për të lidhur faqe brenda të njëjtit website ose projekt.

- **Linke të jashtme (External links)**  
  Përdoren për të lidhur faqe ose burime në internet.

---

## 17. `img` vs `figure`

Në HTML ekziston dallim mes përdorimit të tagut `<img>` dhe `<figure>`.

- **`<img>`**  
  Përdoret për të shfaqur vetëm imazhin në faqe.

- **`<figure>`**  
  Përdoret për të shfaqur imazhin bashkë me një përshkrim (`<figcaption>`),
  zakonisht kur imazhi ka kuptim kontekstual.

---

## 18. Tags për imazhe dhe figura

Për të punuar me imazhe dhe figura në HTML përdoren këto tagje:

- **`<img>`** – për shfaqjen e imazheve
- **`<figure>`** – për përfshirjen e imazhit
- **`<figcaption>`** – për përshkrimin e imazhit

Shembull:
```html
<figure>
  <img src="foto.jpg" alt="Foto shembull">
  <figcaption>Përshkrimi i fotos</figcaption>
</figure>
```