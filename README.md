# Cuba Flag 🇨🇺

Eine HTML/CSS-Implementierung der kubanischen Flagge mit interaktivem Design.

## Beschreibung

Dieses Projekt rendert die Flagge Kubas mit seinen charakteristischen Designelementen:
- **5 horizontale Streifen**: Blau (oben und unten) und Weiß (dazwischen)
- **Rotes Dreieck**: Auf der linken Seite, symbolisiert Blut und Opfer
- **Weißer Stern**: Zentriert im roten Dreieck, steht für Freiheit

Die Flagge ist vollständig mit HTML und CSS erstellt und verwendet moderne CSS-Techniken wie `clip-path` für die geometrischen Formen.

## Dateien

- **index.html** - Die HTML-Struktur der Flagge
- **style.css** - Vollständige Styling- und Layoutdefinitionen

## Features

✨ **Responsive Design** - Viewport-Einstellungen für mobile Geräte  
🎨 **CSS-Geometrie** - Verwendung von `clip-path` für Stern und Dreieck  
📍 **Zentriert** - Die Flagge wird automatisch in der Bildschirmmitte positioniert  
💄 **Sauberer Code** - Gut strukturiert mit aussagekräftigen Kommentaren

## Struktur

### HTML-Struktur
```
flagge (900x600px)
├── eins (blauer Streifen)
│   └── text ("Cuba")
├── zwei (weißer Streifen)
├── drei (blauer Streifen)
├── vier (weißer Streifen)
└── funf (blauer Streifen)

dreieck (rotes Dreieck)
└── stern (weißer Stern)
```

### CSS-Highlights

**Stern im Dreieck zentrieren:**
```css
.stern {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    clip-path: polygon(...); /* 10-zackiger Stern */
}
```

**Dreieck formen:**
```css
.dreieck {
    clip-path: polygon(100% 50%, 0 0, 0 100%);
}
```

## Verwendung

1. Dateien herunterladen oder klonen
2. `index.html` im Browser öffnen
3. Die kubanische Flagge wird zentriert angezeigt

## Anpassungen

- **Größe**: Ändern Sie `width` und `height` in `.flagge`
- **Sternform**: Modifizieren Sie die `clip-path` Polygon-Koordinaten in `.stern`
- **Farben**: Nutzen Sie CSS `background-color` Eigenschaften

## Browser-Kompatibilität

- ✅ Chrome/Edge 88+
- ✅ Firefox 87+
- ✅ Safari 14+
- ✅ Modern browsers mit CSS `clip-path` Unterstützung

## Lizenz

Dieses Projekt ist frei verwendbar für Lern- und Entwicklungszwecke.

---

Made with ❤️ for flag design enthusiasts
