<p align="center">
  <img src="assets/banner.png" alt="Mathe Trainer" width="100%">
</p>

Ein mathematischer Übungsgenerator, der das gesamte Spektrum abdeckt: von einfachem Kopfrechnen bis zur Lagrange Optimierung. Jede Aufgabe entsteht beim Aufrufen neu, wird exakt berechnet und lässt sich auf Wunsch Schritt für Schritt nachvollziehen. Die gesamte Anwendung steckt in einer einzigen HTML Datei - ganz ohne Server, ohne Vorbereitung beim Erstellen und ohne Netzwerkanfragen. Einfach im Browser öffnen und direkt nutzen, selbst ohne Internetverbindung.

→ **Live ausprobieren:** nichtn1ce.github.io/Mathe-Trainer/

---

## Screenshots

| Aufgabe mit Graph | Stochastik im Hellmodus |
|:--:|:--:|
| <img src="assets/screenshot-dark.png" alt="Extremstellen einer Funktion"> | <img src="assets/screenshot-light.png" alt="Bedingte Wahrscheinlichkeit mit Vierfeldertafel"> |

<img src="assets/loesungsweg.png" alt="Lösungsweg Schritt für Schritt">

<img src="assets/hoehenlinien.png" alt="Höhenlinien mit Budgetgerade und Optimum">

## Themen

| Bereich | Themen |
|---|---|
| Grundlagen | Kopfrechnen · Terme vereinfachen · Summen & Produkte · Definitionsmenge · Ökonomische Funktionen |
| Gleichungen | Lineare · Quadratische · Kubische · Bruch- · Betrags- · Potenz- · Wurzel- · Exponential- · Logarithmusgleichungen · Ungleichungen |
| Analysis | Grenzwerte · Folgen & Reihen · Ableitungen · Implizites Ableiten · Extremwerte · Integrale · Elastizitäten |
| Mehrdim. Analysis | Partielle Ableitungen · Gradient & Hesse · Extrema mit zwei Variablen · Lagrange-Optimierung |
| Lineare Algebra | Matrizen · Determinante & Inverse · Gauß-Verfahren · Vektorrechnung |
| Stochastik | Wahrscheinlichkeit · Kombinatorik |

## Veröffentlichen

```
Repository/
├── index.html          ← die Trainer-Datei
├── README.md
└── assets/             ← Bilder für dieses README
```

`Settings → Pages → Source: Deploy from a branch`, Branch `main`, Ordner `/ (root)`. Nach wenigen Minuten ist die Seite unter `https://DEIN-NAME.github.io/repository/` erreichbar.

Die Datei ist vollständig eigenständig — Schriften, Icons und Logo stecken als Data-URI darin, es gibt keine externen Anfragen. Sie funktioniert deshalb auch von einem USB-Stick, in einem Lernmanagementsystem oder offline.

## Entwicklung

Die ausgelieferte Datei wird aus einzelnen Quelldateien zusammengebaut:

```bash
npm install          # nur die Schriften (Montserrat, Afacad)
python3 build.py     # erzeugt mathe-trainer.html
```

Tests:

```bash
node test.js     # 54.300 erzeugte Aufgaben auf Konsistenz
node guard.js    # Lösungen rational und mit der eigenen Prüfung verträglich
node verify.js   # angezeigte Lösungswege zurückrechnen und vergleichen
node dup.js      # Vorrat je Aufgabentyp und Stufe messen
node smoke.js    # Bedienung im Browser (Playwright)
```

## Technik

Reines HTML, CSS und JavaScript ohne Framework. Exakte Bruchrechnung über eine eigene Klasse, ein eigener Parser (Tokenizer und rekursiver Abstieg) für die Eingaben, Termvergleich über Stützstellen statt symbolischer Umformung, Höhenlinien über Marching Squares auf `<canvas>`.
