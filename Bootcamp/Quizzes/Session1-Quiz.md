# 📘 HTML – Pyetje & Përgjigje

## 1. Çka është HTML?

**HTML** (*HyperText Markup Language*) është një gjuhë përshkruese që përdoret për të ndërtuar dhe përshkruar strukturën e faqeve web.  
Ajo i tregon browser-it se si është e organizuar përmbajtja e faqes.
---

## 2. Çfarë lloje të tag-eve kemi në HTML?

Në HTML kemi dy lloje kryesore të tag-eve:

### 🔹 1. Tags hapëse dhe mbyllëse
Këta tag-e kanë një tag hapës dhe një mbyllës.

Shembull:
```html
<p>Teksti</p> 
```
### 🔹 2. Tags vetë-mbyllëse (self-closing)
Këta tag-e nuk kanë nevojë për tag mbyllës.

```html
<img />
<br />
<hr />
```

---

## 3. Struktura e një dokumenti HTML

Struktura bazë e një dokumenti HTML përbëhet nga disa pjesë kryesore:

```html
<!DOCTYPE html>
<html>
  <head>
    <!-- Këtu vendosen meta, title, link-et për CSS etj. -->
  </head>
  <body>
    <!-- Këtu shkruhet përmbajtja e faqes -->
  </body>
</html>
```
---
## 4. Çka vendoset në `<head>`?

Pjesa `<head>` e dokumentit HTML përmban informacion që nuk shfaqet direkt në faqen e web, por është i rëndësishëm për browser-in dhe SEO.

### 🔹 Elementët kryesorë që vendosen në `<head>`:

- **Meta etiketat** (`<meta>`)  
  Përdoren për të specifikuar karakteret, përshkrimin e faqes, keywords, etj.

- **Titulli i faqes** (`<title>`)  
  Shfaqet në skedën e browser-it dhe ndihmon në identifikimin e faqes.

- **Lidhjet me CSS** (`<link>`)  
  Për të lidhur stylesheet-et që japin stilin e faqes.

- **Informacione për browser-in dhe SEO**  
  Përfshin favicon, script-et e nevojshme, dhe metadata për motorët e kërkimit.
---

## 5. Çka vendoset në `<body>`?

Pjesa `<body>` e dokumentit HTML përmban **përmbajtjen e dukshme** të faqes që shfaqet në browser.

### 🔹 Elemente të zakonshme që vendosen në `<body>`:

- **Tekstet** – Paragrafë, tituj, citime etj.
- **Imazhet** – `<img>` për të shtuar grafika dhe foto.
- **Linket** – `<a>` për të lidhur faqe të tjera ose burime.
- **Listat** – `<ul>` / `<ol>` për listë të renditur ose të pakategorizuar.
- **Tabelat** – `<table>` për të shfaqur të dhëna në formë tabelare.
- **Formularët** – `<form>` për të mbledhur informacione nga përdoruesit.
---

## 6. Si renderohen elementet në browser?

Në HTML, elementet renderohen në mënyrë të ndryshme në browser, kryesisht si:

### 🔹 1. Block elements
- Zënë gjithë gjerësinë e linjës (full-width).
- Fillojnë në një linjë të re.
- Shembuj: `<div>`, `<p>`, `<h1>`–`<h6>`, `<section>`.

### 🔹 2. Inline elements
- Zënë vetëm hapësirën e përmbajtjes së tyre.
- Mund të shfaqen brenda një linje me elemente të tjerë.
- Shembuj: `<span>`, `<a>`, `<strong>`, `<em>`.

---
## 7. Cili është dallimi mes inline dhe block elements?

### 🔹 Block elements
- Zënë **tërë gjerësinë** e linjës (full-width).
- Fillojnë në **rresht të ri**.
- Shembuj: `<div>`, `<p>`, `<h1>`–`<h6>`.

### 🔹 Inline elements
- Zënë vetëm **hapësirën e përmbajtjes së tyre**.
- Nuk kalojnë në rresht të ri.
- Shembuj: `<span>`, `<a>`, `<strong>`, `<em>`.

---
## 8. Çka ndihmojnë comments në HTML?

Comments në HTML përdoren për **shpjegim, dokumentim dhe mirëmbajtje të kodit**, pa u shfaqur në faqen e web.

- Përdoren për të shpjeguar pjesë të kodit.
- Ndihmojnë në **dokumentimin e projektit**.
- E bëjnë kodin më të lehtë për mirëmbajtje.
- Browser-i **nuk i shfaq comments**.

> **Shembull i comment në HTML:**
```html
<!-- Ky është një comment në HTML -->
```
---
## 9. Përmend disa etiketa të tekstit në HTML

HTML ka shumë etiketa për **formatimin e tekstit**. Disa nga më të zakonshmet janë:

- **Bold / Trashë:** `<b>`, `<strong>`  
- **Italic / Pjerrët:** `<i>`, `<em>`  
- **Underline / Nënvizim:** `<u>`  
- **Subscript / Superscript:** `<sub>`, `<sup>`  
- **Tituj / Headers:** `<h1>` deri në `<h6>`

---
## 10. Çka janë etiketat semantike?

**Etiketat semantike** janë etiketa që kanë **kuptim logjik** dhe tregojnë **rolin e përmbajtjes** në faqen web.

- Ndihmojnë browser-in dhe motorët e kërkimit (SEO) të kuptojnë përmbajtjen.  
- Shembuj: `<header>`, `<footer>`, `<article>`, `<section>`, `<nav>`

---

## 11. Dallimi mes etiketave të zakonshme dhe semantike

- **Etiketat e zakonshme** (p.sh. `<div>`)  
  - Nuk japin informacion mbi kuptimin e përmbajtjes.  
- **Etiketat semantike** (p.sh. `<header>`, `<footer>`, `<article>`)  
  - Tregon qartë **rolin e përmbajtjes** në faqe.  
  - Përmirëson **accessibility** dhe **SEO**.

---
## 12. Numëro 4 etiketa semantike

Disa nga etiketat semantike më të përdorura në HTML janë:

- `<header>` – për kokën e faqes (p.sh. titull, menu kryesore).  
- `<nav>` – për navigacionin e faqes.  
- `<main>` – për përmbajtjen kryesore të faqes.  
- `<footer>` – për fundin e faqes (p.sh. copyright, links).  

---
## 13. Çfarë lloje listash ekzistojnë në HTML?

Në HTML ekzistojnë tre lloje kryesore listash:

### 🔹 1. Lista të renditura (Ordered List)
- Përdor `<ol>` dhe `<li>`.  
- Elementët numerohen automatikisht.
- Shembull:
```html
<ol>
  <li>Hapi i parë</li>
  <li>Hapi i dytë</li>
</ol>
```
---
## 14. Tags e secilës listë

Çdo lloj liste në HTML ka tag-et e veta karakteristike:

- **Ordered List (Lista e renditur):** `<ol>` → `<li>`  
- **Unordered List (Lista e parenditur):** `<ul>` → `<li>`  
- **Description List (Lista përshkruese):** `<dl>` → `<dt>` dhe `<dd>`  
---
## 15. Cili është tagu për linke dhe atributet e tij?

Tagu për linke në HTML është `<a>`.

### 🔹 Atributet kryesore të `<a>`:

- **`href`** – specifikon **adresën e linkut**.  
- **`target`** – përcakton **ku hapet linku** (p.sh. `_blank` për të hapur në dritare të re).  
- **`title`** – shton një **përshkrim të shkurtër** që shfaqet si tooltip kur përdoruesi kalon mbi link.  

> **Shembull:**
```html
<a href="https://example.com" target="_blank" title="Shko tek Example">Example</a>
```
---
## 16. Lloje të linkeve

Në HTML ekzistojnë dy lloje kryesore linkesh:

- **Linke të brendshme (Internal Links)** – lidhin faqe brenda **të njëjtit projekt**.  
  Shembull: `<a href="faqe.html">Faqja kryesore</a>`

- **Linke të jashtme (External Links)** – lidhin faqe të tjera në internet.  
  Shembull: `<a href="https://example.com">Example</a>`

---

## 17. Dallimi mes imazhit dhe figurës në aspektin vizual

- **Image (`<img>`)** – shfaq vetëm **imazhin** në faqen web.  
- **Figure (`<figure>`)** – përfshin **imazhin + përshkrimin (caption)**, zakonisht me `<figcaption>`.  

> **Shembull:**
```html
<figure>
  <img src="foto.jpg" alt="Foto shembull">
  <figcaption>Kjo është përshkrimi i fotos</figcaption>
</figure>
```

## 18. Cilat tags përdoren për imazhe dhe për figura?

- **Për imazhe:** `<img>` – përdoret për të shfaqur vetëm imazhin.  

- **Për figura:** `<figure>` dhe `<figcaption>` – përdoren për të përfshirë **imazhin + përshkrimin e tij** (caption).  

> **Shembull:**
```html
<figure>
  <img src="foto.jpg" alt="Foto shembull">
  <figcaption>Kjo është përshkrimi i fotos</figcaption>
</figure>
```