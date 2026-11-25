# Werkzeuge für die 1. Runde des Bundeswettbewerbs Informatik

[← zur Übersicht der 1. Runde](https://github.com/ktheu/bwinfN/blob/main/bwinf1.md)

Diese Seite ordnet die Aufgaben 1 bis 5 der 1. Runde vom 30. bis 44. Wettbewerb (2011/12 bis 2025/26) nach den
**Werkzeugen**, die man für sie braucht: Algorithmen, Denkweisen und Python-Bibliotheken. Zu jedem Werkzeug steht kurz, was
es ist, und welche Aufgaben es brauchen. Ein Klick auf eine Aufgabe öffnet ihr Lösungsnotebook. So kannst du ein Verfahren
gezielt an mehreren Aufgaben üben. Am Ende steht ein Vorschlag für eine Reihenfolge.

Viele Aufgaben brauchen mehrere Werkzeuge und stehen deshalb mehrmals da. Was ein Werkzeug genau leistet, erklärt jedes
Lösungsnotebook im Abschnitt „Was dir bei dieser Aufgabe hilft“.

## Voraussetzung: die Werkzeuge der 3. Runde

Die Aufgaben der 1. Runde setzen voraus, was du für die Junioraufgaben brauchst: Texte, Listen, Funktionen und Dateien,
Zählen und Suchen, alle Möglichkeiten mit Schleifen durchprobieren, Tabellen und Raster, Simulation, Wörterbücher und Mengen,
Zufall, Sortieren und gierige Strategien. Das alles steht im [Lehrgang zum Jugendwettbewerb](https://github.com/ktheu/bwinfN/blob/main/jwinf3.md),
vor allem in Phase B (Notebooks 09 bis 16). Aus Phase C sind für die 1. Runde besonders wichtig:
[Rekursion][L22], [Erreichbarkeit][L21], [Geometrie mit Koordinaten][L17] und [Zeichnen zur Kontrolle][L19].

## 1. Systematisch suchen

**Alle Möglichkeiten durchprobieren (Brute Force).** Bei kleinen Eingaben die einfachste und sicherste Lösung, oft mit
`itertools`. Wichtig ist die Abschätzung, wie viele Möglichkeiten es gibt.
Lehrgang: [01 Alle Möglichkeiten durchprobieren][LB01].
[Alphametiken][33_Alphametiken], [Streichholzrätsel][39_Streichholzraetsel], [Nandu][42_Nandu],
[Rationalisierung][32_Rationalisierung], [Schiebeparkplatz][40_Schiebeparkplatz], [Buffet-Lotterie][33_BuffetLotterie], [Vortänzer][32_Vortaenzer],
[Zaras dritter Fehler][30_ZarasDritterFehler], [Aladins Lampen][30_AladinsLampen], [Sudokopie][41_Sudokopie],
[Wandertag][43_Wandertag], [Nasser Hund][44_NasserHund]

**Backtracking.** Eine Lösung Schritt für Schritt mit Rekursion aufbauen, einen Schritt zurücknehmen, sobald er nicht mehr
weiterführt, und früh abbrechen.
Lehrgang: [02 Backtracking][LB02].
[Geldtransporter][31_Geldtransporter], [Alphametiken][33_Alphametiken], [Kassiopeias Weg][34_KassiopeiasWeg],
[Schrebergärten][37_Schrebergaerten], [Widerstand][37_Widerstand], [Blumenbeet][38_Blumenbeet], [Rominos][38_Rominos],
[Dreieckspuzzle][39_Dreieckspuzzle], [Wörter aufräumen][39_WoerterAufraeumen], [Marktwaage][40_Marktwaage],
[Arukone][42_Arukone], [Die goldene Mitte][42_DieGoldeneMitte], [Hopsitexte][43_Hopsitexte],
[Bibertomograph][44_Bibertomograph], [ChoreoGraph][44_ChoreoGraph], [Großstadtbauern][44_Grossstadtbauern]

**Schranken (Branch and Bound).** Beim Suchen nach der besten Lösung einen Zweig abbrechen, sobald eine Abschätzung zeigt,
dass er die bisher beste Lösung nicht mehr schlagen kann.
Lehrgang: [03 Schranken und Symmetrien][LB03].
[Geldtransporter][31_Geldtransporter], [Schrebergärten][37_Schrebergaerten], [Blumenbeet][38_Blumenbeet],
[Großstadtbauern][44_Grossstadtbauern]

**Logisches Schließen (Constraint Propagation).** Aus den Regeln zwingende Folgerungen ziehen, bevor man rät. Das macht
die Suche oft winzig.
Lehrgang: [04 Logisch schließen][LB04].
[Fehlerfrei puzzeln][30_FehlerfreiPuzzeln], [Zimmerbelegung][36_Zimmerbelegung], [Bibertomograph][44_Bibertomograph]

**Symmetrien und Normalform.** Lösungen, die durch Drehen, Spiegeln oder Umordnen auseinander hervorgehen, nur einmal
behandeln. Dafür bringt man jede Lösung in eine feste Normalform.
Lehrgang: [03 Schranken und Symmetrien][LB03].
[Twist][37_Twist], [Blumenbeet][38_Blumenbeet], [Rominos][38_Rominos], [Telepaartie][38_Telepaartie],
[Großstadtbauern][44_Grossstadtbauern]

**Binäre Suche und Meet in the Middle.** In einer sortierten Liste schnell suchen, einen Zielwert raten und prüfen oder
eine große Suche in zwei halbe Suchen teilen.
Lehrgang: [13 Binäre Suche][LB13].
[Vollgeladen][40_Vollgeladen], [Marktwaage][40_Marktwaage], [Widerstand][37_Widerstand]

## 2. Graphen

**Breitensuche mit Vorgängern.** Findet in einem Graphen den Weg mit den wenigsten Schritten. Merkt man sich zu jedem
Knoten den Vorgänger, kann man den Weg rekonstruieren. Die Knoten sind oft keine Orte, sondern **Zustände**.
Lehrgang: [05 Breitensuche][LB05], [06 Zustände][LB06].
[Faires Füllen][33_FairesFuellen], [Rotation][35_Rotation], [Telepaartie][38_Telepaartie], [Hüpfburg][41_Huepfburg],
[Zauberschule][42_Zauberschule], [Arukone][42_Arukone], [Zimmerbelegung][36_Zimmerbelegung],
[Städtepartner][30_Staedtepartner]

**Zustände geschickt wählen.** Der Trick ist oft, was ein Knoten ist: zwei Figuren zugleich, Ort und Uhrzeit, Zwischenfelder für
einen Schritt, der länger dauert.
[Faires Füllen][33_FairesFuellen], [Radfahrspaß][35_Radfahrspass], [Hüpfburg][41_Huepfburg],
[Zauberschule][42_Zauberschule], [Das ägyptische Grabmal][43_AegyptischesGrabmal]

**Kürzeste Wege mit Gewichten (Dijkstra).** Wenn die Schritte verschieden viel kosten, mit einer Prioritätswarteschlange
(`heapq`).
Lehrgang: [07 Dijkstra][LB07].
[Buhnenrennen][35_Buhnenrennen], [Nummernmerker][38_Nummernmerker], [Zauberschule][42_Zauberschule],
[Stadtführung][42_Stadtfuehrung], [Das ägyptische Grabmal][43_AegyptischesGrabmal]

**Labyrinthe ohne Karte.** Wege finden, wenn man nur die Umgebung sieht (Linke-Hand-Regel, Pledge-Algorithmus).
[Turn 90][31_Turn90]

**Reihenfolgen und Kreise (topologische Sortierung).** Dinge so ordnen, dass alle Vorgaben „A vor B“ erfüllt sind, und
Widersprüche als Kreise erkennen.
Lehrgang: [08 Reihenfolgen][LB08].
[Schwierigkeiten][43_Schwierigkeiten]

**Bäume.** Verschachtelte Strukturen (Mobile, Schaltungen, Klammerausdrücke) als Baum speichern und rekursiv auswerten.
Lehrgang: [09 Bäume][LB09].
[Mobile][33_Mobile], [Widerstand][37_Widerstand], [Drehfreudig][44_Drehfreudig]

**Zuordnen (Matching) mit verbessernden Wegen.** Paare bilden, sodass möglichst viele oder möglichst gute Paare entstehen.
Eine bestehende Zuordnung lässt sich über einen verbessernden Weg vergrößern.
Lehrgang: [14 Zuordnen][LB14].
[Städtepartner][30_Staedtepartner], [Tutorien][32_Tutorien], [Wörter aufräumen][39_WoerterAufraeumen],
[Wichteln][39_Wichteln]

## 3. Dynamische Programmierung

**Zwischenergebnisse merken (Memoisierung, dynamische Programmierung).** Eine Aufgabe in kleinere gleichartige Teilaufgaben
zerlegen und jedes Teilergebnis nur einmal ausrechnen, in einem Wörterbuch oder einer Tabelle.
Lehrgang: [10 Merken][LB10], [11 Tabellen][LB11].
[Zaras dritter Fehler][30_ZarasDritterFehler], [Geldtransporter][31_Geldtransporter], [Flaschenzug][34_Flaschenzug],
[Buhnenrennen][35_Buhnenrennen], [Schwimmbad][36_Schwimmbad], [Auto-Scrabble][36_AutoScrabble],
[Superstar][37_Superstar], [Voll daneben][37_VollDaneben], [Nummernmerker][38_Nummernmerker],
[Urlaubsfahrt][38_Urlaubsfahrt], [Die goldene Mitte][42_DieGoldeneMitte], [Stadtführung][42_Stadtfuehrung],
[Wandertag][43_Wandertag], [Bibertomograph][44_Bibertomograph]

**Präfixsummen.** Summen über beliebige Abschnitte einer Liste mit einer einzigen Subtraktion ausrechnen.
Lehrgang: [11 Tabellen][LB11].
[Zaras dritter Fehler][30_ZarasDritterFehler], [Flaschenzug][34_Flaschenzug], [Voll daneben][37_VollDaneben]

## 4. Gierige Verfahren und warum sie stimmen

**Greedy mit Begründung.** Immer den im Moment besten Schritt nehmen. In der 1. Runde gehört dazu eine Begründung, warum
das zum Ziel führt (zum Beispiel ein Austauschargument), oder ein Vergleich mit einer genauen Lösung.
Lehrgang: [12 Greedy][LB12].
[Frühsport][31_Fruehsport], [Mobile][33_Mobile] (wie bei Huffman), [Urlaubsfahrt][38_Urlaubsfahrt],
[Vollgeladen][40_Vollgeladen], [Arukone][42_Arukone], [Wichteln][39_Wichteln] (als Vergleich)

## 5. Simulation für Fortgeschrittene

**Ereignisse der Zeit nach abarbeiten.** Statt jede Minute zu simulieren, springt man mit einer Prioritätswarteschlange
(`heapq`) von Ereignis zu Ereignis.
Lehrgang: [15 Ereignisse und Zufall][LB15].
[Verzinkt][41_Verzinkt], [Fahrradwerkstatt][41_Fahrradwerkstatt]

**Schritt für Schritt simulieren.** Zustand festlegen, Regeln in eine feste Reihenfolge bringen, gleichzeitige Aktionen
richtig behandeln, Endlosschleifen und Sonderfälle erkennen.
[Kaffeerunde][31_Kaffeerunde], [Buffet-Lotterie][33_BuffetLotterie], [Pong][33_Pong], [Ameisenfutter][34_Ameisenfutter],
[Vortänzer][32_Vortaenzer], [Würfelglück][40_Wuerfelglueck], [Nandu][42_Nandu], [Hopsitexte][43_Hopsitexte]

**Monte-Carlo-Verfahren.** Ein Zufallsexperiment sehr oft wiederholen und die Häufigkeiten auswerten, mit festem Startwert
für `random`, damit es nachvollziehbar bleibt.
Lehrgang: [15 Ereignisse und Zufall][LB15].
[Kaffeerunde][31_Kaffeerunde], [Ameisenfutter][34_Ameisenfutter], [Tobis Turnier][39_TobisTurnier],
[Würfelglück][40_Wuerfelglueck], [Verzinkt][41_Verzinkt]

**Spiele und Strategien.** Strategien gegeneinander antreten lassen, aus früheren Runden lernen, beste Antworten und
gemischte Strategien (Spieltheorie), Spielbäume und Gewinnstellungen.
Lehrgang: [19 Spiele][LB19].
[Versteigerung][32_Versteigerung], [Pong][33_Pong], [Groker][34_Groker],
[Bauernopfer][36_Bauernopfer]

## 6. Heuristiken

**Lokale Suche und Zufall mit Neustart.** Wenn die genaue Lösung zu lange dauert: eine Lösung schrittweise verbessern
(Hill-Climbing, Simulated Annealing) oder zufällig neu beginnen, bis es passt.
Lehrgang: [16 Heuristiken][LB16].
[Fehlerfrei puzzeln][30_FehlerfreiPuzzeln], [Schlüssellöcher][34_Schluesselloecher], [Wortsuche][40_Wortsuche]

## 7. Geometrie

**Rechnen mit Koordinaten.** Vektoren, Geraden, Schnittpunkte von Strecken, Abstände von Punkt zu Strecke und von Strecke
zu Strecke. Kommazahlen vergleicht man nie mit `==`, sondern mit einer kleinen Toleranz.
Lehrgang: [17 Geometrie][LB17].
[SVG-Fraktale][31_SVGFraktale], [Pong][33_Pong], [Dreiecke zählen][36_DreieckeZaehlen], [Krocket][43_Krocket],
[Nasser Hund][44_NasserHund]

**Raster und Abstände auf dem Gitter.**
[Ameisenfutter][34_Ameisenfutter], [Kassiopeias Weg][34_KassiopeiasWeg], [Vortänzer][32_Vortaenzer],
[Wortsuche][40_Wortsuche], [Arukone][42_Arukone]

## 8. Mathematik

**Rechnen modulo 2 und das Gauß-Verfahren.** [Aladins Lampen][30_AladinsLampen]
Lehrgang: [18 Mathematik][LB18].

**Größter gemeinsamer Teiler (euklidischer Algorithmus).** [Rationalisierung][32_Rationalisierung], [Mobile][33_Mobile]
Lehrgang: [18 Mathematik][LB18].

**Kombinatorik und große Zahlen.** Möglichkeiten zählen, ohne sie alle aufzuzählen; Python rechnet mit beliebig großen ganzen
Zahlen. [Tutorien][32_Tutorien], [Flaschenzug][34_Flaschenzug], [Schlüssellöcher][34_Schluesselloecher]

**Wahrscheinlichkeiten genau ausrechnen.** [Tobis Turnier][39_TobisTurnier]

**Exakt rechnen mit Brüchen.** `fractions.Fraction` oder Zähler und Nenner selbst speichern.
Lehrgang: [18 Mathematik][LB18].
[Rationalisierung][32_Rationalisierung], [Urlaubsfahrt][38_Urlaubsfahrt], [Drehfreudig][44_Drehfreudig]

**Invarianten und Schubfachprinzip.** Eine Größe finden, die sich nie ändert, und damit zeigen, dass etwas unmöglich ist.
Lehrgang: [18 Mathematik][LB18].
[Frühsport][31_Fruehsport], [Kassiopeias Weg][34_KassiopeiasWeg] (Schachbrettfärbung), [Bauernopfer][36_Bauernopfer],
[Sudokopie][41_Sudokopie], [ChoreoGraph][44_ChoreoGraph] (gerade und ungerade Umordnungen)

**Bitmuster, Hamming-Abstand und Codes.** [Schlüssellöcher][34_Schluesselloecher]

**Hash-Funktionen.** [Wer spielt fair?][30_WerSpieltFair]

## 9. Texte, Bilder, Daten

**Texte zerlegen und durchsuchen.** Tokenisieren, ein Muster an jeder Stelle anlegen, Wörter in einer Menge nachschlagen.
[Zaras dritter Fehler][30_ZarasDritterFehler], [Auto-Scrabble][36_AutoScrabble], [Twist][37_Twist], [Störung][41_Stoerung]

**Klammerfolgen und Verschachtelung.** [Vortänzer][32_Vortaenzer], [Radfahrspaß][35_Radfahrspass],
[Drehfreudig][44_Drehfreudig]

**Datum und Zeit umrechnen.** [Sprichwort][35_Sprichwort], [Fahrradwerkstatt][41_Fahrradwerkstatt]

**Bilder als Zahlen.** Pixel lesen, Nachbarpixel vergleichen, glätten und abziehen, mit Pillow und numpy.
[Fotoforensik][32_Fotoforensik], [Rhinozelfant][35_Rhinozelfant]

**Intervalle.** [Wandertag][43_Wandertag], [Das ägyptische Grabmal][43_AegyptischesGrabmal]

## 10. Modellieren und die Aufgabe verstehen

In der 1. Runde ist oft nicht das Programm schwer, sondern die Frage, was genau gesucht ist. Man muss die Aufgabe in ein
klares Modell übersetzen: Was ist ein Zustand, was ein Knoten, was eine Zahl? Welche Lesart einer unklaren Stelle wähle ich,
und wie begründe ich sie in der Dokumentation?
Lehrgang: [20 Dokumentation][LB20].
[Sprichwort][35_Sprichwort], [Störung][41_Stoerung], [Stadtführung][42_Stadtfuehrung], [Krocket][43_Krocket],
[Nasser Hund][44_NasserHund], [Bibertomograph][44_Bibertomograph], [Großstadtbauern][44_Grossstadtbauern]

## 11. Python-Bibliotheken

Alle Bibliotheken gehören zu Python oder laufen in JupyterLite. Die Tabelle zählt, in wie vielen Lösungsnotebooks sie
vorkommen.

| Bibliothek | wofür | Notebooks |
|---|---|---|
| `random` | Zufall, Simulation, Testdaten | 24 |
| `itertools` (`product`, `permutations`, `combinations`) | alle Möglichkeiten erzeugen | 17 |
| `matplotlib` | zeichnen zur Kontrolle | 12 |
| `collections.deque` | Warteschlange für die Breitensuche | 7 |
| `math` (`sqrt`, `gcd`, `perm`) | Wurzeln, ggT, Anzahlen | 10 |
| `heapq` | Prioritätswarteschlange (Dijkstra, Ereignisse) | 4 |
| `fractions.Fraction` | exakt rechnen mit Brüchen | 2 |
| `bisect` | binäre Suche in sortierten Listen | 2 |
| `numpy` | große Zahlentabellen, Bilder | 2 |
| `PIL` (Pillow) | Bilder lesen und schreiben | 1 |
| `re`, `hashlib`, `secrets`, `xml.etree` | Textmuster, Hash-Funktion, sicherer Zufall, SVG lesen | je 1 |

Beispiele: `deque` in [Faires Füllen][33_FairesFuellen], `heapq` in [Zauberschule][42_Zauberschule], `bisect` in
[Marktwaage][40_Marktwaage], `Fraction` in [Urlaubsfahrt][38_Urlaubsfahrt], `itertools.product` in [Nandu][42_Nandu].

## 12. MiniZinc

41 Lösungsnotebooks lösen die Aufgabe am Ende zusätzlich mit einem MiniZinc-Modell. Das passt gut zu Zuordnungs- und
Rätselaufgaben, zum Beispiel [Wichteln][39_Wichteln], [Blumenbeet][38_Blumenbeet], [Alphametiken][33_Alphametiken]
und [Bibertomograph][44_Bibertomograph]. Bei großen Packaufgaben wie den 5 × 5 × 5-Kisten in
[Die goldene Mitte][42_DieGoldeneMitte] braucht der Solver schon lange, bei Folgen von Schritten wird es schwer: Einen
Versuch mit Grenzen zeigt [ChoreoGraph][44_ChoreoGraph].
Acht Notebooks erklären, warum MiniZinc dort nicht passt: [Frühsport][31_Fruehsport], [Pong][33_Pong],
[Ameisenfutter][34_Ameisenfutter], [Groker][34_Groker], [Schlüssellöcher][34_Schluesselloecher],
[Superstar][37_Superstar], [Twist][37_Twist], [Rominos][38_Rominos].
Wie man mit MiniZinc arbeitet, zeigen die Arbeitsblätter
[Grundlagen](https://ktheu.github.io/python-uebungen/notebooks/index.html?path=minizinc_grundlagen.ipynb),
[Daten](https://ktheu.github.io/python-uebungen/notebooks/index.html?path=minizinc_daten.ipynb) und
[Zuordnen und Planen](https://ktheu.github.io/python-uebungen/notebooks/index.html?path=minizinc_zuordnung.ipynb).

## Vorschlag für eine Reihenfolge zum Üben

Jeder Schritt beginnt mit Aufgaben, bei denen das neue Werkzeug gut zu sehen ist, und endet mit einer, die es mit anderem
kombiniert. Bearbeite eine Aufgabe zuerst selbst und sieh dir das Lösungsnotebook erst danach an.

1. **Durchprobieren mit `itertools`:** [Alphametiken][33_Alphametiken], [Nandu][42_Nandu],
   [Streichholzrätsel][39_Streichholzraetsel]
2. **Simulation:** [Buffet-Lotterie][33_BuffetLotterie], [Würfelglück][40_Wuerfelglueck], [Kaffeerunde][31_Kaffeerunde]
3. **Backtracking:** [Dreieckspuzzle][39_Dreieckspuzzle], [Kassiopeias Weg][34_KassiopeiasWeg],
   [Blumenbeet][38_Blumenbeet], dann [Die goldene Mitte][42_DieGoldeneMitte]
4. **Breitensuche über Zustände:** [Faires Füllen][33_FairesFuellen], [Rotation][35_Rotation],
   [Telepaartie][38_Telepaartie], dann [Hüpfburg][41_Huepfburg]
5. **Zwischenergebnisse merken:** [Schwimmbad][36_Schwimmbad], [Auto-Scrabble][36_AutoScrabble],
   [Flaschenzug][34_Flaschenzug], dann [Voll daneben][37_VollDaneben]
6. **Greedy und binäre Suche:** [Vollgeladen][40_Vollgeladen], [Urlaubsfahrt][38_Urlaubsfahrt],
   [Marktwaage][40_Marktwaage]
7. **Kürzeste Wege mit Dijkstra:** [Zauberschule][42_Zauberschule], [Buhnenrennen][35_Buhnenrennen],
   dann [Das ägyptische Grabmal][43_AegyptischesGrabmal]
8. **Ereignisse und Zufall:** [Verzinkt][41_Verzinkt], [Fahrradwerkstatt][41_Fahrradwerkstatt],
   [Tobis Turnier][39_TobisTurnier]
9. **Geometrie:** [Nasser Hund][44_NasserHund], [Dreiecke zählen][36_DreieckeZaehlen], [Krocket][43_Krocket]
10. **Zuordnen:** [Wörter aufräumen][39_WoerterAufraeumen], [Wichteln][39_Wichteln], [Städtepartner][30_Staedtepartner]
11. **Suche mit Schranken und Symmetrien:** [Rominos][38_Rominos], [Großstadtbauern][44_Grossstadtbauern],
    [Bibertomograph][44_Bibertomograph]
12. **Heuristiken:** [Wortsuche][40_Wortsuche], [Schlüssellöcher][34_Schluesselloecher],
    [Fehlerfrei puzzeln][30_FehlerfreiPuzzeln]

[← zur Übersicht der 1. Runde](https://github.com/ktheu/bwinfN/blob/main/bwinf1.md)

[LB01]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/01_durchprobieren.ipynb
[LB02]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/02_backtracking.ipynb
[LB03]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/03_schranken_symmetrien.ipynb
[LB04]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/04_logisch_schliessen.ipynb
[LB05]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/05_breitensuche.ipynb
[LB06]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/06_zustaende.ipynb
[LB07]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/07_dijkstra.ipynb
[LB08]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/08_reihenfolgen.ipynb
[LB09]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/09_baeume.ipynb
[LB10]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/10_merken.ipynb
[LB11]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/11_tabellen_dp.ipynb
[LB12]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/12_greedy.ipynb
[LB13]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/13_binaere_suche.ipynb
[LB14]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/14_zuordnen.ipynb
[LB15]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/15_ereignisse_zufall.ipynb
[LB16]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/16_heuristiken.ipynb
[LB17]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/17_geometrie.ipynb
[LB18]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/18_mathematik.ipynb
[LB19]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/19_spiele.ipynb
[LB20]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/20_dokumentation.ipynb
[L17]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/17_geometrie.ipynb
[L19]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/19_zeichnen.ipynb
[L21]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/21_erreichbarkeit.ipynb
[L22]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_jwinf3/22_rekursion.ipynb
[30_AladinsLampen]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/30_AladinsLampen/aladinslampen_loesung.ipynb
[30_FehlerfreiPuzzeln]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/30_FehlerfreiPuzzeln/fehlerfreipuzzeln_loesung.ipynb
[30_Staedtepartner]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/30_Staedtepartner/staedtepartner_loesung.ipynb
[30_WerSpieltFair]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/30_WerSpieltFair/werspieltfair_loesung.ipynb
[30_ZarasDritterFehler]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/30_ZarasDritterFehler/zarasdritterfehler_loesung.ipynb
[31_Fruehsport]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/31_Fruehsport/fruehsport_loesung.ipynb
[31_Geldtransporter]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/31_Geldtransporter/geldtransporter_loesung.ipynb
[31_Kaffeerunde]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/31_Kaffeerunde/kaffeerunde_loesung.ipynb
[31_SVGFraktale]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/31_SVGFraktale/svgfraktale_loesung.ipynb
[31_Turn90]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/31_Turn90/turn90_loesung.ipynb
[32_Fotoforensik]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/32_Fotoforensik/fotoforensik_loesung.ipynb
[32_Rationalisierung]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/32_Rationalisierung/rationalisierung_loesung.ipynb
[32_Tutorien]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/32_Tutorien/tutorien_loesung.ipynb
[32_Versteigerung]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/32_Versteigerung/versteigerung_loesung.ipynb
[32_Vortaenzer]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/32_Vortaenzer/vortaenzer_loesung.ipynb
[33_Alphametiken]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/33_Alphametiken/alphametiken_loesung.ipynb
[33_BuffetLotterie]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/33_BuffetLotterie/buffetlotterie_loesung.ipynb
[33_FairesFuellen]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/33_FairesFuellen/fairesfuellen_loesung.ipynb
[33_Mobile]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/33_Mobile/mobile_loesung.ipynb
[33_Pong]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/33_Pong/pong_loesung.ipynb
[34_Ameisenfutter]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/34_Ameisenfutter/ameisenfutter_loesung.ipynb
[34_Flaschenzug]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/34_Flaschenzug/flaschenzug_loesung.ipynb
[34_Groker]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/34_Groker/groker_loesung.ipynb
[34_KassiopeiasWeg]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/34_KassiopeiasWeg/kassiopeiasweg_loesung.ipynb
[34_Schluesselloecher]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/34_Schluesselloecher/schluesselloecher_loesung.ipynb
[35_Buhnenrennen]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/35_Buhnenrennen/buhnenrennen_loesung.ipynb
[35_Radfahrspass]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/35_Radfahrspass/radfahrspass_loesung.ipynb
[35_Rhinozelfant]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/35_Rhinozelfant/rhinozelfant_loesung.ipynb
[35_Rotation]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/35_Rotation/rotation_loesung.ipynb
[35_Sprichwort]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/35_Sprichwort/sprichwort_loesung.ipynb
[36_AutoScrabble]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/36_AutoScrabble/autoscrabble_loesung.ipynb
[36_Bauernopfer]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/36_Bauernopfer/bauernopfer_loesung.ipynb
[36_DreieckeZaehlen]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/36_DreieckeZaehlen/dreieckezaehlen_loesung.ipynb
[36_Schwimmbad]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/36_Schwimmbad/schwimmbad_loesung.ipynb
[36_Zimmerbelegung]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/36_Zimmerbelegung/zimmerbelegung_loesung.ipynb
[37_Schrebergaerten]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/37_Schrebergaerten/schrebergaerten_loesung.ipynb
[37_Superstar]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/37_Superstar/superstar_loesung.ipynb
[37_Twist]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/37_Twist/twist_loesung.ipynb
[37_VollDaneben]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/37_VollDaneben/voll_daneben_loesung.ipynb
[37_Widerstand]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/37_Widerstand/widerstand_loesung.ipynb
[38_Blumenbeet]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/38_Blumenbeet/blumenbeet_loesung.ipynb
[38_Nummernmerker]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/38_Nummernmerker/nummernmerker_loesung.ipynb
[38_Rominos]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/38_Rominos/rominos_loesung.ipynb
[38_Telepaartie]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/38_Telepaartie/telepaartie_loesung.ipynb
[38_Urlaubsfahrt]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/38_Urlaubsfahrt/urlaubsfahrt_loesung.ipynb
[39_Dreieckspuzzle]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/39_Dreieckspuzzle/dreieckspuzzle_loesung.ipynb
[39_Streichholzraetsel]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/39_Streichholzraetsel/streichholzraetsel_loesung.ipynb
[39_TobisTurnier]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/39_TobisTurnier/tobisturnier_loesung.ipynb
[39_Wichteln]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/39_Wichteln/wichteln_loesung.ipynb
[39_WoerterAufraeumen]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/39_WoerterAufraeumen/woerteraufraeumen_loesung.ipynb
[40_Marktwaage]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/40_Marktwaage/marktwaage_loesung.ipynb
[40_Schiebeparkplatz]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/40_Schiebeparkplatz/schiebeparkplatz_loesung.ipynb
[40_Vollgeladen]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/40_Vollgeladen/vollgeladen_loesung.ipynb
[40_Wortsuche]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/40_Wortsuche/wortsuche_loesung.ipynb
[40_Wuerfelglueck]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/40_Wuerfelglueck/wuerfelglueck_loesung.ipynb
[41_Fahrradwerkstatt]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/41_Fahrradwerkstatt/fahrradwerkstatt_loesung.ipynb
[41_Huepfburg]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/41_Huepfburg/huepfburg_loesung.ipynb
[41_Stoerung]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/41_Stoerung/stoerung_loesung.ipynb
[41_Sudokopie]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/41_Sudokopie/sudokopie_loesung.ipynb
[41_Verzinkt]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/41_Verzinkt/verzinkt_loesung.ipynb
[42_Arukone]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/42_Arukone/arukone_loesung.ipynb
[42_DieGoldeneMitte]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/42_DieGoldeneMitte/goldene_mitte_loesung.ipynb
[42_Nandu]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/42_Nandu/nandu_loesung.ipynb
[42_Stadtfuehrung]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/42_Stadtfuehrung/stadtfuehrung_loesung.ipynb
[42_Zauberschule]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/42_Zauberschule/zauberschule_loesung.ipynb
[43_AegyptischesGrabmal]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/43_AegyptischesGrabmal/aegyptischesgrabmal_loesung.ipynb
[43_Hopsitexte]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/43_Hopsitexte/hopsitexte_loesung.ipynb
[43_Krocket]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/43_Krocket/krocket_loesung.ipynb
[43_Schwierigkeiten]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/43_Schwierigkeiten/schwierigkeiten_loesung.ipynb
[43_Wandertag]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/43_Wandertag/wandertag_loesung.ipynb
[44_Bibertomograph]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/44_Bibertomograph/bibertomograph_loesung.ipynb
[44_ChoreoGraph]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/44_ChoreoGraph/choreograph_loesung.ipynb
[44_Drehfreudig]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/44_Drehfreudig/drehfreudig_loesung.ipynb
[44_Grossstadtbauern]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/44_Grossstadtbauern/grossstadtbauern_loesung.ipynb
[44_NasserHund]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/44_NasserHund/nasserhund_loesung.ipynb
