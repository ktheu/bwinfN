# Werkzeuge für die 2. Runde des Bundeswettbewerbs Informatik

[← zur Übersicht der 2. Runde](https://github.com/ktheu/bwinfN/blob/main/bwinf2.md)

Diese Seite ordnet die Aufgaben der 2. Runde vom 30. bis 44. Wettbewerb (2011/12 bis 2025/26) nach den **Werkzeugen**, die
man für sie braucht: Algorithmen, Denkweisen und Python-Bibliotheken. Zu jedem Werkzeug steht kurz, was es ist und welche
Aufgaben es brauchen. Ein Klick auf eine Aufgabe öffnet ihr Lösungsnotebook. Am Ende steht ein Vorschlag für eine Reihenfolge.

Viele Aufgaben brauchen mehrere Werkzeuge und stehen deshalb mehrmals da. Was ein Werkzeug genau leistet, erklärt jedes
Lösungsnotebook im Abschnitt „Was dir bei dieser Aufgabe hilft“.

## Voraussetzung: die Werkzeuge der 1. Runde

Die 2. Runde setzt voraus, was du für die 1. Runde brauchst: Durchprobieren, Backtracking mit Schranken, Breitensuche über
Zustände, Dijkstra, Merken und Tabellen, Greedy mit Begründung, Heuristiken, Geometrie und Simulation. Das alles steht in der
**[Werkzeugübersicht der 1. Runde](https://github.com/ktheu/bwinfN/blob/main/content/bwinf1/werkzeuge.md)** und im
[Lehrgang zur 1. Runde](https://github.com/ktheu/bwinfN/blob/main/bwinf1.md).

Neu ist in der 2. Runde vor allem dreierlei:
- Oft weiß man nicht, ob eine Lösung die beste ist. Man braucht Heuristiken und muss zeigen, wie gut sie sind.
- Die Eingaben sind groß. Man muss die Struktur der Aufgabe ausnutzen.
- Zusatzpunkte gibt es für eigene, begründete Erweiterungen.

## 1. Prüfen und die Güte messen

**Ein Schiedsrichter für jede Lösung.** Bevor man einer Lösung glaubt, prüft ein eigenes, einfaches Programm, ob sie alle
Regeln einhält. Bei kleinen Eingaben vergleicht man außerdem mit einer vollständigen Suche.
Lehrgang: [01 Prüfen und Schranken][L201].
[Missglückte Drohnenlieferung][34_MissglueckteDrohnenlieferung], [Wehret den Wildschweinen!][36_WehretDenWildschweinen],
[Trickey][30_Trickey], [Spießgesellen][39_Spiessgesellen], [Eisbudendilemma][39_Eisbudendilemma]

**Schranken.** Eine untere (oder obere) Schranke sagt, wie gut es höchstens gehen kann. Der Abstand der eigenen Lösung zur
Schranke zeigt, wie viel noch zu holen wäre, auch wenn man das Optimum nicht kennt.
Lehrgang: [01 Prüfen und Schranken][L201].
[Missglückte Drohnenlieferung][34_MissglueckteDrohnenlieferung] (Manhattan-Abstand),
[Flohmarkt in Langdorf][39_FlohmarktInLangdorf] (Fläche), [Die Kunst der Fuge][36_DieKunstDerFuge] (Schubfachprinzip),
[Die Siedler][42_DieSiedler], [Wehret den Wildschweinen!][36_WehretDenWildschweinen], [Pancake Sort][41_PancakeSort]

## 2. Erst nachdenken, dann programmieren

**Die Struktur der Aufgabe erkennen.** Oft folgt aus den Regeln etwas, das die Suche fast überflüssig macht: eine erzwungene
Reihenfolge, eine Formel, eine Zerlegung in unabhängige Teile.
Lehrgang: [02 Struktur erkennen][L202].
[Alles Käse][41_AllesKaese] (Zwangsreihenfolge), [Stilvolle Päckchen][42_StilvollePaeckchen] (Cliquen),
[Hex-Max][40_HexMax] (umformulieren), [Gießroboter][44_Giessroboter] (gute Modellierung), [Trickey][30_Trickey],
[Die Kunst der Fuge][36_DieKunstDerFuge]

**Die Frage umdrehen.** Statt alle Wege zu sperren, eine Mauer bauen; statt vom Start aus vom Ziel aus suchen.
[Wehret den Wildschweinen!][36_WehretDenWildschweinen] (Dualität), [Abbiegen?][38_Abbiegen],
[Simultane Labyrinthe][43_SimultaneLabyrinthe] (Abstände vom Ziel aus), [Lisa rennt][37_LisaRennt] (Zeit rückwärts)

**Mengen, Invarianten und XOR.** Mit Mengen ausschließen, was nicht sein kann; eine Größe finden, die sich nie ändert;
mit XOR und Gauß-Verfahren über {0, 1} rechnen.
Lehrgang: [02 Struktur erkennen][L202].
[Spießgesellen][39_Spiessgesellen], [Zara Zackigs Zurückkehr][40_ZaraZackigsZurueckkehr], [Transformers][44_Transformers]
(Invarianten, Normalform), [Eisbudendilemma][39_Eisbudendilemma] (Mengen als Bitmasken)

## 3. Heuristiken

**Gierig eine Lösung bauen.** Schritt für Schritt das tun, was im Moment am meisten bringt. Meist gibt es mehrere sinnvolle
Regeln; man vergleicht sie an allen Beispielen und kennt ihre Grenzen.
Lehrgang: [03 Heuristiken bauen][L203].
[Flohmarkt in Langdorf][39_FlohmarktInLangdorf], [Die Siedler][42_DieSiedler], [Dreiecksbeziehungen][37_Dreiecksbeziehungen],
[Buschfeuer][32_Buschfeuer], [Missglückte Drohnenlieferung][34_MissglueckteDrohnenlieferung], [Rosinen picken][35_RosinenPicken],
[Tourality][31_Tourality], [Laubmaschen][42_Laubmaschen], [Vortänzer Challenge][32_VortaenzerChallenge]

**Lokale Suche, Zufall und Neustarts.** Eine Lösung durch kleine Änderungen verbessern (Bergsteigen), mit Simulated
Annealing auch Verschlechterungen zulassen, mit Zufall neu beginnen, Teile räumen und neu füllen.
Lehrgang: [04 Lokale Suche][L204].
[Kool][30_Kool], [Ned][30_Ned], [Komplementär][31_Komplementaer], [Eisbudendilemma][39_Eisbudendilemma],
[Flohmarkt in Langdorf][39_FlohmarktInLangdorf], [Stilvolle Päckchen][42_StilvollePaeckchen], [Konfetti][43_Konfetti],
[Weniger krumme Touren][41_WenigerKrummeTouren], [Die Kunst der Fuge][36_DieKunstDerFuge], [Müllabfuhr][40_Muellabfuhr]

**Rundreisen und Touren.** Eine kurze Rundreise durch alle Orte (TSP: nächster Nachbar, Einfügen, 2-opt) oder eine Tour
über alle Straßen (Eulerkreis, Knoten ungeraden Grades paaren).
[Gießroboter][44_Giessroboter], [Müllabfuhr][40_Muellabfuhr], [Ned][30_Ned], [Tourality][31_Tourality],
[Weniger krumme Touren][41_WenigerKrummeTouren]

## 4. Vollständige Suche bei großen Fällen

**Backtracking mit gutem Abschneiden.** Dort verzweigen, wo es die wenigsten Möglichkeiten gibt, Sackgassen früh erkennen
und merken, Symmetrien ausnutzen, gleiche Teile zusammenfassen.
Lehrgang: [06 Backtracking für große Fälle][L206].
[Konfetti][43_Konfetti], [Die Kunst der Fuge][36_DieKunstDerFuge], [Komplementär][31_Komplementaer], [Kool][30_Kool],
[Stromrallye][38_Stromrallye], [Weniger krumme Touren][41_WenigerKrummeTouren], [Buschfeuer][32_Buschfeuer],
[Lebenslinien][32_Lebenslinien], [Rosinen picken][35_RosinenPicken], [Alles Käse][41_AllesKaese]

**Große Zustandsräume.** Zustände kompakt und in Normalform speichern, die Größe des Raums abschätzen, in Schichten suchen,
vom Ziel aus rechnen.
Lehrgang: [07 Große Zustandsräume][L207].
[Seilschaften][33_Seilschaften], [Simultane Labyrinthe][43_SimultaneLabyrinthe], [Pancake Sort][41_PancakeSort],
[Transformers][44_Transformers], [Stromrallye][38_Stromrallye], [Rechtsrum in Rechthausen][35_RechtsrumInRechthausen]

**Spiele.** Gewinnstellungen mit Tiefenschranke, Rückwärtsanalyse vom Spielende her, Spielbaum und Minimax.
Lehrgang: [07 Große Zustandsräume][L207] (nur als Verweis).
[Schach dem Wildschwein][37_SchachDemWildschwein], [Tourality][31_Tourality], [Vortänzer Challenge][32_VortaenzerChallenge]

## 5. Graphen

**Kürzeste Wege mit Nebenbedingungen.** Dijkstra auf einem erweiterten Graphen, dessen Knoten mehr als einen Ort
beschreiben (Ort und Richtung, Ort und Zeit), mit mehreren Startknoten, mit zwei Zielen nacheinander.
[Abbiegen?][38_Abbiegen], [Rechtsrum in Rechthausen][35_RechtsrumInRechthausen], [Lieferkette][44_Lieferkette],
[Lisa rennt][37_LisaRennt], [Müllabfuhr][40_Muellabfuhr], [Wehret den Wildschweinen!][36_WehretDenWildschweinen]

**Struktur von Graphen.** Brücken und Zusammenhangskomponenten, Erreichbarkeit in gerichteten Graphen (auch rückwärts),
Cliquen, 2-Färbung.
[Transformers][44_Transformers] (Brücken), [Torkelnde Yamyams][34_TorkelndeYamyams], [Rosinen picken][35_RosinenPicken],
[Lebenslinien][32_Lebenslinien], [Stilvolle Päckchen][42_StilvollePaeckchen], [Wehret den Wildschweinen!][36_WehretDenWildschweinen]

**Fluss, Schnitt und Zuordnung.** Maximaler Fluss und minimaler Schnitt (Edmonds-Karp), Zuordnungsprobleme.
[Rosinen picken][35_RosinenPicken] (für Neugierige), [Missglückte Drohnenlieferung][34_MissglueckteDrohnenlieferung]

## 6. Dynamische Programmierung

**Tabellen für Fortgeschrittene.** Nach Kosten aufbauen (erst alles mit Kosten 1, dann 2, …), Tabelle von hinten mit
gieriger Wahl von vorn, Teilstücke von Programmen, Rückwärtsrechnung im Spiel.
[Geburtstag][38_Geburtstag], [Hex-Max][40_HexMax], [Rechenrätsel][40_Rechenraetsel],
[Vortänzer Challenge][32_VortaenzerChallenge], [Ned][30_Ned], [Tourality][31_Tourality], [Pancake Sort][41_PancakeSort],
[Lieferkette][44_Lieferkette], [Konfetti][43_Konfetti] (größte Teilsumme)

## 7. Geometrie

**Polygone, Winkel und Wege um Hindernisse.** Punkt im Polygon, Flächeninhalt, Winkel aus Koordinaten, Sichtbarkeitsgraph,
Toleranzen bei Kommazahlen oder gleich mit ganzen Zahlen rechnen.
[Geburtstagskuchen][34_Geburtstagskuchen] (Polygone, Voronoi, Lloyd), [Lisa rennt][37_LisaRennt] (Sichtbarkeitsgraph),
[Panorama-Kegeln][33_PanoramaKegeln], [Marsch auf Mars][31_MarschAufMars] (Strahl und Kreis, kleinster Kreis),
[Dreiecksbeziehungen][37_Dreiecksbeziehungen], [Die Siedler][42_DieSiedler], [Rechtsrum in Rechthausen][35_RechtsrumInRechthausen],
[Abbiegen?][38_Abbiegen] (ganze Zahlen statt Steigungen), [Weniger krumme Touren][41_WenigerKrummeTouren]

## 8. Simulation und Zufall

**Simulation in Takten und mit gleichzeitigen Aktionen.** Alle Beteiligten sehen sich gleichzeitig um, dann bewegen sich
alle; Strategien in vielen Läufen gegeneinander antreten lassen.
[Marsch auf Mars][31_MarschAufMars], [Buschfeuer][32_Buschfeuer], [Tourality][31_Tourality],
[Missglückte Drohnenlieferung][34_MissglueckteDrohnenlieferung]

**Zufall und Erwartungswert.** Über viele Läufe mitteln, oder gleich mit Wahrscheinlichkeiten rechnen (Übergangstabelle,
Erwartungswert, numerisch integrieren).
[Laubmaschen][42_Laubmaschen], [Panorama-Kegeln][33_PanoramaKegeln], [Torkelnde Yamyams][34_TorkelndeYamyams]

## 9. Texte, Codes und Bilder

**Texte und Codes.** Teilzeichenketten zählen, Positionen statt Zeichenketten speichern, Gruppen verfeinern;
präfixfreie Codes als Baum, Huffman-Codierung.
[Mississippi][33_Mississippi], [Schmucknachrichten][43_Schmucknachrichten], [Kreis-Code][35_KreisCode] (Drehungen einer Zeichenkette)

**Bilder und Raster.** Bilder als Zahlentabellen (`numpy`, `PIL`), Schwellenwert, Zusammenhangskomponenten, Quadtree.
[Kreis-Code][35_KreisCode], [Quo vadis, Quax?][36_QuoVadisQuax], [Buschfeuer][32_Buschfeuer]

## 10. Die Einsendung der 2. Runde

Es gelten die Regeln der 1. Runde, dazu:
- Die Pflichtbeispiele von der BWINF-Webseite gehören in die Dokumentation, neben eigenen Beispielen.
- Zusatzpunkte gibt es für eigenständige Erweiterungen, die sinnvoll sind und eine eigene Schwierigkeit haben. Das muss man
  begründen.
- Man gibt an, ob und wie man Werkzeuge benutzt hat, etwa Bibliotheken oder KI-Systeme.

Gerade bei Heuristiken gehört in die Dokumentation, wie gut das Ergebnis ist: Vergleich mit einer Schranke, mit einer
exakten Lösung kleiner Fälle oder mit anderen Verfahren. Die Lösungsnotebooks vergleichen dazu ehrlich mit den Zahlen der
offiziellen Lösungshinweise, auch wenn sie schlechter sind.
Lehrgang: [16 Experimente auswerten][L216].

## 11. Python-Bibliotheken

Alle Bibliotheken gehören zu Python oder laufen in JupyterLite. Die Tabelle zählt, in wie vielen der 46 Lösungsnotebooks sie
vorkommen.

| Bibliothek | wofür | Notebooks |
|---|---|---|
| `random` | Zufall, Neustarts, Testdaten | 31 |
| `matplotlib` | zeichnen zur Kontrolle | 22 |
| `math` | Wurzeln, Winkel (`atan2`), Anzahlen | 20 |
| `itertools` | alle Möglichkeiten erzeugen | 16 |
| `collections` (`deque`, `Counter`, `defaultdict`) | Warteschlange, Zählen | 12 |
| `heapq` | Prioritätswarteschlange (Dijkstra, gierige Verfahren) | 11 |
| `numpy` | große Zahlentabellen, Bilder | 8 |
| `PIL` (Pillow) | Bilder lesen | 2 |
| `fractions.Fraction` | exakt rechnen mit Brüchen | 1 |

## 12. MiniZinc

36 der 46 Lösungsnotebooks lösen die Aufgabe (oder einen Teil davon) am Ende zusätzlich mit einem MiniZinc-Modell. Bei
Optimierungsaufgaben ist das oft der Vergleich, der zeigt, wie gut die Heuristik ist, etwa bei
[Stilvolle Päckchen][42_StilvollePaeckchen] oder [Flohmarkt in Langdorf][39_FlohmarktInLangdorf]. Kein Modell gibt es bei
Simulation, Bildern und Texten und bei einigen großen Graphaufgaben:
[Marsch auf Mars][31_MarschAufMars], [Vortänzer Challenge][32_VortaenzerChallenge], [Mississippi][33_Mississippi],
[Kreis-Code][35_KreisCode], [Quo vadis, Quax?][36_QuoVadisQuax], [Die Siedler][42_DieSiedler], [Laubmaschen][42_Laubmaschen],
[Gießroboter][44_Giessroboter], [Lieferkette][44_Lieferkette], [Transformers][44_Transformers].
Die Modelle laufen nicht in JupyterLite; man kopiert sie in die MiniZinc IDE oder in den
[MiniZinc Playground](https://play.minizinc.org/). Wie man mit MiniZinc arbeitet, zeigen die Arbeitsblätter
[Grundlagen](https://ktheu.github.io/python-uebungen/notebooks/index.html?path=minizinc_grundlagen.ipynb),
[Daten](https://ktheu.github.io/python-uebungen/notebooks/index.html?path=minizinc_daten.ipynb) und
[Zuordnen und Planen](https://ktheu.github.io/python-uebungen/notebooks/index.html?path=minizinc_zuordnung.ipynb).

## Vorschlag für eine Reihenfolge zum Üben

Jeder Schritt beginnt mit Aufgaben, bei denen das Werkzeug gut zu sehen ist. Bearbeite eine Aufgabe zuerst selbst und sieh
dir das Lösungsnotebook erst danach an.

1. **Zustände und Breitensuche (Wiederholung):** [Seilschaften][33_Seilschaften], [Simultane Labyrinthe][43_SimultaneLabyrinthe],
   dann [Pancake Sort][41_PancakeSort]
2. **Struktur erkennen:** [Spießgesellen][39_Spiessgesellen], [Alles Käse][41_AllesKaese], [Hex-Max][40_HexMax]
3. **Kürzeste Wege mit Nebenbedingungen:** [Abbiegen?][38_Abbiegen], [Lieferkette][44_Lieferkette],
   [Rechtsrum in Rechthausen][35_RechtsrumInRechthausen]
4. **Backtracking für große Fälle:** [Konfetti][43_Konfetti], [Die Kunst der Fuge][36_DieKunstDerFuge],
   [Stromrallye][38_Stromrallye]
5. **Heuristiken mit Güte:** [Missglückte Drohnenlieferung][34_MissglueckteDrohnenlieferung],
   [Flohmarkt in Langdorf][39_FlohmarktInLangdorf], [Stilvolle Päckchen][42_StilvollePaeckchen], dann
   [Gießroboter][44_Giessroboter]
6. **Dynamische Programmierung:** [Geburtstag][38_Geburtstag], [Rechenrätsel][40_Rechenraetsel],
   [Vortänzer Challenge][32_VortaenzerChallenge]
7. **Graphstruktur und Spiele:** [Transformers][44_Transformers], [Torkelnde Yamyams][34_TorkelndeYamyams],
   [Schach dem Wildschwein][37_SchachDemWildschwein]
8. **Geometrie, Bilder, Texte:** [Lisa rennt][37_LisaRennt], [Geburtstagskuchen][34_Geburtstagskuchen],
   [Kreis-Code][35_KreisCode], [Schmucknachrichten][43_Schmucknachrichten]

[L201]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf2/01_pruefen_und_schranken.ipynb
[L202]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf2/02_struktur_erkennen.ipynb
[L203]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf2/03_heuristiken_bauen.ipynb
[L204]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf2/04_lokale_suche.ipynb
[L206]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf2/06_backtracking_gross.ipynb
[L207]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf2/07_grosse_zustandsraeume.ipynb
[L216]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf2/16_experimente.ipynb
[30_Kool]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/30_Kool/kool_loesung.ipynb
[30_Ned]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/30_Ned/ned_loesung.ipynb
[30_Trickey]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/30_Trickey/trickey_loesung.ipynb
[31_Komplementaer]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/31_Komplementaer/komplementaer_loesung.ipynb
[31_MarschAufMars]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/31_MarschAufMars/mars_loesung.ipynb
[31_Tourality]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/31_Tourality/tourality_loesung.ipynb
[32_Buschfeuer]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/32_Buschfeuer/buschfeuer_loesung.ipynb
[32_Lebenslinien]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/32_Lebenslinien/lebenslinien_loesung.ipynb
[32_VortaenzerChallenge]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/32_VortaenzerChallenge/vortaenzer_challenge_loesung.ipynb
[33_Mississippi]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/33_Mississippi/mississippi_loesung.ipynb
[33_PanoramaKegeln]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/33_PanoramaKegeln/kegeln_loesung.ipynb
[33_Seilschaften]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/33_Seilschaften/seilschaften_loesung.ipynb
[34_Geburtstagskuchen]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/34_Geburtstagskuchen/kuchen_loesung.ipynb
[34_MissglueckteDrohnenlieferung]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/34_MissglueckteDrohnenlieferung/drohnen_loesung.ipynb
[34_TorkelndeYamyams]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/34_TorkelndeYamyams/yamyams_loesung.ipynb
[35_KreisCode]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/35_KreisCode/kreiscode_loesung.ipynb
[35_RechtsrumInRechthausen]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/35_RechtsrumInRechthausen/rechthausen_loesung.ipynb
[35_RosinenPicken]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/35_RosinenPicken/rosinen_loesung.ipynb
[36_DieKunstDerFuge]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/36_DieKunstDerFuge/fuge_loesung.ipynb
[36_QuoVadisQuax]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/36_QuoVadisQuax/quax_loesung.ipynb
[36_WehretDenWildschweinen]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/36_WehretDenWildschweinen/wildschwein_loesung.ipynb
[37_Dreiecksbeziehungen]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/37_Dreiecksbeziehungen/dreiecke_loesung.ipynb
[37_LisaRennt]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/37_LisaRennt/lisarennt_loesung.ipynb
[37_SchachDemWildschwein]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/37_SchachDemWildschwein/schach_loesung.ipynb
[38_Abbiegen]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/38_Abbiegen/abbiegen_loesung.ipynb
[38_Geburtstag]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/38_Geburtstag/geburtstag_loesung.ipynb
[38_Stromrallye]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/38_Stromrallye/stromrallye_loesung.ipynb
[39_Eisbudendilemma]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/39_Eisbudendilemma/eisbuden_loesung.ipynb
[39_FlohmarktInLangdorf]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/39_FlohmarktInLangdorf/flohmarkt_loesung.ipynb
[39_Spiessgesellen]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/39_Spiessgesellen/spiesse_loesung.ipynb
[40_HexMax]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/40_HexMax/hexmax_loesung.ipynb
[40_Muellabfuhr]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/40_Muellabfuhr/muellabfuhr_loesung.ipynb
[40_Rechenraetsel]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/40_Rechenraetsel/rechenraetsel_loesung.ipynb
[40_ZaraZackigsZurueckkehr]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/40_ZaraZackigsZurueckkehr/zarazackig_loesung.ipynb
[41_AllesKaese]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/41_AllesKaese/kaese_loesung.ipynb
[41_PancakeSort]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/41_PancakeSort/pancake_loesung.ipynb
[41_WenigerKrummeTouren]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/41_WenigerKrummeTouren/touren_loesung.ipynb
[42_DieSiedler]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/42_DieSiedler/siedler_loesung.ipynb
[42_Laubmaschen]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/42_Laubmaschen/laubmaschen_loesung.ipynb
[42_StilvollePaeckchen]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/42_StilvollePaeckchen/paeckchen_loesung.ipynb
[43_Konfetti]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/43_Konfetti/konfetti_loesung.ipynb
[43_Schmucknachrichten]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/43_Schmucknachrichten/schmucknachrichten_loesung.ipynb
[43_SimultaneLabyrinthe]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/43_SimultaneLabyrinthe/simultanelabyrinthe_loesung.ipynb
[44_Giessroboter]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/44_Giessroboter/giessroboter_loesung.ipynb
[44_Lieferkette]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/44_Lieferkette/lieferkette_loesung.ipynb
[44_Transformers]: https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf2/44_Transformers/transformers_loesung.ipynb
