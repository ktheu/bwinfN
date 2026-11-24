# Python für die 1. Runde des Bundeswettbewerbs Informatik

[← zur Startseite](readme.md)

Hier entstehen Lösungsnotebooks zu den Aufgaben 1 bis 5 der 1. Runde des Bundeswettbewerbs Informatik. Die Junioraufgaben
der 1. Runde stehen auf der Seite [Jugendwettbewerb, 3. Runde](jwinf3.md), denn sie sind zugleich die Aufgaben der 3. Runde
des Jugendwettbewerbs.

Jedes Lösungsnotebook enthält den Aufgabentext, die nützlichen Werkzeuge (Algorithmen und Python-Funktionen), die Lösungsidee
und eine Schritt-für-Schritt-Lösung mit allen Beispielen. Zuerst kommt immer eine einfache, gut nachvollziehbare Lösung,
schnellere Verfahren stehen am Ende unter „Für Neugierige“. **Bearbeite eine Aufgabe zuerst selbst** und sieh dir das
Lösungsnotebook erst danach an.

Welche Aufgaben welches Verfahren brauchen und in welcher Reihenfolge man sie üben kann, steht in der Übersicht
**[Werkzeuge für die 1. Runde](https://github.com/ktheu/bwinfN/blob/main/content/bwinf1/werkzeuge.md)**.

Die Notebooks laufen direkt im Browser mit [JupyterLite](https://jupyterlite.readthedocs.io/). Eine Codezelle führst du mit
**Umschalt + Enter** aus.

Einige Notebooks zeigen am Ende zusätzlich eine Lösung mit **MiniZinc**. Die MiniZinc-Modelle laufen nicht im Browser-Python,
sondern in der [MiniZinc IDE](https://www.minizinc.org/) oder im [MiniZinc Playground](https://play.minizinc.org/). Wie man mit
MiniZinc arbeitet, zeigen die Arbeitsblätter
[Grundlagen](https://ktheu.github.io/python-uebungen/notebooks/index.html?path=minizinc_grundlagen.ipynb),
[Daten](https://ktheu.github.io/python-uebungen/notebooks/index.html?path=minizinc_daten.ipynb) und
[Zuordnen und Planen](https://ktheu.github.io/python-uebungen/notebooks/index.html?path=minizinc_zuordnung.ipynb).

## Der Lehrgang: Algorithmen für die 1. Runde

Jedes Notebook stellt ein Werkzeug an einfachen Beispielen vor und endet mit einer **Wettbewerbs-Ecke**: einer
verkleinerten Fassung einer echten Aufgabe der 1. Runde. Voraussetzung ist der
[Lehrgang zum Jugendwettbewerb](jwinf3.md) (mindestens Phase A und B, dazu die Notebooks 18, 21 und 22). Unter jeder Aufgabe
kannst du zuerst einen Tipp und dann die Lösung aufklappen. Weitere Notebooks folgen.

| Nr | Notebook | Inhalt | Wettbewerbs-Ecke |
|---|---|---|---|
| 01 | [Alle Möglichkeiten durchprobieren](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/01_durchprobieren.ipynb) | `itertools.product`, `permutations`, `combinations`, Anzahlen ausrechnen, O-Notation | Alphametiken, Nandu |
| 02 | [Backtracking](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/02_backtracking.ipynb) | Setzen und zurücknehmen, früh abbrechen, Aufrufe zählen, alle Lösungen oder die erste | Dreieckspuzzle, Kassiopeias Weg |
| 03 | [Schranken und Symmetrien](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/03_schranken_symmetrien.ipynb) | Beste Lösung merken, Schranke (Branch and Bound), `sorted` mit `key=lambda`, Symmetrie brechen, Normalform von Figuren | Blumenbeet, Rominos |
| 04 | [Logisch schließen](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/04_logisch_schliessen.ipynb) | Kandidaten, Regeln bis nichts mehr geht, Widersprüche, raten und wieder schließen, Eindeutigkeit, drei Zustände | Sudoku, Bibertomograph |
| 05 | [Breitensuche](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/05_breitensuche.ipynb) | Graph als Wörterbuch, `deque`, beim Einreihen markieren, Vorgänger und Weg, Raster als Graph | Zauberschule, Arukone |
| 06 | [Zustände](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/06_zustaende.ipynb) | Zustände als Tupel, Nachfolger, Breitensuche über Zustände, Normalform, Größe des Zustandsraums, „nicht lösbar“ beweisen | Faires Füllen, Hüpfburg |
| 07 | [Dijkstra](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/07_dijkstra.ipynb) | Gewichtete Kanten, `heapq`, veraltete Einträge überspringen, Weg zurückverfolgen, Zwischenknoten, Zustände mit Kosten | Zauberschule, Ägyptisches Grabmal |
| 10 | [Merken](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/10_merken.ipynb) | Memoisierung mit Wörterbuch und Tupeln als Schlüssel, Aufrufe zählen, beste Lösung zurückverfolgen, `@lru_cache` | Schwimmbad, Nummernmerker |
| 11 | [Tabellen](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/11_tabellen_dp.ipynb) | Von der Rekursion zur Tabelle, Münzwechsel, Wort in Wörter zerlegen, Präfixsummen | Auto-Scrabble, Voll daneben |
| 12 | [Greedy](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/12_greedy.ipynb) | Gierige Wahl mit Begründung, Gegenbeispiele durch Vergleich mit Durchprobieren, Termine planen, Wechselgeld | Urlaubsfahrt, Frühsport |
| 13 | [Binäre Suche](https://ktheu.github.io/bwinfN/notebooks/index.html?path=learn_bwinf1/13_binaere_suche.ipynb) | Binäre Suche selbst und mit `bisect`, Zielwert raten und prüfen, Meet in the Middle | Vollgeladen, Marktwaage |

## Die Lösungsnotebooks

| BwInf | Aufgabe | Kernwerkzeuge | Lösungsnotebook |
|---|---|---|---|
| 44. (2025/26) | Aufgabe 1: Drehfreudig? | Bäume, Klammerfolgen | [drehfreudig_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/44_Drehfreudig/drehfreudig_loesung.ipynb) |
| 44. (2025/26) | Aufgabe 2: ChoreoGraph | Permutationen, Backtracking | [choreograph_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/44_ChoreoGraph/choreograph_loesung.ipynb) |
| 44. (2025/26) | Aufgabe 3: Nasser Hund | Abstände Strecke–Strecke | [nasserhund_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/44_NasserHund/nasserhund_loesung.ipynb) |
| 44. (2025/26) | Aufgabe 4: Bibertomograph | logisches Schließen, Backtracking | [bibertomograph_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/44_Bibertomograph/bibertomograph_loesung.ipynb) |
| 44. (2025/26) | Aufgabe 5: Großstadtbauern | Backtracking, Branch and Bound | [grossstadtbauern_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/44_Grossstadtbauern/grossstadtbauern_loesung.ipynb) |
| 43. (2024/25) | Aufgabe 1: Hopsitexte | Simulation, Backtracking | [hopsitexte_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/43_Hopsitexte/hopsitexte_loesung.ipynb) |
| 43. (2024/25) | Aufgabe 2: Schwierigkeiten | Graph, topologische Sortierung | [schwierigkeiten_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/43_Schwierigkeiten/schwierigkeiten_loesung.ipynb) |
| 43. (2024/25) | Aufgabe 3: Wandertag | Intervalle, dynamische Programmierung | [wandertag_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/43_Wandertag/wandertag_loesung.ipynb) |
| 43. (2024/25) | Aufgabe 4: Krocket | Geraden, Schnittpunkte | [krocket_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/43_Krocket/krocket_loesung.ipynb) |
| 43. (2024/25) | Aufgabe 5: Das ägyptische Grabmal | Zustände mit Zeit, Dijkstra | [aegyptischesgrabmal_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/43_AegyptischesGrabmal/aegyptischesgrabmal_loesung.ipynb) |
| 42. (2023/24) | Aufgabe 1: Arukone | Breitensuche, Backtracking | [arukone_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/42_Arukone/arukone_loesung.ipynb) |
| 42. (2023/24) | Aufgabe 2: Die goldene Mitte | Backtracking, erste freie Stelle | [goldene_mitte_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/42_DieGoldeneMitte/goldene_mitte_loesung.ipynb) |
| 42. (2023/24) | Aufgabe 3: Zauberschule | Breitensuche, Dijkstra | [zauberschule_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/42_Zauberschule/zauberschule_loesung.ipynb) |
| 42. (2023/24) | Aufgabe 4: Nandu | Simulation, Wahrheitstabelle | [nandu_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/42_Nandu/nandu_loesung.ipynb) |
| 42. (2023/24) | Aufgabe 5: Stadtführung | Modellieren, dynamische Programmierung | [stadtfuehrung_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/42_Stadtfuehrung/stadtfuehrung_loesung.ipynb) |
| 41. (2022/23) | Aufgabe 1: Störung | Textsuche, Tokenisieren | [stoerung_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/41_Stoerung/stoerung_loesung.ipynb) |
| 41. (2022/23) | Aufgabe 2: Verzinkt | Ereignisse mit heapq, Zufall | [verzinkt_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/41_Verzinkt/verzinkt_loesung.ipynb) |
| 41. (2022/23) | Aufgabe 3: Sudokopie | Durchprobieren, Invarianten | [sudokopie_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/41_Sudokopie/sudokopie_loesung.ipynb) |
| 41. (2022/23) | Aufgabe 4: Fahrradwerkstatt | Ereignissimulation, Kennzahlen | [fahrradwerkstatt_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/41_Fahrradwerkstatt/fahrradwerkstatt_loesung.ipynb) |
| 41. (2022/23) | Aufgabe 5: Hüpfburg | Breitensuche über Paare | [huepfburg_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/41_Huepfburg/huepfburg_loesung.ipynb) |
| 40. (2021/22) | Aufgabe 1: Schiebeparkplatz | Rekursion, Tupel vergleichen | [schiebeparkplatz_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/40_Schiebeparkplatz/schiebeparkplatz_loesung.ipynb) |
| 40. (2021/22) | Aufgabe 2: Vollgeladen | Greedy, binäre Suche | [vollgeladen_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/40_Vollgeladen/vollgeladen_loesung.ipynb) |
| 40. (2021/22) | Aufgabe 3: Wortsuche | Zufall mit Neustart | [wortsuche_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/40_Wortsuche/wortsuche_loesung.ipynb) |
| 40. (2021/22) | Aufgabe 4: Würfelglück | Simulation, Monte-Carlo | [wuerfelglueck_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/40_Wuerfelglueck/wuerfelglueck_loesung.ipynb) |
| 40. (2021/22) | Aufgabe 5: Marktwaage | binäre Suche, Meet in the Middle | [marktwaage_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/40_Marktwaage/marktwaage_loesung.ipynb) |
| 39. (2020/21) | Aufgabe 1: Wörter aufräumen | Matching, Backtracking | [woerteraufraeumen_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/39_WoerterAufraeumen/woerteraufraeumen_loesung.ipynb) |
| 39. (2020/21) | Aufgabe 2: Dreieckspuzzle | Backtracking, Drehen mit Modulo | [dreieckspuzzle_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/39_Dreieckspuzzle/dreieckspuzzle_loesung.ipynb) |
| 39. (2020/21) | Aufgabe 3: Tobis Turnier | Monte-Carlo, Wahrscheinlichkeiten | [tobisturnier_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/39_TobisTurnier/tobisturnier_loesung.ipynb) |
| 39. (2020/21) | Aufgabe 4: Streichholzrätsel | Darstellung, Durchprobieren | [streichholzraetsel_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/39_Streichholzraetsel/streichholzraetsel_loesung.ipynb) |
| 39. (2020/21) | Aufgabe 5: Wichteln | Matching, verbessernde Wege | [wichteln_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/39_Wichteln/wichteln_loesung.ipynb) |
| 38. (2019/20) | Aufgabe 1: Blumenbeet | Backtracking, Branch and Bound | [blumenbeet_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/38_Blumenbeet/blumenbeet_loesung.ipynb) |
| 38. (2019/20) | Aufgabe 2: Nummernmerker | Memoisierung, kürzeste Wege | [nummernmerker_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/38_Nummernmerker/nummernmerker_loesung.ipynb) |
| 38. (2019/20) | Aufgabe 3: Telepaartie | Breitensuche, Normalform | [telepaartie_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/38_Telepaartie/telepaartie_loesung.ipynb) |
| 38. (2019/20) | Aufgabe 4: Urlaubsfahrt | Greedy, dynamische Programmierung | [urlaubsfahrt_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/38_Urlaubsfahrt/urlaubsfahrt_loesung.ipynb) |
| 38. (2019/20) | Aufgabe 5: Rominos | Backtracking, Symmetrien | [rominos_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/38_Rominos/rominos_loesung.ipynb) |
| 37. (2018/19) | Aufgabe 1: Superstar | Ausschließen, Kandidat prüfen | [superstar_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/37_Superstar/superstar_loesung.ipynb) |
| 37. (2018/19) | Aufgabe 2: Twist | Mischen, Normalform | [twist_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/37_Twist/twist_loesung.ipynb) |
| 37. (2018/19) | Aufgabe 3: Voll daneben | dynamische Programmierung, Präfixsummen | [voll_daneben_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/37_VollDaneben/voll_daneben_loesung.ipynb) |
| 37. (2018/19) | Aufgabe 4: Schrebergärten | Backtracking, untere Schranke | [schrebergaerten_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/37_Schrebergaerten/schrebergaerten_loesung.ipynb) |
| 37. (2018/19) | Aufgabe 5: Widerstand | Bäume, Rekursion | [widerstand_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/37_Widerstand/widerstand_loesung.ipynb) |
| 36. (2017/18) | Aufgabe 1: Zimmerbelegung | zwingende Folgerungen, Flutfüllen | [zimmerbelegung_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/36_Zimmerbelegung/zimmerbelegung_loesung.ipynb) |
| 36. (2017/18) | Aufgabe 2: Schwimmbad | Rekursion mit Memoisierung | [schwimmbad_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/36_Schwimmbad/schwimmbad_loesung.ipynb) |
| 36. (2017/18) | Aufgabe 3: Dreiecke zählen | Schnittpunkte, Kommazahlen | [dreieckezaehlen_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/36_DreieckeZaehlen/dreieckezaehlen_loesung.ipynb) |
| 36. (2017/18) | Aufgabe 4: Auto-Scrabble | dynamische Programmierung, Mengen | [autoscrabble_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/36_AutoScrabble/autoscrabble_loesung.ipynb) |
| 36. (2017/18) | Aufgabe 5: Bauernopfer | Invariante, Spielgraph | [bauernopfer_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/36_Bauernopfer/bauernopfer_loesung.ipynb) |
| 35. (2016/17) | Aufgabe 1: Sprichwort | Datum umrechnen, lineare Suche | [sprichwort_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/35_Sprichwort/sprichwort_loesung.ipynb) |
| 35. (2016/17) | Aufgabe 2: Rhinozelfant | Bilder, Nachbarpixel | [rhinozelfant_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/35_Rhinozelfant/rhinozelfant_loesung.ipynb) |
| 35. (2016/17) | Aufgabe 3: Rotation | Breitensuche über Zustände | [rotation_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/35_Rotation/rotation_loesung.ipynb) |
| 35. (2016/17) | Aufgabe 4: Radfahrspaß | Menge von Zuständen, Klammerfolgen | [radfahrspass_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/35_Radfahrspass/radfahrspass_loesung.ipynb) |
| 35. (2016/17) | Aufgabe 5: Buhnenrennen | kürzeste Wege, dynamische Programmierung | [buhnenrennen_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/35_Buhnenrennen/buhnenrennen_loesung.ipynb) |
| 34. (2015/16) | Aufgabe 1: Kassiopeias Weg | Backtracking, Schachbrettfärbung | [kassiopeiasweg_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/34_KassiopeiasWeg/kassiopeiasweg_loesung.ipynb) |
| 34. (2015/16) | Aufgabe 2: Ameisenfutter | Simulation in Ticks, Zufall | [ameisenfutter_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/34_Ameisenfutter/ameisenfutter_loesung.ipynb) |
| 34. (2015/16) | Aufgabe 3: Flaschenzug | Rekursion, dynamische Programmierung | [flaschenzug_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/34_Flaschenzug/flaschenzug_loesung.ipynb) |
| 34. (2015/16) | Aufgabe 4: Schlüssellöcher | Hamming-Abstand, lokale Suche | [schluesselloecher_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/34_Schluesselloecher/schluesselloecher_loesung.ipynb) |
| 34. (2015/16) | Aufgabe 5: Groker | Spieltheorie, gemischte Strategie | [groker_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/34_Groker/groker_loesung.ipynb) |
| 33. (2014/15) | Aufgabe 1: Faires Füllen | Breitensuche über Zustände | [fairesfuellen_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/33_FairesFuellen/fairesfuellen_loesung.ipynb) |
| 33. (2014/15) | Aufgabe 2: Mobile | Bäume, Rekursion | [mobile_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/33_Mobile/mobile_loesung.ipynb) |
| 33. (2014/15) | Aufgabe 3: Buffet-Lotterie | Simulation im Kreis | [buffetlotterie_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/33_BuffetLotterie/buffetlotterie_loesung.ipynb) |
| 33. (2014/15) | Aufgabe 4: Alphametiken | Durchprobieren, Backtracking | [alphametiken_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/33_Alphametiken/alphametiken_loesung.ipynb) |
| 33. (2014/15) | Aufgabe 5: Pong | Simulation, Spiegeln | [pong_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/33_Pong/pong_loesung.ipynb) |
| 32. (2013/14) | Aufgabe 1: Rationalisierung | Euklid, Durchprobieren | [rationalisierung_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/32_Rationalisierung/rationalisierung_loesung.ipynb) |
| 32. (2013/14) | Aufgabe 2: Tutorien | Matching, Kombinatorik | [tutorien_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/32_Tutorien/tutorien_loesung.ipynb) |
| 32. (2013/14) | Aufgabe 3: Vortänzer | Klammerfolgen, Simulation | [vortaenzer_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/32_Vortaenzer/vortaenzer_loesung.ipynb) |
| 32. (2013/14) | Aufgabe 4: Fotoforensik | Bilder mit numpy, Korrelation | [fotoforensik_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/32_Fotoforensik/fotoforensik_loesung.ipynb) |
| 32. (2013/14) | Aufgabe 5: Versteigerung | Strategien, Simulation | [versteigerung_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/32_Versteigerung/versteigerung_loesung.ipynb) |
| 31. (2012/13) | Aufgabe 1: Frühsport | Invariante, Greedy | [fruehsport_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/31_Fruehsport/fruehsport_loesung.ipynb) |
| 31. (2012/13) | Aufgabe 2: Geldtransporter | Backtracking, Branch and Bound | [geldtransporter_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/31_Geldtransporter/geldtransporter_loesung.ipynb) |
| 31. (2012/13) | Aufgabe 3: Turn 90 | Pledge-Algorithmus, Simulation | [turn90_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/31_Turn90/turn90_loesung.ipynb) |
| 31. (2012/13) | Aufgabe 4: SVG-Fraktale | Ersetzungsregel, Vektoren | [svgfraktale_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/31_SVGFraktale/svgfraktale_loesung.ipynb) |
| 31. (2012/13) | Aufgabe 5: Kaffeerunde | Simulation, Zufall | [kaffeerunde_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/31_Kaffeerunde/kaffeerunde_loesung.ipynb) |
| 30. (2011/12) | Aufgabe 1: Wer spielt fair? | Hash-Funktion, Festlegen ohne Verraten | [werspieltfair_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/30_WerSpieltFair/werspieltfair_loesung.ipynb) |
| 30. (2011/12) | Aufgabe 2: Aladins Lampen | Rechnen modulo 2, Gauß-Verfahren | [aladinslampen_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/30_AladinsLampen/aladinslampen_loesung.ipynb) |
| 30. (2011/12) | Aufgabe 3: Fehlerfrei puzzeln | Simulated Annealing, logisches Schließen | [fehlerfreipuzzeln_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/30_FehlerfreiPuzzeln/fehlerfreipuzzeln_loesung.ipynb) |
| 30. (2011/12) | Aufgabe 4: Zaras dritter Fehler | Präfixsummen, dynamische Programmierung | [zarasdritterfehler_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/30_ZarasDritterFehler/zarasdritterfehler_loesung.ipynb) |
| 30. (2011/12) | Aufgabe 5: Städtepartner | Matching, verbessernde Wege | [staedtepartner_loesung.ipynb](https://ktheu.github.io/bwinfN/notebooks/index.html?path=bwinf1/30_Staedtepartner/staedtepartner_loesung.ipynb) |

Die Aufgaben des laufenden Wettbewerbs sind absichtlich nicht dabei.

Die Spalte „Kernwerkzeuge“ nennt die wichtigsten Verfahren jeder Aufgabe. Die Übersicht
**[Werkzeuge für die 1. Runde](https://github.com/ktheu/bwinfN/blob/main/content/bwinf1/werkzeuge.md)** ordnet alle Aufgaben
nach Werkzeugen (Suchen, Graphen, dynamische Programmierung, Simulation, Geometrie, Mathematik, Python-Bibliotheken,
MiniZinc) und schlägt eine Reihenfolge zum Üben vor.

[← zur Startseite](readme.md)
