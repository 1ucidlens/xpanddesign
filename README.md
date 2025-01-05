# xpand Website Style Guide

Dieser Style Guide beschreibt alle zentralen Gestaltungsrichtlinien für die xpand-Webseiten. Er enthält Farbvorgaben, Typografie-Empfehlungen, Icon- und Logoverwendung sowie Hinweise zur Anwendung der Gestaltungselemente (z.B. Buttons, Tabs, Akkordeons). Dieses Dokument soll Webentwickler*innen und Designer*innen als verbindliche Grundlage für ein konsistentes Erscheinungsbild dienen.

---

## 1. Logos

### xpand Logos

#### Dateien:
- **Primärlogo (blauer Hintergrund, #1d2362))**: `xpand-auf-blau.svg`
- **Primärlogo (weißer Hintergrund)**: `xpand-auf-weiss.svg`

---

### xpandAI Logos (zusätzlich zum xpand-Logo bei Einsatz von KI)

#### Dateien:
- **xpandAI (blauer Hintergrund)**: `xpandai-auf-blau.svg`
- **xpandAI (weißer Hintergrund)**: `xpandai-auf-weiss.svg`

---

### Logogröße & Schutzzone
- Um die Logos herum ist eine Mindestrandzone (auch „Clearspace“ genannt) einzuhalten.  
- Richtwert: Der Abstand zu angrenzenden Elementen sollte mindestens die Höhe des roten „x“ betragen.

---

## 2. Farben

### Primäre Farben
| Farbe        | RGB        | CMYK          | HEX      | Pantone   |
|--------------|------------|---------------|----------|-----------|
| **Navy**     | 14, 23, 86 | 100, 90, 0, 40| `#1d2362`| 280 C     |
| **Rot**      | 203, 0, 26 | 0, 100, 100, 10 | `#d10a10`| 186 C     |
| **Weiß**     | 255, 255, 255 | 0, 0, 0, 0 | `#ffffff`| –         |

### Sekundärfarben (abgeleitete Töne)
- Navy-Hellstufen: RGB: (40er, 60er, 80er Abstufungen), z.B. `#3b4379` oder in CSS als `rgba(29,35,98,0.2–0.8)`  
- Rot-Hellstufen: z.B. `#f5c1c1` (leichte Abstufung durch Transparenz oder hellere Töne)  

---

## 3. Typografie

### 3.1 Hauptschrift Poppins
- **Gewichte**: ExtraLight, Light, Regular, Medium, Bold (jeweils + Italic)  
- **Einsatzbereiche**: Lauftexte, Fließtexte, Detailtexte, kleinere Zwischenüberschriften.

Empfohlene CSS-Varianten:
```css
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;500;700&display=swap');

body {
  font-family: 'Poppins', sans-serif;
}
```

### 3.2 Überschriften Red Hat Display
- **Gewichte**: Light, Regular, Medium, SemiBold, Bold (jeweils + Italic)  
- **Einsatzbereiche**: Große Headlines, Subheadlines, auffällige Zwischenüberschriften.

Beispiel:
```css
@import url('https://fonts.googleapis.com/css2?family=Red+Hat+Display:wght@300;400;500;600;700&display=swap');

h1, h2, h3, h4 {
  font-family: 'Red Hat Display', sans-serif;
}
```

---

## 4. Icons

Icons folgen einem reduzierten Flat-Design-Stil:
- **Farben**: Navy (#1d2362) auf hellem Hintergrund, invertiert (weiß auf navy-blauem Hintergrund).  
- **Formen**: Geometrische Einfachheit (z.B. Parallelogramme, Kreise, Plus-/Minuszeichen).

---

## 5. Buttons

### 5.1 Primärbutton (Call to Action)
- **Farbe**: Rot (#d10a10) mit weißer Schrift (#ffffff).
- **Hover-Effekt**: Dunkleres Rot (#b0090e).  

Beispiel-CSS:
```css
.btn-primary {
  background-color: #d10a10;
  color: #ffffff;
  border: none;
  border-radius: 24px;
  padding: 12px 24px;
  font-family: 'Poppins', sans-serif;
  cursor: pointer;
  transition: background-color 0.2s ease-in-out;
}
.btn-primary:hover {
  background-color: #b0090e; /* dunkleres Rot */
}
```

---

## 6. Tabs & Akkordeons

### Tabs
- **Aktive Tabs**: Navy-Hintergrund mit weißer Schrift.  
- **Design**: Abgerundete Ecken.

### Akkordeons
- **Expand-/Collapse-Icons**: Pfeil-Symbole, die den Status (aufgeklappt/geschlossen) anzeigen.

---

## 7. Layout-Empfehlungen

- **Weißraum**: Ausreichender Abstand zwischen Elementen, um eine klare visuelle Struktur zu gewährleisten.  
- **Responsive Design**: Nutzung eines 12-Spalten-Grids (z.B. mit CSS-Grid).  

---

## 8. Bildsprache

- **Themen**: Natur, Dynamik, abstrakte Visualisierungen.
- **Farbharmonie**: Fotos sollten mit Markenfarben (Navy/Rot) harmonieren.

---

Dieser Style Guide hilft, das Design konsistent umzusetzen, und bietet klare Richtlinien für alle visuellen und funktionalen Aspekte der xpand-Website.
