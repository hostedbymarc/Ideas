# Angebot: Marille Kauf-Check

Methode: die Offers-Linse (`founder-board/lenses.md`), angewandt auf die Einwände aus Panel v2 (`archive-v2/panel/results.md`) und die Wettbewerbsanalyse. Alter Pitch: `pitch-v1.md`, neuer Pitch: `pitch.md`.

## 1. Problemliste (in Käuferworten, aus Panel und Wettbewerb)

Vor dem Kauf
1. „Ohne Gratisversion kauf ich die Katze im Sack.“
2. „Wer steht hinter Marille?“
3. „Wo liegen meine Kredit- und Wohnungsdaten?“
4. „Es gibt keine Bewertungen.“
5. „Der Score und die Steuer sind eine Blackbox.“
6. „Stimmen Grunderwerbsteuer, Eintragung, Pfandrecht, AfA, Mietpreisdeckel?“
7. „19 € ist so billig, ist das ein Hobbyprojekt, das in einem Jahr weg ist?“
8. „Es gibt gratis Rechner (Optifin, ImmoScout24, Bank).“
9. „Die Bank rechnet mir das sowieso vor.“
10. „Mein Excel reicht.“
11. „Ich verstehe Beleihungsauslauf und Cashflow nach Steuer nicht gut genug.“
12. „Ich trau mir nicht zu, die richtigen Zahlen einzugeben.“

Während der Nutzung
13. „Ich muss alles händisch eintippen.“
14. „Ich will gegen meine Tabelle prüfen können.“
15. „Nimmt die Bank so einen PDF-Report ernst?“
16. „Ich will nicht noch eine App neben Parqet.“

Nach dem Kauf
17. „Nach dem Kauf brauche ich den Check nicht mehr, wozu verlängern?“
18. „Was passiert mit meinen Daten, wenn es Marille nicht mehr gibt?“
19. „Hilft mir das bei der Steuererklärung für die Mieteinnahmen?“
20. „Wenn's falsch rechnet, kostet mich ein falsches PDF mehr als 19 €.“

## 2. Lösungen, bewertet

Wert für den Käufer 1-5, Kosten 1-5 (Geld oder deine Zeit bei 5 h/Woche; Geldkosten sind bei Software fast null, die knappe Ressource ist deine Zeit).

| Problem | Lösung | Wert | Kosten | behalten? |
| --- | --- | ---: | ---: | --- |
| 1, 4, 5 | öffentlicher Beispiel-Report einer echten Wiener Wohnung, ohne Anmeldung | 5 | 1 | ✅ Bonus |
| 5, 6, 14 | jede Zahl mit aufklappbarer Formel und Quelle | 5 | 3 | ✅ Bonus |
| 10, 14 | Excel/CSV-Export | 4 | 2 | ✅ Bonus |
| 2, 3, 7 | Impressum mit Namen, Gründer-Seite, EU-Server | 5 | 1 | ✅ Kern (Pflicht) |
| 1, 20 | 30 Tage Geld zurück, eine E-Mail genügt | 4 | 1 | ✅ Garantie |
| 7 | Gründungsmitglieder behalten 19 € dauerhaft | 3 | 1 | ✅ echte Knappheit |
| 18 | Datenexport jederzeit, Löschung auf Knopfdruck | 3 | 2 | ✅ Kern |
| 6 | Mietpreisdeckel/Richtwert für Altbau | 4 | 3-4 | ❓ nur wenn die App das schon kann |
| 6, 9, 15 | Rechenlogik von Steuerberatung prüfen lassen | 5 | 4 (Geld) | ⏳ später, sobald Umsatz da |
| 13 | Inserat-Import (willhaben-Link) | 4 | 5 | ❌ zu teuer jetzt, AGB-Fragen |
| 16 | Parqet-Sync | 3 | 5 | ❌ |
| 19 | E1b-Hilfe für die Steuererklärung | 4 | 4 | ⏳ Kandidat für den Grund zu verlängern |

## 3. Der Stack

- **Name:** Marille Kauf-Check.
- **Kern (das Ergebnis):** „Du weißt vor der Unterschrift, ob deine erste Anlagewohnung dich jeden Monat Geld kostet oder dir Geld bringt, gerechnet nach österreichischen Regeln.“ Dazu PDF für die Bank und das Portfolio nach dem Kauf.
- **Bonus 1, Beispiel-Report ohne Anmeldung** → tötet „Katze im Sack“.
- **Bonus 2, Formel und Quelle bei jeder Zahl** → tötet „Blackbox“ und „stimmen die AT-Zahlen?“.
- **Bonus 3, Excel-Export** → tötet „mein Excel reicht“ (Marille wird zum Prüfwerkzeug für die eigene Tabelle).
- **Vertrauen:** Gründer mit Namen, Impressum, EU-Server.
- **Garantie:** 30 Tage Geld zurück ohne Begründung.
- **Knappheit (echt):** die ersten 100 Gründungsmitglieder behalten 19 €/Jahr, solange sie verlängern.

## 4. Was die Garantie kostet

Bei 50 Kunden × 19 € = 950 € Umsatz. Erstattet wird der Preis; die Stripe-Gebühr von etwa 0,54 € pro Zahlung (1,5 % + 0,25 € für EWR-Standardkarten laut [ki-syndikat.de](https://www.ki-syndikat.de/tools/stripe/), offizielle Seite prüfen) bekommt man bei einer Erstattung nach meinem Wissen nicht zurück; bitte in Stripe prüfen.

| Erstattungsquote | erstattete Kunden | Umsatzverlust |
| ---: | ---: | ---: |
| 10 % | 5 | ca. 98 € |
| 20 % | 10 | ca. 195 € |
| 30 % | 15 | ca. 293 € |

Die Quote ist unbekannt. Der CFO rechnet sie als Was-wäre-wenn.

## 5. Wertgleichung (1-10, vorher → nachher)

| Element | vorher | nachher | was es bewegt |
| --- | ---: | ---: | --- |
| Wunschergebnis | 6 | 7 | Ergebnis statt Funktionsliste („vor der Unterschrift wissen“) |
| Wahrgenommene Wahrscheinlichkeit | 3 | 6 | Beispiel-Report, Formeln mit Quelle, Impressum, Garantie |
| Zeit bis zum Ergebnis | 6 | 6 | unverändert (Eingabe bleibt händisch) |
| Aufwand | 5 | 6 | Excel-Export erspart den Doppelabgleich; Eintippen bleibt |

## 6. Re-Test (gleiche 20 Käufer, Seed 555280)

- **Vorher (Pitch v2): 8 von 20 (40 %). Nachher: 9 von 20 (45 %).** Ein Käufer kippt zu Ja (P011: Beispiel-Report, Impressum und Garantie räumen das Vertrauensproblem aus). Keiner kippt zu Nein.
- **„Keine Gratisversion“ fällt von 14 auf 4 Einwände.** Der Beispiel-Report wirkt genau dort, wo er soll.
- **Die Vorsichtigen Prüfer steigen von 33 % auf 67 %.**
- **Was sich nicht bewegt:** Wer sich auf Bank und Kreditvermittler verlässt (0 von 4), Gratis-Nutzer (0 von 3) und wer schon gekauft hat (1 von 5). Das ist kein Angebotsproblem, sondern Markt: diese Leute haben keinen Moment, in dem sie den Check brauchen, oder trauen sich das Rechnen nicht zu.
- **Neuer Einwand:** zwei Käufer (P015, P016) fragen gezielt, ob der **Mietpreisdeckel/Richtwert bei Altbau** berücksichtigt ist.

**Schluss:** Das Angebot hat die Vertrauenshürde gesenkt, die Kaufrate aber kaum gehoben. Die Grenze liegt beim Segment: verkauft wird an Leute **mitten in Besichtigungen** (64 %), nicht an Leute, die schon gekauft haben oder Profis rechnen lassen. Marketing sollte genau diesen Moment suchen.

## 7. Vor dem Launch zu bauen (sonst darf der Pitch es nicht versprechen)

- [ ] Beispiel-Report einer echten Wiener Wohnung öffentlich (ohne Anmeldung)
- [ ] Formel und Quelle bei jeder Zahl
- [ ] Excel/CSV-Export
- [ ] Impressum, Datenschutzerklärung, Gründer-Seite
- [ ] Supabase-Region prüfen: liegt das Projekt in der EU? (sonst „EU-Server“ streichen)
- [ ] Stripe-Abo mit 30-Tage-Erstattung; Widerrufsrecht für digitale Inhalte mit Anwalt/WKO klären
- [ ] Klären, ob Marille den Mietpreisdeckel/Richtwert schon rechnet
