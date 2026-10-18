# Zusammenfassung

**Was:** Marille ist eine fertige Web-App, mit der Erstinvestoren in Österreich vor der Unterschrift sehen, ob ihre Anlagewohnung sie jeden Monat Geld kostet oder Geld bringt, nach österreichischen Regeln und mit jeder Zahl offengelegt. Nach dem Kauf übernimmt man die Wohnung ins Portfolio. Preis: 19 € pro Jahr (Test gegen 29 €), ohne Gratisversion, mit öffentlichem Beispiel-Report und 30 Tagen Geld zurück.

**Urteil (berechnet von `compile.py`): Profitable.** Die drei Zahlen dahinter:
- **Beitrag pro Kunde: 18,33 € (96 %)** nach Stripe-Gebühren.
- **Break-even: knapp 2 neue Kunden pro Monat** (Fixkosten 31 €/Monat).
- **Jahr 1: 543 € Betriebsergebnis** bei 50 Kunden und 950 € Umsatz.

**Was dieses „Profitable“ nicht enthält, ohne Beschönigung:**
- Die **Werbung** (500 €) zählt als Startkosten: nach ihr bleiben in Jahr 1 **+43 €**; mit dem vollen Budget von 1.000 € **-457 €**.
- **Steuerberatung, WKO-Grundumlage und Haftpflichtversicherung** fehlen, weil es noch keine Angebote gibt. Schon wenige hundert Euro davon machen Jahr 1 negativ.
- **Deine Zeit** ist mit 0 € gerechnet (260 Stunden im Jahr, also etwa 0,17 € pro Stunde).
- Die **50 Kunden** sind dein Ziel, nicht gemessen.
Profitabel heißt hier: Jeder Kunde rechnet sich, und der Betrieb trägt sich. Ein Einkommen ist es bei 50 Kunden nicht.

**Worin Panel und Board übereinstimmen:** Der Kunde zahlt im Moment vor dem Kauf (Panel: 64 % der Leute mitten in Besichtigungen kaufen, alle anderen 20-25 %); das Portfolio allein verkauft nicht; Vertrauen und österreichische Genauigkeit sind der Kern; über den Preis gewinnt man nicht. **Wo sie sich unterscheiden:** Der Board (2× Pass, 1× Fund if; Schnitt 3,3/10) bezweifelt Markt und Vertrieb grundsätzlich; das Panel zeigt nach dem Umbau des Angebots 45 % Kaufbereitschaft. Das Panel sind simulierte Käufer und eher zu freundlich; die Board-Skepsis zu Reichweite und Wiederholung ist damit **nicht** widerlegt.

**Das größte Risiko:** dass Marille rechtlich als Beratung gilt oder falsch rechnet. Beides zerstört das Vertrauen, auf dem das Angebot steht. Plan: WKO/Anwalt diese Woche fragen; Testfälle gegen echte Kaufverträge; Fehler-Routine (SOP C).

**Was du zum Start brauchst:** 500-1.000 € für Werbung, ca. 60 Stunden bis zum 11. Jänner 2027 und **den Vorverkauf vom 16. November bis 13. Dezember** als ersten Test mit echten Käufern (Erfolg: mindestens 10 Vorbestellungen und 2 % der Besucher bei 300+ Besuchern).

**Diese Woche:** Beim WKO-Gründerservice anfragen: Gewerbe IT-Dienstleistung **und** ob eine Rechenhilfe mit Investment-Score als Beratung gilt.
