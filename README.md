<p align="center">
  <img src="assets/banner.png" alt="Mathe Trainer" width="100%">
</p>

<p align="center">
  <a href="#-live"><img alt="Live" src="https://img.shields.io/badge/Live-GitHub%20Pages-1475e1?style=flat-square"></a>
  <img alt="Eine Datei" src="https://img.shields.io/badge/Eine%20Datei-560%20KB-14bf96?style=flat-square">
  <img alt="Ohne Abhängigkeiten" src="https://img.shields.io/badge/Abh%C3%A4ngigkeiten-keine-14bf96?style=flat-square">
  <img alt="Offline" src="https://img.shields.io/badge/offline-lauff%C3%A4hig-14bf96?style=flat-square">
  <img alt="Lizenz" src="https://img.shields.io/badge/Lizenz-MIT-a9bcd4?style=flat-square">
</p>

---

**Mathe Trainer** erzeugt unbegrenzt viele Übungsaufgaben — von Kopfrechnen bis zur Lagrange-Optimierung. Jede Aufgabe wird beim Aufrufen neu gewürfelt, die Antwort exakt geprüft und auf Wunsch Schritt für Schritt vorgerechnet. Zu den meisten Aufgaben gibt es einen Graphen zum Zoomen und Verschieben.

Das Ganze ist **eine einzige HTML-Datei**. Kein Server, kein Build-Schritt, kein Konto, keine Netzwerkanfragen — doppelklicken genügt, und auf dem Handy funktioniert es im Flugmodus genauso.

## 🚀 Live

👉 **[dein-name.github.io/mathe-trainer](https://dein-name.github.io/mathe-trainer)**

Oder [`mathe-trainer.html`](mathe-trainer.html) herunterladen und im Browser öffnen.

## 📸 Screenshots

| Dunkel | Hell |
|:--:|:--:|
| <img src="assets/shot-dark.png" alt="Extremstellen im Dunkelmodus"> | <img src="assets/shot-light.png" alt="Lagrange-Optimierung im Hellmodus"> |

<p align="center">
  <img src="assets/shot-contour.png" alt="Höhenlinien mit Budgetgerade und Optimum" width="88%"><br>
  <sub>Höhenlinien statt 3D-Gitter — läuft flüssig, auch auf dem iPad.</sub>
</p>

## ✨ Was drin steckt

- **28 Themen, 146 Aufgabentypen, 10 Schwierigkeitsstufen.** Die Stufe steuert nicht nur die Zahlen, sondern auch die Struktur: Auf Stufe 1 steht `x + 3 = 7`, auf Stufe 10 warten verschachtelte Wurzeln, e-Funktionen und Logarithmen.
- **Exakte Prüfung statt Zeichenvergleich.** Gerechnet wird mit Brüchen, nicht mit Fließkomma. `0,5`, `1/2` und `2/4` gelten alle. Terme werden an Stützstellen verglichen, deshalb zählt auch `2(x+1)` als Antwort auf `2x+2`.
- **Lösungsweg Schritt für Schritt** — erst auf Klick, damit er nichts verrät. Bei einer falschen Antwort gibt es weitere Versuche statt sofort die Lösung.
- **Graph zu 100 von 146 Aufgabentypen.** Funktionen, Lösungsbereiche, Höhenlinien mit Gradient und Nebenbedingung. Zoomen per Regler, Verschieben per Ziehen.
- **Formelsammlung** mit 119 Formeln aus allen Themen, plus einer Übersicht der Eingabe-Schreibweise.
- **Statistik**: Trefferquote je Thema, Verlaufskurve, aktuelle und beste Serie. Wird lokal im Browser gespeichert und ist beim nächsten Öffnen wieder da.
- **Übungsmodi**: freies Üben, Serien über 10 oder 20 Aufgaben, Zeitläufe über 2 oder 5 Minuten, sowie ein Zufallsmodus über ganze Themenbereiche.
- **Hell und dunkel.** Startet nach der Einstellung des Geräts, lässt sich mit einem Klick umschalten.

## 📚 Themen

| Bereich | Themen |
|---|---|
| **Grundlagen** | Kopfrechnen · Terme vereinfachen · Summen & Produkte · Definitionsmenge · Ökonomische Funktionen |
| **Gleichungen** | Lineare · Quadratische · Kubische · Bruch- · Betrags- · Potenz- · Wurzel- · Exponential- · Logarithmus-Gleichungen · Ungleichungen |
| **Analysis** | Grenzwerte · Ableitungen · Implizites Ableiten · Extremwerte · Integrale · Elastizitäten |
| **Mehrdim. Analysis** | Partielle Ableitungen · Gradient & Hesse · Extrema mit zwei Variablen · Lagrange-Optimierung |
| **Lineare Algebra** | Matrizen-Rechnung · Determinante & Inverse · Gauß-Verfahren |

## ⌨️ So tippst du ein

Kein LaTeX. Die Schreibweise orientiert sich daran, wie man Formeln ohnehin in eine Zeile schreibt:

| | Eingabe | Ergebnis |
|---|---|---|
| Mal & geteilt | `2*x` oder `2x` · `6/2` | 2·x · ³⁄₂ |
| Potenz | `x^2` · `x^(n+1)` | x² · xⁿ⁺¹ |
| Bruch | `1/x` · `(x+1)/(x-1)` | ¹⁄ₓ · (x+1)/(x−1) |
| Wurzel | `sqrt(x)` · `root(3, x)` | √x · ∛x |
| e-Funktion & ln | `e^(2x)` · `ln(x)` | e²ˣ · ln(x) |
| Betrag | `abs(x-3)` oder `\|x-3\|` | \|x−3\| |
| Konstanten | `pi` · `e` · `inf` | π · e · ∞ |
| Dezimalzahlen | `0.25` · `0,25` · `1/4` | 0,25 |

Komma und Punkt sind beide erlaubt — `f(2,5)` als Dezimalzahl und `root(3, x)` als Argumenttrenner werden auseinandergehalten.

**Tastenkürzel:** `Enter` prüfen bzw. nächste Aufgabe · `N` neue Aufgabe · `L` Lösungsweg · `Esc` Dialog schließen

## 📦 Auf GitHub Pages stellen

1. Neues Repository anlegen und `index.html` (die Kopie der Trainer-Datei) hochladen.
2. **Settings → Pages → Source: Deploy from a branch**, Branch `main`, Ordner `/ (root)`.
3. Nach ein bis zwei Minuten liegt die Seite unter `https://dein-name.github.io/repo-name/`.

Die Datei ist vollständig eigenständig — Schriften, Icons und Logo stecken als Data-URI mit drin, es gibt **null externe Anfragen**. Sie funktioniert deshalb genauso von einem USB-Stick, aus Moodle heraus oder offline.

## 🔧 Technik

- **Kein Framework.** Reines HTML, CSS und JavaScript. Was der Browser schon kann, wird nicht nachgebaut.
- **Exakte Arithmetik** über eine eigene Bruchklasse — dadurch keine Rundungsfehler wie `0.1 + 0.2 ≠ 0.3`.
- **Eigener Parser** (Tokenizer + rekursiver Abstieg) für die Eingaben, tolerant gegenüber fehlenden Malzeichen und Klammern.
- **Termvergleich per Stützstellen** statt symbolischer Umformung: Zwei Terme gelten als gleich, wenn sie auf einem Gitter übereinstimmen. Für Terme mit zwei Variablen wird über ein Flächengitter geprüft.
- **Höhenlinien** über Marching Squares, direkt auf ein `<canvas>` gezeichnet.
- **Speicherung** im `localStorage`; ist er gesperrt, läuft alles weiter, nur ohne Gedächtnis.

### Selbst bauen

Die Datei entsteht aus einzelnen Quelldateien, damit sie überhaupt wartbar bleibt:

```bash
npm install            # nur für die Schriften (Montserrat, Afacad)
python3 build.py       # baut mathe-trainer.html
```

`build.py` hängt die Skripte in `shell.html` ein und bettet die Schriften als Base64 ein.

### Tests

```bash
node test.js      # 43 800 erzeugte Aufgaben auf Konsistenz prüfen
node verify.js    # angezeigte Lösungswege in Terme zurückrechnen und vergleichen
node smoke.js     # Bedienung im echten Browser (Playwright)
```

## 📄 Lizenz

MIT — nutzen, ändern und weitergeben ausdrücklich erwünscht, gerne im Unterricht.
