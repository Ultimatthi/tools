# tools

Kleine Browser-Tools und Experimente. Jedes Tool liegt in einem eigenen Ordner und läuft direkt im Browser, ohne Build-Schritt.

| Tool | Beschreibung |
| --- | --- |
| [Stockfish Hand und Brain](stockfish-hand-und-brain/) | Hand-und-Brain-Schach mit Stockfish als „Brain“: Die Engine sagt die Figur an, du ziehst sie am echten Brett. Mit den Varianten Klassisch, Atomic und Dreischach. |
| [Palabras](palabras/) | Spanisch-Vokabeltrainer. |

## Lokal starten

Die Tools laden Dateien nach (z. B. die Stockfish-Engine als Web Worker), darum über einen lokalen Webserver öffnen statt per Doppelklick:

```sh
python3 -m http.server
```

Dann `http://localhost:8000/` im Browser öffnen.

## Hinweise

- **Stockfish Hand und Brain** enthält Stockfish 19 (über [stockfish.js](https://github.com/nmrugg/stockfish.js)) und den Multi-Variant-Stockfish (über [niklasf/stockfish.js](https://github.com/niklasf/stockfish.js)), beide unter GPLv3, siehe `Stockfish-GPL-Copying.txt`. Regeln: chessops.
- **Palabras**: Die Audiodatei `audio.js` aus dem ursprünglichen Artefakt fehlt hier, weil sie zu groß zum Übertragen war. Ohne sie liest der Browser die Wörter mit seiner eingebauten Sprachausgabe vor.
