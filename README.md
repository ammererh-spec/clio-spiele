# Clio Spiele

Spielseite für die Clio Suite: Lehrkräfte erstellen ein Spiel in der Suite und zeigen einen QR-Code; Schüler:innen spielen es im Handy-Browser – ohne App, ohne Anmeldung.

## Wie es funktioniert

Die Spieldaten stehen im Link hinter `#`:

```
https://ammererh-spec.github.io/clio-spiele/#z=<base64url(deflate-raw(JSON))>
JSON: {"v": 1, "typ": "zeitleiste", "titel": "…", "e": [["Ereignis", 1955], …]}
```

Der Teil hinter `#` wird vom Browser nie an einen Server geschickt. Die Seite speichert nichts, sammelt keine Daten und hat keine Verbindung zur Suite.

## Spieltypen

- `zeitleiste` – Ereignisse in die richtige Reihenfolge bringen (ziehen oder ▲▼), Jubel bei richtiger, traurige Posaune bei falscher Lösung.

Die Klänge werden im Browser erzeugt (Web Audio) – keine Audiodateien.
