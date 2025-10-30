# Was ist das?

Diese Datei ist eine HTML-Vorlage (Seitenskelett) für eine deutschsprachige Informations-/Landing‑Seite, aufgebaut mit Bootstrap. Kurz zusammengefasst:

- Zweck: Grundlage/Template für eine Website‑Seite namens "Seitenskelett" — zeigt Inhaltblöcke (Cards) zu Themen wie Schreiben, Vorbereitung/Planung, Bilder und Basteln. Zwei der Cards (Bilder, Basteln) werden zur Laufzeit per JavaScript generiert.
- Layout und Technik:
  - Bootstrap für Grid, Navbar und Komponenten; responsive <picture>-Elemente für adaptive Bildquellen.
  - Fixed-top Navbar mit Navigation zu anderen Seiten (Home, Ideen, Planung, u. a.).
  - Hauptbereich (main) mit mehreren Reihen (row-0, row-1, row-2) und Cards in zwei Spalten.
  - Footer mit Services und Kontaktinformationen.
- Interaktivität:
  - JavaScript-Funktionen zum Ein-/Ausblenden von Abschnitten: toggleExample und toggleHiddenSections.
  - Ein Script erzeugt dynamisch zwei Cards aus dem cardsData‑Array (mit Bildquellen, Titeln, Bullet‑Listen und optionalen "Mehr anzeigen"‑Sektionen).
  - DOM-Helferfunktionen createEl, cardList, renderCard für sauberes Erzeugen der Elemente.
- Inhalt/Platzhalter:
  - Viele Bilder, Texte und Medien sind Platzhalter (via.placeholder.com) oder gekennzeichnet (z. B. "Foto: N.N.", "Bild: inhouse").
  - Meta‑ und Title‑Tags sind gesetzt; locale ist Deutsch (lang="de").
- Stil:
  - Zusätzliche inline-CSS-Regeln zur Anpassung von Abständen, versteckten Sektionen, Thumbnails und Buttons (.mehr-button, .example-container etc.).
- Barrierefreiheit/Performance:
  - alt‑Attribute bei Bildern, aria-current auf aktivem Link, lazy loading/decoding-Attribute für das Logo (teilweise genutzt).
  - Externe Scripts (jQuery slim, Bootstrap Bundle) werden am Ende eingebunden.

**Kurz:** skeleton.html ist ein responsive Seiten-Template mit Bootstrap, das statische und dynamisch erzeugte Inhaltskarten sowie einfache UI‑Interaktionen (Mehr‑/Weniger‑Anzeigen) bereitstellt — ideal als Ausgangspunkt für eine Inhaltsseite mit Platzhaltern und einem kleinen Component-System in plain JavaScript.
