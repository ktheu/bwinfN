# Von Blockly zu Python: Übersetzungstabelle

Die Blöcke stammen aus der Blockly-Umgebung des Jugendwettbewerbs Informatik (Bildschirmfotos aus der Werkzeugleiste).
Werte in Blöcken wie `10` oder `i` sind Beispiele. Die Auswahlmenüs (▾) sind ebenfalls aus der
JwInf-Umgebung übernommen.

**Wichtigster Unterschied:** In Blockly zählt man Buchstaben und Listenplätze ab **1**, in Python ab **0**.
Der 1. Buchstabe von `text` ist in Python `text[0]`.

## Ausgeben und Eingabe (rot)

| Blockly | Python | Notebook |
|---|---|---|
| schreibe … | `print(…)` | 01 |
| lies Zeile als ganze Zahl | `int(input())` (bzw. eine Zeile aus einer Datei) | 08 |
| lies Zeile als Text | `input()` | 08 |
| lies Zeile als Zahl | `float(input())` | 08 |
| Ende der Eingabe | keine Zeile mehr übrig: Python liest stattdessen alle Zeilen einer Datei auf einmal | 08 |

Im Lehrgang (JupyterLite) lesen wir aus **Dateien** statt mit `input()`.

## Umwandeln (gelb)

| Blockly | Python | Notebook |
|---|---|---|
| Text zu Zahl | `int(text)` (ganze Zahl) oder `float(text)` (Kommazahl) | 01 |
| Zahl zu Zeichen | `chr(65)` → `'A'` | 05 |
| Zeichen zu Zahl | `ord('A')` → `65` | 05 |
| (kein Block) | `str(7)` → `'7'` | 01 |

## Logik (grün)

| Blockly | Python | Notebook |
|---|---|---|
| falls … mache … (über ⚙ „sonst falls“ und „sonst“ anbauen) | `if …:` / `elif …:` / `else:` | 02 |
| … = … (Auswahl: = ≠ < ≤ > ≥) | `==` `!=` `<` `<=` `>` `>=` | 02 |
| … und … (Auswahl: und, oder) | `and`, `or` | 02 |
| nicht … | `not …` | 02 |
| wahr (Auswahl: wahr, unwahr) | `True`, `False` | 02 |
| null | `None` | 07 |
| prüfe … falls wahr … falls unwahr … | `a if bedingung else b` | 02 (Für Profis) |

## Schleifen (türkis)

| Blockly | Python | Notebook |
|---|---|---|
| wiederhole 10 mal: mache … | `for _ in range(10):` | 03 |
| wiederhole solange … mache … | `while …:` | 04 |
| zähle i von 1 bis 10 in Schritten von 1: mache … | `for i in range(1, 11):` (**bis 10 einschließlich** → `range(1, 11)`) | 03 |
| zähle i von 1 bis 10 in Schritten von 2 | `for i in range(1, 11, 2):` | 03 |
| für jeden Wert i aus der Liste … mache … | `for i in liste:` | 06 |
| die Schleife abbrechen | `break` | 04 |

## Mathematik (blau)

| Blockly | Python | Notebook |
|---|---|---|
| 0 (Zahl) | `0`, Kommazahlen mit Punkt: `3.5` | 01 |
| 1 + 1 (Auswahl: + - × ÷ ^) | `+` `-` `*` `/` `**` | 01 |
| (kein Block) | `//` ganzzahlig teilen | 01 |
| Rest von 64 ÷ 10 | `64 % 10` | 01 |
| Quadratwurzel 9 | `math.sqrt(9)` (vorher `import math`) | 17 |
| sin 45 (Auswahl: sin, cos, tan, asin, acos, atan) | `math.sin(math.radians(45))` (Blockly rechnet in Grad, Python im Bogenmaß); `math.degrees(math.asin(x))` | 17 |
| π | `math.pi` | 17 |
| 0 ist gerade | `x % 2 == 0` (ungerade: `x % 2 == 1`) | 02 |
| runde 3.1 (Auswahl: runde, runde auf, runde ab) | `round(3.1)`; runde auf: `math.ceil(x)`, runde ab: `math.floor(x)` (vorher `import math`) | 01/17 |
| Summe über die Liste | `sum(liste)` | 06 |
| begrenze 50 zwischen 1 und 100 | `min(max(50, 1), 100)` | 09 |
| ganzzahlige Zufallszahl zwischen 1 und 100 | `random.randint(1, 100)` (beide Grenzen möglich, wie in Blockly) | 16 |
| Zufallszahl (0.0 - 1.0) | `random.random()` | 16 |

Achtung: `round(2.5)` ist in Python `2` (Python rundet bei ,5 zur geraden Zahl).

## Text (violett)

| Blockly | Python | Notebook |
|---|---|---|
| “ ” (Text) | `'…'` oder `"…"` | 01 |
| erstelle Text aus … | `'a' + 'b'` oder `f'{a} und {b}'` | 05 |
| an etwas Text anhängen … | `etwas = etwas + '…'` | 05 |
| Länge von … | `len(text)` | 05 |
| … ist leer | `text == ''` | 05 |
| im Text suche erstes Auftreten des Begriffs … | `text.find(begriff)` (Blockly: Position ab 1, 0 = nicht gefunden; Python: ab 0, -1 = nicht gefunden) | 05 |
| vom Text nehme #ten Buchstaben | `text[i - 1]` (Python zählt ab 0!) |
| vom Text nehme #ten Buchstaben von hinten | `text[-i]` |
| vom Text nehme ersten / letzten Buchstaben | `text[0]` / `text[-1]` |
| vom Text nehme zufälligen Buchstaben | `random.choice(text)` | 05 |
| im Text nehme Teil ab #tem Buchstaben bis zum #ten Buchstaben | `text[a - 1:b]` | 05 |
| wandel um in GROSSBUCHSTABEN (Auswahl: GROSSBUCHSTABEN, kleinbuchstaben, Substantive) | `text.upper()`, `text.lower()`, `text.title()` (jedes Wort mit großem Anfangsbuchstaben) | 05 |
| entferne Leerzeichen vom Anfang und vom Ende | `text.strip()` | 05/08 |
| gib aus … | `print(…)` | 01 |
| frage nach Text mit Hinweis … | `input('Hinweis')` | – (nicht in JupyterLite) |

## Listen (orange)

| Blockly | Python | Notebook |
|---|---|---|
| erzeuge eine leere Liste | `[]` | 06 |
| erzeuge Liste mit … | `[a, b, c]` | 06 |
| erzeuge Liste mit 5 mal dem Element … | `[x] * 5` | 06 |
| Länge von … | `len(liste)` | 06 |
| … ist leer | `liste == []` oder `len(liste) == 0` | 06 |
| in der Liste suche erstes Auftreten von … | `liste.index(x)` (Python: ab 0, Fehler wenn nicht vorhanden; vorher `x in liste` prüfen) | 06/09 |
| in der Liste nimm #tes | `liste[i - 1]` | 06 |
| in der Liste setze für #tes ein … | `liste[i - 1] = x` | 06 |
| in der Liste erhalte Unterliste von # bis zu # | `liste[a - 1:b]` | 06 |
| Liste aus Text erstellen mit Trennzeichen „,“ (Auswahl: Liste aus Text, Text aus Liste) | `text.split(',')` (Leerzeichen: `text.split()`) | 06/08 |
| Text aus Liste erstellen mit Trennzeichen „,“ (Auswahl im selben Block) | `','.join(liste)` | 06 |
| numerisch aufsteigend sortieren | `sorted(liste)` (absteigend: `sorted(liste, reverse=True)`) | 06 |
| (kein Block) | `liste.append(x)`: hinten anhängen | 06 |

## Variablen

| Blockly | Python | Notebook |
|---|---|---|
| setze zaehler auf … | `zaehler = …` | 01 |
| erhöhe zaehler um 1 | `zaehler = zaehler + 1` (kurz: `zaehler += 1`) | 01 |
| zaehler (Wert benutzen) | `zaehler` | 01 |

Namen in Python: Buchstaben, Ziffern, `_`, keine Leerzeichen, nicht mit Ziffer beginnen; üblich ist Kleinschreibung
ohne Umlaute (`zaehler_vokale` statt `Zähler_Vokale`).

## Funktionen (lila)

| Blockly | Python | Notebook |
|---|---|---|
| etwas tun (ohne Rückgabe) | `def etwas_tun():` | 07 |
| etwas tun … gib zurück … | `def etwas_tun():` … `return wert` | 07 |
| falls … gib zurück … | `if …: return …` | 07 |
| Parameter (über ⚙) | `def etwas_tun(a, b):` | 07 |

## Farben (lila)

Die Farbblöcke (Farbe, zufällige Farbe, Farbe aus rot/grün/blau, mische Farbe) haben keine direkte Entsprechung.
In Python schreibt man Farben als Tupel `(100, 50, 0)` (rot, grün, blau), z. B. beim Zeichnen und bei Bildern (Notebooks 19, 20).
