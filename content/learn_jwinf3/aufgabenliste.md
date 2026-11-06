# Die Junioraufgaben von 2011 bis 2025: Überblick und Schwierigkeit

Hier stehen alle 30 Junioraufgaben aus den Jahren 2011 bis 2025 (30. bis 44. Bundeswettbewerb Informatik; ab 2018 sind sie
zugleich die 3. Runde des Jugendwettbewerbs). Zu jeder Aufgabe findest du:

- **worum es geht** (in einem Satz),
- welche **Werkzeuge** du brauchst und in welchen Notebooks dieses Lehrgangs sie vorkommen,
- wo die typische **Stolperstelle** liegt,
- eine Einschätzung der **Schwierigkeit**,
- einen Link auf das **Lösungsnotebook** im Ordner `jwinf3`.

## Wie die Schwierigkeit eingeschätzt ist

Objektive Maßstäbe gibt es nicht. Die Sterne sind eine Einschätzung, die sich danach richtet, wie viele Werkzeuge man
kombinieren muss, wie viel man selbst modellieren und entscheiden muss und wie viele Fallen es gibt:

| Sterne | Bedeutung |
|---|---|
| ★ | Die Aufgabe ist offen gestellt, aber schon mit wenigen Grundlagen gut lösbar. |
| ★★ | Ein klares Verfahren mit Werkzeugen aus Phase A und B (Notebooks 1 bis 16), dazu ein, zwei Fallen oder Unklarheiten. |
| ★★★ | Man muss mehrere Werkzeuge verbinden, ein eigenes Maß oder Modell finden, auf Laufzeit oder Sonderfälle achten. |
| ★★★★ | Die Idee ist nicht offensichtlich, oder man braucht Werkzeuge aus Phase C (Suche, Rekursion, Gruppen). |

Was jemandem schwer fällt, ist sehr verschieden. Wer gern mit Texten arbeitet, findet die Silbentrennung vielleicht leichter
als eine Geometrie-Aufgabe, und umgekehrt.

## Überblick

| Schwierigkeit | Aufgabe | Jahr | Kernwerkzeuge |
|---|---|---|---|
| ★ | Passwörter | 2020 | Zufall, Texte zusammensetzen |
| ★★ | Wundertüte | 2023 | `//` und `%`, reihum verteilen |
| ★★ | Bällebad | 2025 | Tabelle (Nutzungsplan), Maximum |
| ★★ | Texthopsen | 2024 | Texte filtern, `while`, Simulation |
| ★★ | Auf und Ab | 2018 | Simulation, Wörterbuch, Endlosschleife erkennen |
| ★★ | Baywatch | 2018 | Rechnen im Kreis, Vergleich mit Lücken |
| ★★ | Parallelen | 2019 | Wörter und Buchstaben zählen, Sprünge |
| ★★ | Zum Winde verweht | 2021 | Abstand, Minimum |
| ★★ | Container | 2022 | Mengen, Ausscheiden |
| ★★ | St. Egano | 2023 | Pixel lesen, `%`, `chr` |
| ★★ | Landnahme | 2015 | Rechtecke überschneiden |
| ★★ | Skyline | 2012 | Abstand Punkt–Rechteck, ganzzahlig rechnen |
| ★★ | Bücherregal | 2017 | Sortieren, gierige Strategie |
| ★★ | Zahlenspiel | 2014 | ggT, alle Möglichkeiten, Zufall |
| ★★ | Songwriter | 2013 | Zufall, Texte nach Regeln bauen |
| ★★ | LAMA | 2016 | Raster, Nachbarn umschalten |
| ★★★ | Treffsicherheit | 2021 | Tabelle, Zählen, eine wichtige Einsicht |
| ★★★ | Quadratisch, praktisch, grün | 2024 | alle Möglichkeiten, Maß festlegen, Laufzeit |
| ★★★ | Silbentrennung | 2025 | Regeln nacheinander, Bewertung, eigene Regeln |
| ★★★ | Reimerei | 2022 | Vokalgruppen, alle Paare oder Gruppieren |
| ★★★ | Baulwürfe | 2020 | Raster, Muster suchen, Doppelzählung |
| ★★★ | Fähre füllen | 2014 | Strategien erfinden und vergleichen |
| ★★★ | Verben | 2012 | Regeln auf Texten, Grenzen zeigen |
| ★★★ | Kassiopeia | 2015 | Erreichbarkeit (Flood Fill) |
| ★★★ | Wintervorrat | 2017 | Simulation im Raster, Zeitlücken |
| ★★★ | Zollstock | 2013 | Modellieren, alle Möglichkeiten, Simulation |
| ★★★ | Rechteckschoner | 2011 | Rekursion, Zeichnen, Zufall |
| ★★★★ | Kacheln | 2019 | Gruppen gleicher Felder, Widersprüche erkennen |
| ★★★★ | Luftballons | 2016 | Simulation einer Maschine, beste Auswahl (Teilmengen) |
| ★★★★ | Glücksrad | 2011 | Wahrscheinlichkeiten, alle Folgen rekursiv, Brüche |

---

## ★ Einstieg

### Passwörter (2020) ★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/39_Passwoerter/passwoerter_loesung.ipynb)

- **Worum es geht:** Ein Generator für zufällige Passwörter, die schwer zu erraten, aber gut auszusprechen sind, nach mindestens
  drei eigenen, begründeten Regeln.
- **Werkzeuge:** `random.choice`, Texte zusammensetzen, Regeln durch Bausteine (Silben aus Konsonant und Vokal) oder durch
  „erzeugen und prüfen“ (Notebook 5, 16).
- **Stolperstelle:** Es gibt keine „richtige“ Lösung. Die Punkte gibt es für gut **begründete** Regeln, und am besten auch für
  eine Abschätzung, wie viele Passwörter möglich sind.

---

## ★★ Klare Verfahren mit Grundwerkzeugen

### Wundertüte (2023) ★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/42_Wundertuete/wundertuete_loesung.ipynb)

- **Worum es geht:** Spiele mehrerer Sorten so auf Tüten verteilen, dass sich die Tüten und jede Sorte um höchstens eins
  unterscheiden.
- **Werkzeuge:** reihum verteilen mit `%`, Listen, Datei lesen, Prüffunktion (Notebook 1, 3, 6, 7, 8).
- **Stolperstelle:** Bei jeder neuen Sorte dort weitermachen, wo die vorige aufgehört hat, nicht wieder bei Tüte 1.

### Bällebad (2025) ★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/44_Baellebad/baellebad_loesung.ipynb)

- **Worum es geht:** Aus einem Stundenplan mit Klassengrößen bestimmen, wie viele Medizinbälle höchstens gleichzeitig gebraucht
  werden und wann.
- **Werkzeuge:** Datei mit Kopfzeile lesen, Tabelle Tag × Stunde füllen, Maximum mit Position, Sonderfälle (Notebook 8, 9, 11, 14).
- **Stolperstelle:** Braucht eine Klasse „von 13 bis 15 Uhr“ um 15 Uhr noch Bälle? Das Beispiel des Aufgabenblatts entscheidet:
  nein (Notebook 23).

### Texthopsen (2024) ★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/43_Texthopsen/texthopsen_loesung.ipynb)

- **Worum es geht:** Zwei Personen hopsen nach den Sprungweiten der Buchstaben durch einen Text. Wer ist zuerst draußen?
- **Werkzeuge:** Text filtern, Wörterbuch für die Sprungweiten, `while`-Schleife, UTF-8 für Umlaute (Notebook 5, 15, 24).
- **Stolperstelle:** Wer gewinnt bei gleich vielen Sprüngen? Die Aufgabe lässt es offen, man muss sich festlegen. Notebook 24
  löst die ganze Aufgabe.

### Auf und Ab (2018) ★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/37_AufUndAb/aufundab_loesung.ipynb)

- **Worum es geht:** Leiterspiel mit 100 Feldern: Kommt man mit immer derselben Augenzahl ins Ziel, und nach wie vielen Würfen?
- **Werkzeuge:** Simulation, Leitern als Wörterbuch, „schon gesehen“ mit einer Menge (Notebook 4, 7, 13, 15).
- **Stolperstelle:** Manche Augenzahlen führen in eine Endlosschleife. Außerdem steht nicht da, wo die Figur startet.

### Baywatch (2018) ★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/37_Baywatch/baywatch_loesung.ipynb)

- **Worum es geht:** Eine vollständige, aber verdrehte Liste der Landzungen einer Insel so drehen, dass sie zu einer lückenhaften
  Liste passt.
- **Werkzeuge:** Rechnen im Kreis (`%`), alle Drehungen ausprobieren, Widerspruch suchen (Notebook 9, 11).
- **Stolperstelle:** Es können **mehrere** Drehungen passen (in den Beispieldateien kommt das vor, einmal passen sogar alle).
  Dann ist die Karte nicht eindeutig. Das Programm sollte außerdem erkennen, wenn gar keine Drehung passt.

### Parallelen (2019) ★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/38_Parallelen/parallelen_loesung.ipynb)

- **Worum es geht:** Im Gedicht von Wort zu Wort springen, je so weit, wie das Wort Buchstaben hat. Endet man immer beim selben
  Wort?
- **Werkzeuge:** Wörter zerlegen, Buchstaben zählen (ohne Satzzeichen), Sprünge simulieren, alle Startwörter prüfen (Notebook 5, 6, 9).
- **Stolperstelle:** „n Wörter weiter“ kann zwei Dinge heißen, und das Ergebnis hängt davon ab (Notebook 23).

### Zum Winde verweht (2021) ★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/40_ZumWindeVerweht/zumwindeverweht_loesung.ipynb)

- **Worum es geht:** Für jeden geplanten Standort einer Windkraftanlage die höchste erlaubte Höhe bestimmen (10-facher Abstand zum
  nächsten Haus).
- **Werkzeuge:** Abstand nach Pythagoras, Minimum suchen, Datei lesen (Notebook 9, 17).
- **Stolperstelle:** Bei „höchstens“ abrunden, nicht runden. Bei großen Dateien wird „jeder Standort gegen jedes Haus“ langsamer.

### Container (2022) ★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/41_Container/container_loesung.ipynb)

- **Worum es geht:** Aus paarweisen Wägungen bestimmen, ob der schwerste Container eindeutig feststeht.
- **Werkzeuge:** Mengen, „wer war nie leichter?“ (Notebook 15), Gegenprobe über Erreichbarkeit (Notebook 21).
- **Stolperstelle:** Die einfache Idee zu finden: Wer einmal leichter war, scheidet aus. Bleibt genau einer übrig, ist es sicher.

### St. Egano (2023) ★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/42_StEgano/stegano_loesung.ipynb)

- **Worum es geht:** Eine geheime Nachricht in Bildern lesen: Jedes Pixel verrät ein Zeichen und den Weg zum nächsten Pixel.
- **Werkzeuge:** Bild lesen (Pillow oder PPM als Text), `chr`, Rechnen im Kreis über den Bildrand (Notebook 5, 11, 20).
- **Stolperstelle:** Das Einlesen der Bilder. Die Regel selbst ist kurz. Bei PNG-Bildern mit vierter Farbe (RGBA) erst umwandeln.

### Landnahme (2015) ★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/34_Landnahme/landnahme_loesung.ipynb)

- **Worum es geht:** Rechteckige Grundstücke der Reihe nach genehmigen, wenn sie sich mit keinem früher genehmigten überschneiden.
- **Werkzeuge:** Strecken und Rechtecke überschneiden, Ecken sortieren mit `min` und `max` (Notebook 17), Zeichnen (Notebook 19).
- **Stolperstelle:** Berühren zählt nicht als Überschneiden (`<` statt `<=`), und man vergleicht nur mit **genehmigten** Rechtecken.

### Skyline (2012) ★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/31_Skyline/skyline_loesung.ipynb)

- **Worum es geht:** Erlaubte Gebäudehöhen abhängig vom kleinsten Abstand des Grundrisses zu einem Turm.
- **Werkzeuge:** Abstand eines Punktes zu einem Rechteck, `math.isqrt` (Notebook 17).
- **Stolperstelle:** Der nächste Punkt ist nicht immer eine Ecke, und Kommazahlen können an den 100-m-Grenzen falsch runden.

### Bücherregal (2017) ★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/36_Buecherregal/buecherregal_loesung.ipynb)

- **Worum es geht:** Bücher so in Abschnitte aufteilen, dass sich die Höhen in jedem Abschnitt um höchstens 3 cm unterscheiden.
  Reichen die Deko-Figuren dafür?
- **Werkzeuge:** Sortieren, gierige Strategie (Notebook 18).
- **Stolperstelle:** Die Dateien geben die Höhen in Millimetern an, nicht in Zentimetern. Und man sollte begründen, warum die
  gierige Strategie die wenigsten Abschnitte findet.

### Zahlenspiel (2014) ★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/33_Zahlenspiel/zahlenspiel_loesung.ipynb)

- **Worum es geht:** Zufällige Übungsaufgaben zum Kürzen von Brüchen in drei Schwierigkeitsstufen erzeugen.
- **Werkzeuge:** ggT (`math.gcd`), Ziffern zählen, alle Brüche durchprobieren, zufällig auswählen (Notebook 4, 10, 16).
- **Stolperstelle:** Alle Bedingungen der Stufen genau einhalten (Länge, Summe von Zähler und Nenner, wirklich kürzbar).

### Songwriter (2013) ★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/32_Songwriter/songwriter_loesung.ipynb)

- **Worum es geht:** Liedtexte aus Silben nach festen Regeln erzeugen (Zeilen, Strophen, Muster), die sich voneinander unterscheiden.
- **Werkzeuge:** Zufall, Funktionen für jede Ebene (Silbe, Zeile, Strophe, Song), Muster mit `%`, Menge gegen Doppelte (Notebook 7, 16).
- **Stolperstelle:** Die vielen Regeln vollständig umsetzen und eine Silbe wie `di` vermeiden, die mit dem angehängten `p di`
  verwechselt werden kann.

### LAMA (2016) ★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/35_LAMA/lama_loesung.ipynb)

- **Worum es geht:** Das Spiel „Lights Out“ programmieren: Ein Tastendruck schaltet ein Lämpchen und seine Nachbarn um. Dazu
  andere Brettgrößen und eine Variante.
- **Werkzeuge:** Raster, Nachbarn mit Randprüfung, Zustand ändern und anzeigen (Notebook 12, 13).
- **Stolperstelle:** Die Aufgabe verlangt ein **interaktives** Spiel mit Eingaben. In JupyterLite simuliert man die Züge besser
  über eine vorgegebene Zugfolge (wie in Notebook 13).

---

## ★★★ Mehrere Werkzeuge, eigene Entscheidungen

### Treffsicherheit (2021) ★★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/40_Treffsicherheit/treffsicherheit_loesung.ipynb)

- **Worum es geht:** Wie viele Einträge einer Bewertungstabelle muss man mindestens ändern, damit ein Termin allen am besten gefällt?
- **Werkzeuge:** Tabelle lesen, für jeden Termin zählen, Minimum (Notebook 9, 11).
- **Stolperstelle:** Die Einsicht, dass jedes Mitglied, das einen anderen Termin lieber hat, **genau eine** Änderung kostet. Wer das
  nicht sieht, probiert viel zu kompliziert herum.

### Quadratisch, praktisch, grün (2024) ★★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/43_QuadratischPraktischGr%C3%BCn/quadratisch_praktisch_gruen_loesung.ipynb)

- **Worum es geht:** Ein Grundstück in mindestens so viele gleich große Gärten aufteilen, wie es Interessenten gibt (höchstens 10 %
  mehr), die möglichst quadratisch sind.
- **Werkzeuge:** zwei Schleifen über Reihen und Spalten, das Beste merken, `k * 11 // 10` (Notebook 9, 10).
- **Stolperstelle:** „So quadratisch wie möglich“ selbst festlegen und begründen, und die Schleifen so begrenzen, dass das größte
  Beispiel (35 000 Interessenten) nicht ewig dauert.

### Silbentrennung (2025) ★★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/44_Silbentrennung/silbentrennung_loesung.ipynb)

- **Worum es geht:** Silbentrennung nach vorgegebenen Regeln, dann eigene, bessere Regeln finden und die Leistung bewerten.
- **Werkzeuge:** Begriffe als Funktionen, Regeln nacheinander (die letzte gewinnt), Bewertung gegen eine Referenz (Notebook 5, 14).
- **Stolperstelle:** Die Aufgabe ist **offen**: Man muss selbst Verbesserungen finden und messen. Ohne Bewertung lässt sich nicht
  zeigen, dass eine Regel hilft.

### Reimerei (2022) ★★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/41_Reimerei/reimerei_loesung.ipynb)

- **Worum es geht:** In einer Wortliste alle Reimpaare nach drei genau definierten Regeln finden (Vokalgruppen).
- **Werkzeuge:** Texte zerlegen, Vokalgruppen bestimmen, alle Paare (Notebook 10) oder Gruppieren mit einem Wörterbuch (Notebook 15).
- **Stolperstelle:** Die Regeln sind lang und genau. Man muss jede Regel einzeln umsetzen und an den Beispielen der Aufgabe testen.

### Baulwürfe (2020) ★★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/39_Baulwuerfe/baulwuerfe_loesung.ipynb)

- **Worum es geht:** Auf einer Hügelkarte rechteckige Baue in einem festen Muster zählen.
- **Werkzeuge:** Rasterdatei lesen (Leerzeichen erhalten!), Muster an jeder Stelle prüfen, benutzte Felder merken (Notebook 12).
- **Stolperstelle:** Aneinanderstoßende Baue erzeugen „scheinbare“ Baue. Ob man sie mitzählt, ist eine Frage der Lesart.

### Fähre füllen (2014) ★★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/33_FaehreFuellen/faehrefuellen_loesung.ipynb)

- **Worum es geht:** Zwei einfache Strategien zum Beladen einer Fähre finden, von denen mal die eine, mal die andere besser ist.
- **Werkzeuge:** Simulation, Strategie als Parameter, Vergleichstabelle, ganzzahlig in Zentimetern (Notebook 17, 18).
- **Stolperstelle:** Man muss selbst ein Beispiel **konstruieren**, bei dem die zweite Strategie gewinnt.

### Verben (2012) ★★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/31_Verben/verben_loesung.ipynb)

- **Worum es geht:** Aus einer Verbform mit Regeln die Grundform bestimmen („sagst“ → „sagen“).
- **Werkzeuge:** `startswith`, `endswith`, Ausschnitte, Reihenfolge der Regeln, Testtabelle (Notebook 5, 14).
- **Stolperstelle:** Die deutsche Sprache hat viele Ausnahmen. Die Aufgabe verlangt ausdrücklich, auch zu zeigen, was **nicht** klappt.

### Kassiopeia (2015) ★★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/34_Kassiopeia/kassiopeia_loesung.ipynb)

- **Worum es geht:** Kann eine Schildkröte alle weißen Felder ihres Landes erreichen?
- **Werkzeuge:** Rasterdatei lesen, Flood Fill mit Stapel und Menge (Notebook 12, 21).
- **Stolperstelle:** Ohne Flood Fill kommt man nicht weit. Mit Flood Fill ist die Aufgabe kurz. Eine Beispieldatei ist leer.

### Wintervorrat (2017) ★★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/36_Wintervorrat/wintervorrat_loesung.ipynb)

- **Worum es geht:** Raubvögel fliegen über einen Rechteckwald hin und her. Welche Felder werden nie überflogen, welche haben
  30 Minuten am Stück Ruhe?
- **Werkzeuge:** Simulation Minute für Minute, Raster mit Listen, längste Lücke finden (Notebook 11, 13, 19).
- **Stolperstelle:** Die Bedeutung der Koordinaten (wo ist Norden?) und Grenzfälle bei Zeiträumen. Hier hilft die mitgelieferte
  erwartete Ausgabe zum ersten Beispiel.

### Zollstock (2013) ★★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/32_Zollstock/zollstock_loesung.ipynb)

- **Worum es geht:** Wie viele verschiedene Arten gibt es, einen Zollstock so zu falten, dass er in einen kurzen Beutel passt?
  Reichen sie für zwei Monate?
- **Werkzeuge:** Modellieren (jedes Gelenk gefaltet oder nicht), alle 512 Möglichkeiten erzeugen, jede simulieren (Notebook 10, 13, 22).
- **Stolperstelle:** Die Aufgabe enthält **kein** Programmierverfahren. Man muss selbst erkennen, wie man „Faltung“ als Daten
  darstellt und was „verschieden“ heißt.

### Rechteckschoner (2011) ★★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/30_Rechteckschoner/rechteckschoner_loesung.ipynb)

- **Worum es geht:** Ein Bildschirmschoner aus ineinander geschachtelten Rechtecken, die sich nach und nach zufällig verändern.
- **Werkzeuge:** Rekursion, Zufall, Zeichnen (Notebook 16, 19, 22).
- **Stolperstelle:** Die Rechtecke als Baum speichern, damit man später ein Teilrechteck gezielt verändern kann.

---

## ★★★★ Für Fortgeschrittene

### Kacheln (2019) ★★★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/38_Kacheln/kacheln_loesung.ipynb)

- **Worum es geht:** Eine Landschaft aus Kacheln mit Wasser und Land so vervollständigen, dass überall Land an Land und Wasser an
  Wasser grenzt, oder erkennen, dass es nicht geht.
- **Werkzeuge:** Raster, Gruppen von Feldern, die gleich sein müssen (Flood Fill, Notebook 21), Prüffunktion (Notebook 14).
- **Stolperstelle:** Die Einsicht, welche Viertel einer Kachel mit welchen Vierteln der Nachbarn übereinstimmen müssen. Danach ist
  es eine Gruppenaufgabe. Widersprüche innerhalb einer Gruppe bedeuten „unmöglich“.

### Luftballons (2016) ★★★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/35_Luftballons/luftballons_loesung.ipynb)

- **Worum es geht:** Eine Verpackungsmaschine mit 10 Fächern so steuern, dass jede Packung mindestens 20 und möglichst genau
  20 Luftballons enthält.
- **Werkzeuge:** Simulation der Maschine, beste Auswahl von Fächern (alle 1024 Teilmengen, Notebook 22), Füllfolge abarbeiten.
- **Stolperstelle:** Nach jedem Entleeren werden Fächer neu gefüllt. Darum muss man nach jedem Schritt neu entscheiden. Wie die
  zehn leeren Fächer am Anfang gefüllt werden, sagt die Aufgabe nicht genau. Das muss man festlegen (naheliegend: mit den ersten
  zehn Zahlen der Füllfolge).

### Glücksrad (2011) ★★★★
[Lösungsnotebook](https://ktheu.github.io/bwinfN/notebooks/index.html?path=jwinf3/30_Gluecksrad/gluecksrad_loesung.ipynb)

- **Worum es geht:** Wie wahrscheinlich ist es, mit sechs Drehungen eines Glücksrads jedes Feld genau einmal zu erreichen?
- **Werkzeuge:** alle Folgen rekursiv durchgehen, Wahrscheinlichkeiten multiplizieren, exakte Brüche, Zwischenergebnisse merken
  (Notebook 22).
- **Stolperstelle:** Die Mathematik: Wahrscheinlichkeiten einer Folge multiplizieren, die aller Folgen addieren. Und das Startfeld
  zählt erst, wenn man wieder dort ankommt.

---

## Vorschlag für eine Reihenfolge

1. **Zum Einstieg** (nach Phase A): Wundertüte, Bällebad, Texthopsen, am besten mit Notebook 24 als Anleitung.
2. **Nach Phase B**: die übrigen ★★-Aufgaben, zum Beispiel Auf und Ab, Baywatch, Container, Zum Winde verweht, Parallelen.
3. **Dann** die ★★★-Aufgaben. Quadratisch, praktisch, grün und Silbentrennung sind gute Übungen für **offene** Aufgaben, bei denen
   man selbst festlegen und begründen muss. Das ist in den letzten Jahren typisch geworden.
4. **Zum Schluss**, wer mag: die ★★★★-Aufgaben.

Bearbeite eine Aufgabe zuerst **selbst** (mit Notebook 23 und 24 als Anleitung) und sieh dir das Lösungsnotebook erst danach an.
