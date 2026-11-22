# 🍪 Plätzchen-Wettbewerb

Webseite für einen Plätzchenbackwettbewerb, komplett am Handy.

- **Für alle:** https://fammarek.github.io/Plaetzchen/
- **Leitung:** https://fammarek.github.io/Plaetzchen/?leitung

## Ablauf
1. **Anmelden** (Tab „Anmelden“): Jeder Bäcker trägt Namen und Sorte ein. Mehrere Sorten pro Person sind möglich.
   Eigene Einträge lassen sich wieder entfernen. Die Sorten bekommen Nummern (zum Beschriften der Teller).
   Die Bäcker bleiben bis zur Siegerehrung geheim.
2. **Verkostung starten** (Leitung): schließt die Anmeldung. Alle Handys springen zu „Bewerten“.
3. **Bewerten:** Namen eintragen und jede Sorte nach 5 Kriterien von 1 bis 10 bewerten.
   Wer mit dem Namen seiner Anmeldung bewertet, bewertet die eigene Sorte nicht.
   Man kann bis zur Verkündung nachbessern. Es zählt die letzte Abgabe.
4. **Platzierungen verkünden** (Leitung): Die Leitung sieht, welche Bäcker schon abgestimmt haben.
   Ein Druck auf den Knopf zeigt auf allen Handys nach einem Trommelwirbel das Siegertreppchen und die Rangliste.

## Leitungs-Ansicht
Die Seite mit `?leitung` aufrufen, also https://fammarek.github.io/Plaetzchen/?leitung.
Nur dort gibt es die Knöpfe zum Starten und Verkünden (inklusive Zurückschalten bei Fehlern).
Diesen Link nicht weitergeben.

## Bewertung
| Kriterium    | Gewicht | Frage |
|--------------|:------:|-------|
| Geschmack    | 4 | Wie lecker ist es? |
| Textur       | 2 | Mürbe, saftig, knusprig – passt es? |
| Nachschlag   | 2 | Würdest du sofort noch eins nehmen? |
| Aussehen     | 1 | Form, Farbe, Verzierung |
| Originalität | 1 | Besondere Idee oder Note? |

Pro Bewerter und Sorte wird der gewichtete Durchschnitt gebildet, dann über alle Bewerter gemittelt (max. 10 Punkte).
Bei gleicher Punktzahl teilen sich die Sorten den Platz.
Anpassbar im Block `KONFIGURATION` in `index.html`.

## Einrichten
1. GitHub → *Settings → Pages* → *Deploy from a branch* → Branch und Ordner `/ (root)` wählen.
2. In `index.html` bei `kanal` einen eigenen, schwer erratbaren Namen eintragen
   (oder den Link mit `?kanal=meinname` bzw. `?kanal=meinname&leitung` verwenden).
3. Link als QR-Code verteilen.

## Speicherung
Die Daten liegen beim kostenlosen Dienst [ntfy.sh](https://ntfy.sh) (ohne Anmeldung), und zwar nur **ca. 12 Stunden**.
Deshalb am Tag des Wettbewerbs anmelden.
Für jeden neuen Wettbewerb einen neuen Kanalnamen verwenden.
