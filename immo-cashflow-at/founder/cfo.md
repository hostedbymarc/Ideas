# CFO-Notiz: Marille

**Lesehilfe:** Das Tool schreibt `$`, gemeint sind **Euro**. Weil Marille Jahresabos verkauft und kein Café ist, steht „a day“ hier für **neue zahlende Kunden pro Monat** (`days_per_month = 1`). Umsatz = Zahlung bei Abschluss (Kassensicht); Verlängerungen kommen erst ab Monat 13 und sind nicht in Jahr 1.

- **Die Marge:** Jedes Abo lässt nach Stripe-Gebühren **18,33 € (96 %)** übrig. Die Fixkosten sind mit 30 € im Monat winzig, Break-even liegt bei **knapp 2 neuen Kunden pro Monat**. Bei deinem Ziel von 50 Kunden in Jahr 1 bleiben **556 € Betriebsergebnis** auf 950 € Umsatz, nach 500 € Werbung **+56 €**.
- **Die Zeile, die alles entscheidet: Werbung pro Kunde.** Mit 500 € Werbung kostet jeder der 50 Kunden 10 € Werbung, Ergebnis Jahr 1 **+56 €**, Startgeld in Monat 12 zurück. Mit 1.000 € Werbung kostet jeder Kunde 20 € Werbung, also **mehr, als er in Jahr 1 einbringt (18,33 €)**: Ergebnis **-444 €**, Startgeld nicht in Jahr 1 zurück. Bei 19 € darf ein Kunde höchstens rund 18 € Werbung kosten, sonst rechnet er sich erst mit der Verlängerung.
- **Cash:** 500 € (oder 1.000 € mit vollem Werbebudget), weil die Werbung vor den ersten Verkäufen bezahlt wird. Bisher ausgegebene ca. 300 € für Abos sind darin nicht enthalten (schon ausgegeben).
- **Deine Zeit:** gerechnet mit 0 €. Zur Einordnung: 5 h/Woche sind rund 260 Stunden im Jahr; 56 € Ergebnis sind etwa **0,20 € pro Stunde**. Das ist wichtig, weil es zeigt: Bei 50 Kunden ist Marille ein Projekt, noch kein Einkommen.
- **Garantie:** 20 % Erstattungen wirken wie „Volume -20 %“: Betriebsergebnis 373 €, nach 500 € Werbung **-127 €**.

**Drei Wege, die Marge zu verbessern (aus dem Tool gerechnet):**
1. **Preis 29 € statt 19 €:** Beitrag 28,33 €, Betriebsergebnis Jahr 1 **1.056 €** (+500 €). Liegt im akzeptablen Bereich des Panels (5-49 €). Mit 39 €: **1.556 €**.
2. **Werbung durch Partner und Content ersetzen** (Kreditvermittler, Finanz-Communities, eigener Beispiel-Report): jeder Euro Werbung, der wegfällt, geht 1:1 ins Ergebnis.
3. **Verlängerungen** (nicht im Modell): Jeder verlängernde Kunde bringt in Jahr 2 nochmals 18,33 € ohne Werbekosten. Das ist der Hebel, für den das Portfolio da ist.

**Board-Bedingungen zum Geld (`board.md`):**
- „Unit Economics, die aufgehen“: **teilweise erfüllt.** Pro Kunde ja (96 % Beitrag, Fixkosten minimal). Insgesamt nur knapp und nur, wenn ein Kunde weniger als ~18 € Werbung kostet.
- „19 € tragen kaum Kundengewinnung, Steuerprüfung und Betrieb“: **bestätigt.** Eine Steuerberater-Prüfung der Rechenlogik ist in diesen Zahlen nicht drin; schon wenige hundert Euro dafür machen Jahr 1 negativ.

**Offene Kosten (nicht im Modell, weil noch nicht aktiviert):** Domain, E-Mail, Steuerberater, Supabase-Bezahltarif ab mehr Nutzern. Bitte Preise nennen, sobald du sie hast.

**Steuern:** Die Beträge sind ohne Umsatzsteuer gerechnet. In Österreich gibt es eine Kleinunternehmerregelung (bei diesem Umsatz vermutlich anwendbar, dann keine USt auf 19 €). Ob und wie (Gewerbe, Einkommensteuer, SVS) muss ein Steuerberater bestätigen. Das hier ist keine Steuer-, Rechts- oder Finanzberatung.

---

# Unit economics: Marille (Kauf-Check + Portfolio, 19 € pro Jahr)

Every number below comes from the input file. Nothing is looked up or guessed.

## One Jahresabo (neuer zahlender Kunde)

| line | per Jahresabo (neuer zahlender Kunde) |
| --- | ---: |
| Price | $19.00 |
| Stripe Kartengebühr (1,5 % + 0,25 €) | -$0.54 |
| Stripe Billing für Abos (ca. 0,7 %, Schätzung) | -$0.13 |
| **Contribution** (what each Jahresabo (neuer zahlender Kunde) leaves to pay the fixed costs) | **$18.33** (96%) |

## The margin that matters

Fixed costs: $30 a month (Claude-Abo $22, Netlify $8, Supabase (Gratis-Tarif) $0).

- **Break-even: 2 Jahresabo (neuer zahlender Kunde)s a day.** Below that you lose money every month.
- **Profit margin at your plan** (5 a day): **65%** of every sale, after every cost.

## Year 1, month by month

| month | Jahresabo (neuer zahlender Kunde)s a day | revenue | profit | cumulative (after $500 startup) |
| ---: | ---: | ---: | ---: | ---: |
| 1 | 2 | $38 | $7 | -$493 |
| 2 | 3 | $57 | $25 | -$468 |
| 3 | 3 | $57 | $25 | -$443 |
| 4 | 4 | $76 | $43 | -$400 |
| 5 | 4 | $76 | $43 | -$357 |
| 6 | 4 | $76 | $43 | -$313 |
| 7 | 5 | $95 | $62 | -$252 |
| 8 | 5 | $95 | $62 | -$190 |
| 9 | 5 | $95 | $62 | -$128 |
| 10 | 5 | $95 | $62 | -$67 |
| 11 | 5 | $95 | $62 | -$5 |
| 12 | 5 | $95 | $62 | $56 |

- **Year 1 operating profit: $556** on $950 of revenue.
- After the $500 startup spend: $56.
- Startup money earned back: month 12.
- Cash you need before it pays for itself: **$500**.

## What if

| scenario | margin at plan | break-even a day | year 1 profit |
| --- | ---: | ---: | ---: |
| Base plan | 65% | 2 | $556 |
| Price -10% | 61% | 2 | $462 |
| Volume -20% | 57% | 2 | $373 |
| Unit costs +15% | 64% | 2 | $551 |

No red flags in these numbers. They are only as good as the inputs: check every cost against a real quote.
