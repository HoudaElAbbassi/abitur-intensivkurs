# abitur-intensivkurs

Webseite und Anmeldeformular für den Mathematik Abitur Intensivkurs 2025.

## Dateien

```
abitur-intensivkurs/
├── index.html       # Landingpage: Hero, Kurse, Preise, Ablauf, FAQ
├── anmeldung.html   # Anmeldeformular mit Live-Validierung
└── README.md
```

## Kurse & Preise

| Paket | Termin | Preis |
|-------|--------|-------|
| Leistungskurs | 1.–3. April 2025, 10:00–13:30 | 99 € |
| Grundkurs | 8.–10. April 2025, 10:00–13:30 | 99 € |
| Kombi (LK + GK) | Beide Termine | 179 € |

## GitHub Pages einrichten

1. Repo auf GitHub erstellen: `abitur-intensivkurs`
2. Alle Dateien pushen oder hochladen
3. **Settings → Pages → Branch: `main` → Folder: `/root` → Save**
4. Seite läuft unter: `https://DEIN-USERNAME.github.io/abitur-intensivkurs/`

## Kontaktdaten anpassen

In beiden HTML-Dateien suchen & ersetzen:
- `info@meinschulzentrum.de` → deine E-Mail
- `0123 · 456 789 0` → deine Telefonnummer
- `MeinSchulzentrum` → dein Schulname

## Formular-Backend (E-Mail-Versand)

Das Formular zeigt aktuell eine Erfolgsseite ohne echten Versand.
Für echten E-Mail-Empfang **Formspree** einbinden (kostenlos):

1. Konto auf [formspree.io](https://formspree.io) erstellen
2. Formular anlegen → Endpoint kopieren
3. In `anmeldung.html` das `<form>`-Tag ändern:

```html
<form action="https://formspree.io/f/DEIN-CODE" method="POST">
```

## Tech-Stack

- Reines HTML / CSS / JavaScript — keine Dependencies
- Google Fonts: Syne + Instrument Sans
- Vollständig responsiv (Mobile-optimiert)
- GitHub Pages kompatibel (statisch)
