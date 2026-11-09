Stand: 06.02.2026
Die 1. und 2. Zeile der Ausgabe muss für alle Beispieleingaben in der Dokumentation abgedruckt sein.

Die vollständige Ausgabedatei muss für folgende Beispiele in der Dokumentation abgedruckt sein:
lieferung00.txt
lieferung01.txt
lieferung02.txt
lieferung03.txt

Die vollständige Ausgabe aller Beispieleingaben muss außerdem als .txt in einem Output-Ordner abgegeben werden. Die Dateien sollten eindeutig benannt sein, zum Beispiel lieferung00_out.txt
Die .txt-Dateien müssen diesem Ausgabeformat folgen:

1. Zeile: MOEGLICH für lösbare bzw. UNMOEGLICH für nicht lösbare Beispiele. Ist das Beispiel nicht lösbar, müssen die folgenden Zeilen nicht ausgegeben werden.
2. Zeile: Maximale Routendauer, die nach dem Plan eintreten kann.
Leerzeile
Dauer der Route von S zu T ohne Streik.
Die Route von S zu T ohne Streik.
In den folgenden Zeilen folgen die Alternativrouten:
- In der ersten Zeile die Gesamtdauer der Alternativroute von S zu T.
- In der zweiten Zeile die Alternativroute. Sie startet mit der Werks-ID des bestreikten Werks und endend bei T.
Leerzeile am Ende der Ausgabe.

Eine Route wird durch die Werks-IDs der nacheinander besuchten Werke, sowie S und T angegeben. Die ID eines Werks, in dem ein Produktionsschritt stattfindet, wird zusammen mit der Kennzahl dieses Produktionsschritts in eckige Klammern gesetzt. Zum Beispiel würde [1 3] bedeuten, dass in dem Werk mit der Werks-ID 1 der Produktionsschritt 3 ausgeführt wird. Wird in einem Werk kein Produktionsschritt ausgeführt, wird nur die Werks-ID angegeben.
Je Arbeitsschritt wird eine Alternativroute angegeben, falls das Werk für diesen Arbeitsschritt auf der ursprünglich geplanten Route bestreikt wird. Die Angabe einer Alternativroute beginnt mit der ID des Werks, in dem wegen einem Streik auf der ursprünglich geplanten Route die Durchführung des Arbeitsschritts nicht möglich ist, und enthält die alternative Route ab dem bestreikten Werk bis zu T mit allen Zwischenschritten. Die Routendauer der Alternativroute wird von S zu T angegeben.

Hier ein Beispiel:
MOEGLICH
11

9
S [3 1] [5 2] T
10
3 [2 1] [4 2] T
11
5 T [4 2] T

Das Beispiel ist lösbar, und es werden maximal 11 Zeiteinheiten benötigt.
Die direkte Route von S zu T dauert 9 Zeiteinheiten. Die Route beginnt beim Startpunkt S und führt über Werk 3 (hier wird Schritt 1 ausgeführt) und Werk 5 (hier wird Schritt 2 ausgeführt) zum Zielpunkt T.
Da in Werk 3 und 5 Arbeitsschritte ausgeführt werden, müssen zwei Alternativrouten angegeben werden: Eine für den Ausfall von Werk 3 und eine für den Ausfall von Werk 5.
Sollte Werk 3 bestreikt werden, kann dort der 1. Arbeitsschritt nicht ausgeführt werden. Die alternative Route dauert insgesamt 10 Zeiteinheiten. Von Werk 3 aus führt die Route über Werk 2 (hier wird Schritt 1 ausgeführt) und Werk 4 (hier wird Schritt 2 ausgeführt) zu T.
Sollte Werk 5 bestreikt werden, kann dort der 2. Arbeitsschritt nicht ausgeführt werden. Die alternative Route dauert insgesamt 11 Zeiteinheiten. Von Werk 5 aus führt die Route über T zu Werk 4 (hier wird Schritt 2 ausgeführt) zurück zu T.