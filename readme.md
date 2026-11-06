# bwinfN: Python für die 3. Runde des Jugendwettbewerbs Informatik

Dieses Repository enthält einen **Lehrgang**, der von Blockly zu Python führt, und **Lösungsnotebooks** zu allen
Junioraufgaben der Jahre 2011 bis 2025. Der Lehrgang richtet sich an alle, die im Jugendwettbewerb Informatik schon mit
Blockly programmiert haben und nun die Aufgaben der 3. Runde (zugleich die Junioraufgaben der 1. Runde des Bundeswettbewerbs
Informatik) in Python lösen möchten. Er beginnt ganz von vorn und ist ab etwa Klasse 7 geeignet.

Alle Notebooks laufen direkt im Browser mit [JupyterLite](https://jupyterlite.readthedocs.io/), ohne Installation und ohne
Anmeldung. Ein Klick auf einen Link öffnet das Notebook.

**So arbeitest du mit den Notebooks**

- Eine Codezelle führst du mit **Umschalt + Enter** aus.
- Unter jeder Aufgabe kannst du zuerst einen **Tipp** und dann die **Lösung** aufklappen. Versuche es immer erst selbst.
- Deine Änderungen speichert der Browser. In einem anderen Browser oder auf einem anderen Gerät siehst du wieder die
  ursprüngliche Fassung.
- Welcher Blockly-Block in Python wie heißt, steht in der [Übersetzungstabelle Blockly → Python](https://github.com/ktheu/bwinfN/blob/main/content/learn_jwinf3/blockly_python.md).

## Der Lehrgang

Die Notebooks bauen aufeinander auf. Jedes ist für etwa eine Unterrichtsstunde gedacht und endet mit einer
**Wettbewerbs-Ecke**: einer verkleinerten Fassung einer echten Junioraufgabe, die genau die neue Fähigkeit braucht.

### Phase A: Python-Grundlagen aus Blockly heraus

Hier lernst du die Python-Grundlagen. Zu jedem neuen Befehl steht der passende Blockly-Block dabei: Variablen,
Entscheidungen, Schleifen, Texte, Listen, Funktionen und Dateien. Nach Phase A kannst du schon einfache Wettbewerbsaufgaben
vollständig lösen.

> **Wer schon Übung mit Python hat**, kann diesen Abschnitt überspringen und gleich mit Notebook 23 (Aufgaben lesen) und
> Phase B beginnen.

| Nr | Notebook | Inhalt | Wettbewerbs-Ecke |
|---|---|---|---|
| 01 | [Erste Schritte mit Python](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/01_erste_schritte.ipynb) | `print`, Rechnen mit `//` und `%`, Variablen, Fehlermeldungen lesen | Wundertüten gleichmäßig packen |
| 02 | [Entscheidungen mit if](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/02_entscheidungen.ipynb) | `if`/`elif`/`else`, Vergleiche, `and`/`or`/`not`, Einrückung | Bällebad, ein Zug im Leiterspiel |
| 03 | [Wiederholen mit for](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/03_wiederholen_for.ipynb) | `for` und `range`, Summen und Zähler, `if` in Schleifen | Wundertüten reihum packen |
| 04 | [Wiederholen mit while](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/04_wiederholen_while.ipynb) | `while`, Ziffern abtrennen, Endlosschleifen, `break` | Leiterspiel bis ins Ziel |
| 05 | [Texte](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/05_texte.ipynb) | Texte: Positionen ab 0, Ausschnitte, Zeichen prüfen, `ord`/`chr` | Texthopsen |
| 06 | [Listen](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/06_listen.ipynb) | Listen: anhängen, Summe und Maximum, zwei Listen, `split`/`join` | Bällebad, Wundertüte |
| 07 | [Funktionen](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/07_funktionen.ipynb) | Funktionen: `def`, Parameter, `return`, Testaufrufe | Leiterspiel mit Funktionen |
| 08 | [Dateien lesen und Ergebnisse schreiben](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/08_dateien.ipynb) | Dateien lesen und schreiben, Ausgabe mit f-Strings | Bällebad und Wundertüte komplett |

Gleich nach Phase A lohnt sich **Notebook 23 (Aufgaben lesen und Unklarheiten finden)** aus Phase D.

### Phase B: Werkzeuge für die 3. Runde

Typische Werkzeuge, die in vielen Aufgaben vorkommen: Suchen und Zählen, alle Möglichkeiten durchprobieren, Tabellen und
Raster, Simulationen, Testen, Wörterbücher und Mengen, Zufall. Phase B ist der Kern des Lehrgangs.

| Nr | Notebook | Inhalt | Wettbewerbs-Ecke |
|---|---|---|---|
| 09 | [Zählen, Suchen, das Beste merken](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/09_zaehlen_suchen.ipynb) | Suchen, Zählen, das Beste merken, Gleichstand | Treffsicherheit, Zum Winde verweht |
| 10 | [Schleifen ineinander: alle Möglichkeiten](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/10_alle_moeglichkeiten.ipynb) | Schleifen ineinander, alle Paare, Laufzeit abschätzen | Quadratisch praktisch grün, Reimerei, Zahlenspiel |
| 11 | [Tabellen und Rechnen im Kreis](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/11_tabellen_kreis.ipynb) | Tabellen (Listen von Listen), Rechnen im Kreis, Koordinaten | Bällebad-Plan, Baywatch, St. Egano |
| 12 | [Raster und Karten](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/12_raster.ipynb) | Raster einlesen, Nachbarn mit Randprüfung, Muster suchen | Kassiopeia, Minensuche, Baulwürfe |
| 13 | [Simulation](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/13_simulation.ipynb) | Simulation: Zustand, Schritt, Schleife, „schon gesehen“ | Leiterspiel, Wintervorrat, Lights Out |
| 14 | [Regeln, Prüfen, Testen](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/14_regeln_testen.ipynb) | Regeln nacheinander, Testtabellen, Sonderfälle, Bewertung | Verben, Bällebad-Sonderfälle, Silbentrennung |
| 15 | [Wörterbücher und Mengen](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/15_woerterbuecher_mengen.ipynb) | Wörterbücher und Mengen: nachschlagen, zählen, gruppieren | Auf und Ab, Container |
| 16 | [Zufall](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/16_zufall.ipynb) | Zufall: erzeugen nach Regeln, erzeugen und prüfen, viele Versuche | Passwörter, Songwriter |

### Phase C: Vertiefung

Für Fortgeschrittene (etwa ab Klasse 9) oder für Schnelle: Geometrie, Strategien vergleichen, Zeichnen und Bilder. Die
Notebooks 21 (Erreichbarkeit) und 22 (Rekursion) sind freiwillig, sie werden nur für wenige, eher ältere Aufgaben gebraucht.

| Nr | Notebook | Inhalt | Wettbewerbs-Ecke |
|---|---|---|---|
| 17 | [Geometrie mit Koordinaten](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/17_geometrie.ipynb) | Abstände, Rechtecke, links/rechts einer Geraden, Winkel | Landnahme, Skyline |
| 18 | [Strategien vergleichen](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/18_strategien.ipynb) | Sortieren, gierige Strategien, Strategien vergleichen | Fähre füllen, Bücherregal |
| 19 | [Zeichnen zur Kontrolle](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/19_zeichnen.ipynb) | Zeichnen mit matplotlib: Punkte, Rechtecke, Farbbilder | Landnahme, Wintervorrat |
| 20 | [Bilder als Daten](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/20_bilder.ipynb) | Bilder als Daten: Pixel, RGB, Pillow, PPM | St. Egano mit den echten Bildern |
| 21 | [Erreichbarkeit (freiwillig)](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/21_erreichbarkeit.ipynb) | Erreichbarkeit mit Flood Fill, Gruppen zählen (freiwillig) | Kassiopeia, Container |
| 22 | [Rekursion (freiwillig)](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/22_rekursion.ipynb) | Rekursion, alle Möglichkeiten, Zwischenergebnisse merken (freiwillig) | Glücksrad, Rechteckschoner, Luftballons |

### Phase D: Wettbewerbstraining

Hier geht es um den Wettbewerb selbst: Aufgaben genau lesen und Unklarheiten erkennen, eine Aufgabe vollständig bearbeiten
und die Dokumentation schreiben, auf die es bei der Bewertung vor allem ankommt.

| Nr | Notebook | Inhalt | Wettbewerbs-Ecke |
|---|---|---|---|
| 23 | [Aufgaben lesen und Unklarheiten finden](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/23_aufgaben_lesen.ipynb) | Aufgaben lesen, Unklarheiten finden, Lesarten festlegen | Bällebad, Texthopsen, Parallelen, Quadratisch praktisch grün |
| 24 | [Eine Aufgabe von A bis Z](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/24_a_bis_z.ipynb) | eine ganze Aufgabe von A bis Z: lesen, Idee, Funktionen, Beispiele, Sonderfälle | Texthopsen |
| 25 | [Die Dokumentation](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/25_dokumentation.ipynb) | die Dokumentation: Lösungsidee, Umsetzung, Beispiele, Quellcode, Bewertung | Musterdokumentation zu Texthopsen |

Zum Weiterüben: Die **[Aufgabenliste](https://github.com/ktheu/bwinfN/blob/main/content/learn_jwinf3/aufgabenliste.md)** beschreibt alle Junioraufgaben von 2011 bis 2025
mit den nötigen Werkzeugen, der typischen Stolperstelle und einer Einschätzung der Schwierigkeit, und schlägt eine
Reihenfolge vor.

## Die Lösungsnotebooks

Zu jeder Junioraufgabe der Jahre 2011 bis 2025 gibt es ein Lösungsnotebook. Es enthält den Aufgabentext, die nützlichen
Werkzeuge, die Lösungsidee und eine Schritt-für-Schritt-Lösung mit allen Beispielen. Zuerst kommt immer die einfachste
Lösung, schnellere Verfahren stehen am Ende unter „Für Neugierige“. **Bearbeite eine Aufgabe zuerst selbst** und sieh dir das
Lösungsnotebook erst danach an. Die Sterne geben eine grobe Einschätzung der Schwierigkeit (★ leicht bis ★★★★ schwer, Erklärung
in der Aufgabenliste).

Die Aufgaben des laufenden Wettbewerbs sind absichtlich nicht dabei.

| Jahr | Aufgabe | Schwierigkeit | Lösungsnotebook |
|---|---|---|---|
| 2025 | Bällebad | ★★ | [baellebad_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/44_Baellebad/baellebad_loesung.ipynb) |
| 2025 | Silbentrennung | ★★★ | [silbentrennung_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/44_Silbentrennung/silbentrennung_loesung.ipynb) |
| 2024 | Quadratisch, praktisch, grün | ★★★ | [quadratisch_praktisch_gruen_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/43_QuadratischPraktischGr%C3%BCn/quadratisch_praktisch_gruen_loesung.ipynb) |
| 2024 | Texthopsen | ★★ | [texthopsen_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/43_Texthopsen/texthopsen_loesung.ipynb) |
| 2023 | St. Egano | ★★ | [stegano_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/42_StEgano/stegano_loesung.ipynb) |
| 2023 | Wundertüte | ★★ | [wundertuete_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/42_Wundertuete/wundertuete_loesung.ipynb) |
| 2022 | Container | ★★ | [container_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/41_Container/container_loesung.ipynb) |
| 2022 | Reimerei | ★★★ | [reimerei_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/41_Reimerei/reimerei_loesung.ipynb) |
| 2021 | Treffsicherheit | ★★★ | [treffsicherheit_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/40_Treffsicherheit/treffsicherheit_loesung.ipynb) |
| 2021 | Zum Winde verweht | ★★ | [zumwindeverweht_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/40_ZumWindeVerweht/zumwindeverweht_loesung.ipynb) |
| 2020 | Baulwürfe | ★★★ | [baulwuerfe_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/39_Baulwuerfe/baulwuerfe_loesung.ipynb) |
| 2020 | Passwörter | ★ | [passwoerter_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/39_Passwoerter/passwoerter_loesung.ipynb) |
| 2019 | Kacheln | ★★★★ | [kacheln_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/38_Kacheln/kacheln_loesung.ipynb) |
| 2019 | Parallelen | ★★ | [parallelen_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/38_Parallelen/parallelen_loesung.ipynb) |
| 2018 | Auf und Ab | ★★ | [aufundab_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/37_AufUndAb/aufundab_loesung.ipynb) |
| 2018 | Baywatch | ★★ | [baywatch_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/37_Baywatch/baywatch_loesung.ipynb) |
| 2017 | Bücherregal | ★★ | [buecherregal_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/36_Buecherregal/buecherregal_loesung.ipynb) |
| 2017 | Wintervorrat | ★★★ | [wintervorrat_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/36_Wintervorrat/wintervorrat_loesung.ipynb) |
| 2016 | LAMA | ★★ | [lama_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/35_LAMA/lama_loesung.ipynb) |
| 2016 | Luftballons | ★★★★ | [luftballons_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/35_Luftballons/luftballons_loesung.ipynb) |
| 2015 | Kassiopeia | ★★★ | [kassiopeia_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/34_Kassiopeia/kassiopeia_loesung.ipynb) |
| 2015 | Landnahme | ★★ | [landnahme_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/34_Landnahme/landnahme_loesung.ipynb) |
| 2014 | Fähre füllen | ★★★ | [faehrefuellen_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/33_FaehreFuellen/faehrefuellen_loesung.ipynb) |
| 2014 | Zahlenspiel | ★★ | [zahlenspiel_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/33_Zahlenspiel/zahlenspiel_loesung.ipynb) |
| 2013 | Songwriter | ★★ | [songwriter_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/32_Songwriter/songwriter_loesung.ipynb) |
| 2013 | Zollstock | ★★★ | [zollstock_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/32_Zollstock/zollstock_loesung.ipynb) |
| 2012 | Skyline | ★★ | [skyline_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/31_Skyline/skyline_loesung.ipynb) |
| 2012 | Verben | ★★★ | [verben_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/31_Verben/verben_loesung.ipynb) |
| 2011 | Glücksrad | ★★★★ | [gluecksrad_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/30_Gluecksrad/gluecksrad_loesung.ipynb) |
| 2011 | Rechteckschoner | ★★★ | [rechteckschoner_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/30_Rechteckschoner/rechteckschoner_loesung.ipynb) |

## Für Lehrkräfte

- Die Notebooks entstehen im Repository bwinfCC und werden mit einem Skript in den Ordner `content/` exportiert. Änderungen
  am besten dort vornehmen.
- Die JupyterLite-Seite baut ein GitHub-Actions-Workflow (`.github/workflows/deploy.yml`) bei jedem Push auf `main` und
  veröffentlicht sie über GitHub Pages. Dafür muss unter *Settings → Pages* als *Source* „GitHub Actions“ eingestellt sein.
- Lokal bauen: `pip install -r requirements.txt` und `jupyter lite build --contents content --output-dir _site`.

## Quellen

Die Aufgabentexte und Beispieldaten stammen von den Bundesweiten Informatikwettbewerben (BWINF),
[bwinf.de](https://bwinf.de). Die Fotos in der Aufgabe St. Egano stammen von pixabay (Quellenangaben in den Ordnern
`beispieldaten` bzw. `daten`).
n.