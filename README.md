# Einfache Überraschungs-Weiterleitung

Öffne `index.html` im Browser. Die Seite leitet nach wenigen Sekunden automatisch weiter (oder sofort nach Klick auf den Knopf). Die Ziel-URL ist in der Datei base64-kodiert, sodass sie nicht direkt angezeigt wird.

Schnelltest (im Projektordner) mit einem lokalen Server:

```bash
python -m http.server 8000
# Dann im Browser öffnen: http://localhost:8000/index.html
```

Wenn du die Zielseite ändern willst, ersetze die Base64-Zeichenkette in `index.html` (Konstante `encoded`) durch `btoa('dein-ziel.html')` oder verwende einen Online-Base64-Encoder.
