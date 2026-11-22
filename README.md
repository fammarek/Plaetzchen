# 🍪 Plätzchen-Wettbewerb

Die Teilnehmer bewerten jede Plätzchensorte am Handy nach festgelegten Kriterien.
`index.html` sammelt die Stimmen und berechnet den Sieger automatisch.

## Einrichten
1. In `index.html` den Block **KONFIGURATION** anpassen: Sorten, Kriterien mit Gewicht, Skala und `kanal`.
   Für den `kanal` einen eigenen, schwer erratbaren Namen wählen.
2. GitHub → *Settings → Pages* → Source: *Deploy from a branch*, Branch wählen, Ordner `/ (root)`.
3. Den Link (z. B. als QR-Code) an alle verteilen.

## Ablauf
- **Bewerten:** Namen eintragen, optional die eigene Sorte wählen (die bewertet man dann nicht), alle Kriterien antippen, abschicken.
  Man kann erneut abschicken. Es zählt immer die letzte Abgabe pro Name.
- **Ergebnis:** Siegertreppchen, Rangliste, Durchschnitt je Kriterium und wer schon abgestimmt hat. Aktualisiert sich alle 15 s.

## Berechnung
Pro Bewerter und Sorte: gewichteter Durchschnitt der Kriterien.
Gesamtpunkte einer Sorte: Mittelwert über alle Bewerter.
Bei gleicher Punktzahl entscheidet die Anzahl der Stimmen.

## Speicherung
Die Stimmen gehen an den kostenlosen Dienst [ntfy.sh](https://ntfy.sh) (ohne Anmeldung) und bleiben dort **ca. 12 Stunden** gespeichert.
Wer den Kanalnamen kennt, kann mitlesen und auch Stimmen abgeben.
Für einen neuen Wettbewerb einfach einen neuen Kanal nehmen oder den Link mit `?kanal=neuername` verwenden.
