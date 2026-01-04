╔══════════════════════════════════════════════════════════════════════════════╗
║                                                                              ║
║   ██████╗ ████████╗███╗   ███╗██╗                                             ║
║   ██╔══██╗╚══██╔══╝████╗ ████║██║                                             ║
║   ██████╔╝   ██║   ██╔████╔██║██║                                             ║
║   ██╔══██╗   ██║   ██║╚██╔╝██║██║                                             ║
║   ██║  ██║   ██║   ██║ ╚═╝ ██║███████╗                                        ║
║   ╚═╝  ╚═╝   ╚═╝   ╚═╝     ╚═╝╚══════╝                                        ║
║                                                                              ║
║                 HTML — PYETJE & PËRGJIGJE (BASICS)                            ║
║                                                                              ║
╚══════════════════════════════════════════════════════════════════════════════╝
  ╲                                                                            ╱
   ╲__________________________________________________________________________/ 
    ╲                                                                          ╱
     ╲________________________________________________________________________╱


┌──────────────────────────────────────────────────────────────────────────────┐
│ ABOUT                                                                         │
└──────────────────────────────────────────────────────────────────────────────┘
  Ky dokument përmbledh konceptet bazë të HTML (HyperText Markup Language).
  Shërben si material mësimor dhe referencë e shpejtë për zhvillimin web.


┌──────────────────────────────────────────────────────────────────────────────┐
│ CONTENTS                                                                      │
└──────────────────────────────────────────────────────────────────────────────┘
  01  Çka është HTML
  02  Llojet e tag-eve
  03  Struktura bazë e dokumentit
  04  Çka vendoset në head
  05  Çka vendoset në body
  06  Si renderohen elementet
  07  Block vs Inline
  08  Comments
  09  Etiketa të tekstit
  10  Etiketat semantike
  11  Semantike vs të zakonshme
  12  4 etiketa semantike
  13  Llojet e listave
  14  Tags e listave
  15  Linket dhe atributet
  16  Llojet e linkeve
  17  img vs figure
  18  Tags për imazhe dhe figura


╔══════════════════════════════════════════════════════════════════════════════╗
║  01  ÇKA ËSHTË HTML                                                          ║
╚══════════════════════════════════════════════════════════════════════════════╝
  HTML (HyperText Markup Language) është një gjuhë përshkruese për strukturimin
  e faqeve web.

  Nuk është gjuhë programimi.
  HTML i tregon browser-it si të organizohet dhe shfaqet përmbajtja.


╔══════════════════════════════════════════════════════════════════════════════╗
║  02  LLOJET E TAG-EVE                                                        ║
╚══════════════════════════════════════════════════════════════════════════════╝
  Dy kategori kryesore:

  A) Tags hapëse + mbyllëse
     Shembull:
     <p>Tekst</p>

  B) Tags vetë-mbyllëse
     Shembuj:
     <img />
     <br />
     <hr />


╔══════════════════════════════════════════════════════════════════════════════╗
║  03  STRUKTURA BAZË E DOKUMENTIT                                             ║
╚══════════════════════════════════════════════════════════════════════════════╝
  <!DOCTYPE html>
  <html>
    <head>
    </head>
    <body>
    </body>
  </html>


╔══════════════════════════════════════════════════════════════════════════════╗
║  04  ÇKA VENDOSET NË HEAD                                                    ║
╚══════════════════════════════════════════════════════════════════════════════╝
  Head përmban informacione që nuk shfaqen direkt në faqe, por janë të rëndësishme
  për funksionimin e saj.

  - Meta tags (charset, viewport, description)
  - Title i faqes
  - Lidhje me CSS (link)
  - Informacione për browser dhe SEO


╔══════════════════════════════════════════════════════════════════════════════╗
║  05  ÇKA VENDOSET NË BODY                                                    ║
╚══════════════════════════════════════════════════════════════════════════════╝
  Body përmban përmbajtjen e dukshme të faqes web.

  - Tekste (tituj, paragrafë)
  - Imazhe
  - Linke
  - Lista
  - Tabela
  - Forma


╔══════════════════════════════════════════════════════════════════════════════╗
║  06  SI RENDEROHEN ELEMENTET                                                 ║
╚══════════════════════════════════════════════════════════════════════════════╝
  Elementet HTML shfaqen zakonisht si:

  - Block elements
  - Inline elements


╔══════════════════════════════════════════════════════════════════════════════╗
║  07  BLOCK vs INLINE                                                         ║
╚══════════════════════════════════════════════════════════════════════════════╝
  Block elements
  - Zënë gjithë gjerësinë e rreshtit
  - Fillojnë në rresht të ri
  Shembuj: div, p, h1-h6

  Inline elements
  - Zënë vetëm hapësirën e përmbajtjes
  - Qëndrojnë në të njëjtin rresht
  Shembuj: span, a, strong, em


╔══════════════════════════════════════════════════════════════════════════════╗
║  08  COMMENTS                                                                ║
╚══════════════════════════════════════════════════════════════════════════════╝
  Comments përdoren për shpjegim dhe dokumentim të kodit.
  Browser-i nuk i shfaq.

  Shembull:
  <!-- Ky është një comment -->


╔══════════════════════════════════════════════════════════════════════════════╗
║  09  ETIKETA TË TEKSTIT                                                      ║
╚══════════════════════════════════════════════════════════════════════════════╝
  - Bold: b, strong
  - Italic: i, em
  - Underline: u
  - Sub/Sup: sub, sup
  - Tituj: h1 deri h6


╔══════════════════════════════════════════════════════════════════════════════╗
║  10  ETIKETAT SEMANTIKE                                                      ║
╚══════════════════════════════════════════════════════════════════════════════╝
  Etiketat semantike tregojnë rolin e përmbajtjes në faqe.
  Ndihmojnë SEO dhe accessibility.

  Shembuj:
  header, nav, main, section, article, footer


╔══════════════════════════════════════════════════════════════════════════════╗
║  11  SEMANTIKE vs TË ZAKONSHME                                               ║
╚══════════════════════════════════════════════════════════════════════════════╝
  - div (tag i zakonshëm): nuk tregon kuptim/rol
  - header/nav/main/footer (semantike): tregojnë qartë rolin e përmbajtjes


╔══════════════════════════════════════════════════════════════════════════════╗
║  12  4 ETIKETA SEMANTIKE                                                     ║
╚══════════════════════════════════════════════════════════════════════════════╝
  header
  nav
  main
  footer


╔══════════════════════════════════════════════════════════════════════════════╗
║  13  LLOJET E LISTAVE                                                        ║
╚══════════════════════════════════════════════════════════════════════════════╝
  - Ordered list
  - Unordered list
  - Description list


╔══════════════════════════════════════════════════════════════════════════════╗
║  14  TAGS E LISTAVE                                                          ║
╚══════════════════════════════════════════════════════════════════════════════╝
  Ordered list:     ol + li
  Unordered list:   ul + li
  Description list: dl + dt + dd


╔══════════════════════════════════════════════════════════════════════════════╗
║  15  LINKET (a) DHE ATRIBUTET                                                ║
╚══════════════════════════════════════════════════════════════════════════════╝
  Tagu: a

  Atributet kryesore:
  - href   (adresa)
  - target (ku hapet)
  - title  (përshkrim)

  Shembull:
  <a href="https://example.com" target="_blank" title="Example">Example</a>


╔══════════════════════════════════════════════════════════════════════════════╗
║  16  LLOJET E LINKEVE                                                        ║
╚══════════════════════════════════════════════════════════════════════════════╝
  - Linke të brendshme (brenda projektit)
  - Linke të jashtme (në internet)


╔══════════════════════════════════════════════════════════════════════════════╗
║  17  IMG vs FIGURE                                                           ║
╚══════════════════════════════════════════════════════════════════════════════╝
  img    — shfaq vetëm imazhin
  figure — shfaq imazhin + përshkrimin (figcaption)


╔══════════════════════════════════════════════════════════════════════════════╗
║  18  TAGS PËR IMAZHE DHE FIGURA                                              ║
╚══════════════════════════════════════════════════════════════════════════════╝
  Për imazhe: img
  Për figura: figure + figcaption

  Shembull:
  <figure>
    <img src="foto.jpg" alt="Foto">
    <figcaption>Përshkrimi i fotos</figcaption>
  </figure>


┌──────────────────────────────────────────────────────────────────────────────┐
│ END                                                                          │
└──────────────────────────────────────────────────────────────────────────────┘
