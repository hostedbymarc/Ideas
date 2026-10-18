# Marille (Immo-Cashflow) · Business plan

**Verdict: Profitable**

- ✓ Each Jahresabo (neuer zahlender Kunde) earns $18.33 before fixed costs (96% contribution).
- ✓ Year 1 operating profit: $543.
- ✓ 9 of 20 simulated buyers buy (45%, the bar is 25%).

| key number | |
| --- | ---: |
| Price | $19.00 a Jahresabo (neuer zahlender Kunde) |
| Profit margin at plan | 64% per Jahresabo (neuer zahlender Kunde) |
| Break-even | 2 Jahresabo (neuer zahlender Kunde)s a day |
| Year 1 operating profit | $543 |
| Startup spend | $500 |
| Cash needed before it pays for itself | $500 |
| Startup money earned back | month 12 |
| Buyer panel | 9 buy · 11 pass |

## The idea

- What it is: Eine fertig gebaute Web-App (marille.netlify.app), mit der private Immobilieninvestoren in Österreich prüfen, ob sich eine Wohnung rentiert und ob ihr monatlicher Cashflow nach der Kreditrate positiv oder negativ ist (Deal-Analyse), und ihr Immobilienportfolio tracken (Wert, Eigentumsanteil, Tilgung, Restschuld, Cashflow pro Monat).
- Who it is for: Erstinvestoren in Österreich, die gerade ihre erste Vorsorge- bzw. Anlagewohnung suchen oder gekauft haben.
- What it sells, at what price: „Marille Kauf-Check“: Zugang für 19 € pro Jahr (Test gegen 29 €), Deal-Analyse + Portfolio-Tracking. Keine Gratisversion; öffentlicher Beispiel-Report und 30 Tage Geld zurück.
- Where and how: Online (Web-App), ganz Österreich. Kanäle: Reddit, Instagram mit Grafiken, Beispiel-Report als Landingpage, kleiner Google-Ads-Test; Zahlung über Stripe. Launch 11. Jänner 2027, Vorverkauf ab 16. November 2026.
- Budget and constraints: Gründer arbeitet seit Anfang 2026 allein daran und hat die App selbst mit Claude Code gebaut. Bisher rund 300 € für Abos ausgegeben (Claude, Supabase, Netlify). 5 Stunden pro Woche (Zeit mit 0 € gerechnet); Werbebudget 500-1.000 €; Ziel Jahr 1: 50 zahlende Kunden.

### Was die App heute kann (aus Screenshots und zwei Deal-Reports vom 18.10.2026)
- Deal-Analyse mit Tabs Überblick, Bank, Cashflow, Details.
- Investment-Score 0-100 aus Rendite (45 %), Risiko (25 %), Substanz (15 %), Lage (15 %), mit Ampel von "Vorsicht" bis "Top" und Textbewertung.
- Österreichische Kaufnebenkosten einzeln: Grunderwerbsteuer, Maklercourtage, Grundbucheintragung, Kaufvertragserrichtung, Pfandrechtseintragung.
- Bank-Kennzahlen: LTV auf Kaufpreis und Gesamtinvestition, Beleihungsauslauf auf Bankwert, DSCR, Annuität, Zinsbindung, Anschlusszins-Annahme.
- Cashflow-Kette von Kaltmiete über BK/Rücklage, Annuität und Steuer bis Netto, Tilgung und "realer Vermögensaufbau"; Mietausfall-Puffer; Cashflow-Projektion mit Mietindexierung und Break-even-Jahr.
- PDF-Deal-Report (14 Seiten) und "In Portfolio übernehmen".
- Portfolio: Gesamtwert, Eigentumsanteil, Restschuld, nächster Tilgungs-Meilenstein, Monatsbilanz (Tilgung, Cashflow, Marktwert).
- Der Gründer nutzt es selbst mit zwei eigenen Wohnungen in Wien.

## Summary

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

## What the board said

### Abstimmung

**2 PASS, 1 FUND IF** · Durchschnitt **3,3 / 10**

| Linse | Score | Vote |
| --- | ---: | --- |
| Offers | 3 | PASS |
| Monopoly | 3 | PASS |
| Product | 4 | FUND IF |

Memos: `board/offers.md`, `board/monopoly.md`, `board/product.md`.

### Risiken, die mehrere Mitglieder nennen (zuerst)

1. **Seltener Moment, wiederkehrender Preis** (alle drei). Ein Erstinvestor braucht die Analyse wenige Wochen rund um einen Kauf, dann jahrelang nicht. Ein Jahresabo wird einmal gekauft und nicht verlängert. Portfolio-Tracking ist vor dem Kauf wertlos (Panel: 0 von 9 Erstinvestoren hätten gezahlt).
2. **Gegen Gratis gewinnt man nicht über den Preis** (alle drei). Excel war der häufigste Ablehnungsgrund (8 von 20). 19 € senken den Preis, nicht den Einwand, und ein sehr niedriger Preis kann bei einer sechsstelligen Entscheidung Vertrauen kosten (Offers).
3. **19 € pro Jahr tragen kaum Kundengewinnung, Steuerprüfung und Betrieb** (Offers, Monopoly; Product fragt danach). Kosten und Akquisitionskosten sind unbekannt.
4. **Vertrauen und Richtigkeit für Österreich** (alle drei). Ein falscher Wert bei Nebenkosten oder AfA ist ein Vertrauensbruch. Die österreichische Rechenlogik, geprüft und sichtbar belegt, ist zugleich der stärkste mögliche Vorteil.

Nur Monopoly: kein Schutz gegen Nachahmer (Banken, Kreditvermittler, Parqet könnten das gratis anbieten), kein erkennbarer Vertriebsweg. Nur Product: zwei Produkte in einem, das Produkt braucht *ein* Ding.

### Uneinigkeit

Offers und Monopoly lehnen ab, weil Markt und Vertrieb (wer zahlt, wiederholt, wie erreicht man ihn) nicht tragen. Product sieht einen klaren Kernmoment („Rentiert sich diese Wohnung?“) und würde unter Bedingungen finanzieren, wenn der Fokus geschärft und das Preismodell an den Moment angepasst wird.

### Bedingungen (Checkliste für den Rest des Packs)

- [ ] **Ein Kernprodukt wählen** (naheliegend: Prüfung eines konkreten Objekts bis zur Cashflow-Antwort); Tracking als spätere Stufe. *(Product)*
- [ ] **Ein Satz ohne „und“ plus die ersten fünf Minuten** vom Inserat bis zur Antwort, mit Zahl der Eingaben. *(Product)*
- [ ] **Preismodell passend zum Moment:** Einmalkauf rund um einen Kauf testen oder belegen, welchen laufenden Wert ein Jahresabo nach dem Kauf liefert. *(Offers, Product → /founder-pricing, /founder-offer)*
- [ ] **Ein Angebot, das nicht über den Preis gewinnt:** geprüfte Österreich-Rechnung, Import statt Eintippen, Zinsszenarien, Check vor der Unterschrift, leistbare Garantie. *(Offers → /founder-offer)*
- [ ] **Rechenlogik von einer Steuerberatung prüfen lassen**, sichtbar im Produkt, mit Impressum, Team und EU-Datenhaltung. *(alle → /founder-ops, /founder-brand)*
- [ ] **Segment belegen:** Wie viele Erstinvestoren pro Jahr in Österreich, oder ein Segment mit wiederkehrendem Bedarf (Mehrfachinvestoren, Kreditvermittler, Makler). *(Offers, Monopoly → /founder-competitors, /founder-consumer)*
- [ ] **Vertriebsweg zu den ersten 100 zahlenden Kunden** mit Kosten pro Kunde, ggf. über Partner. *(Monopoly → /founder-marketing)*
- [ ] **Wettbewerb kartieren:** Wer bietet diesen Käufern heute Rechner an, gratis oder bezahlt? *(Monopoly, Offers → /founder-competitors)*
- [ ] **Unit Economics, die aufgehen:** Entwicklungs-, Betriebs- und Akquisitionskosten gegen den Preis. *(alle → /founder-cfo)*
- [ ] **Echte Käufer statt Panel:** Vorverkauf oder Warteliste mit echtem Preis. *(Offers, Product → /founder-launch)*

### Die stärkste Version, die der Board sieht

Nicht „Rechner plus Tracker im Jahresabo für 19 €“, sondern ein **Kauf-Check für eine konkrete Wohnung**: Der Erstinvestor gibt ein Inserat ein und bekommt in wenigen Minuten eine von einer österreichischen Steuerberatung geprüfte Antwort, ob die Wohnung nach Kreditrate Geld bringt oder kostet, mit Zinsszenarien und einer Fragenliste für Makler und Bank, bezahlt einmal pro Kaufentscheidung zu einem Preis, der eher eine Entscheidung über eine sechsstellige Summe widerspiegelt als 19 €. Das Tracking kommt erst, wenn der Kunde gekauft hat, und wäre der Weg vom Einmalkunden zum Wiederkehrenden. Das weicht vom Pitch ab: weniger Funktionen, anderes Preismodell, und vermutlich ein Vertrieb über Partner, die Erstinvestoren schon erreichen. Alle Zahlen dazu sind offen.

## The competition

Stand 18.10.2026. Nur öffentliche Quellen, jede Angabe verlinkt. **Einschränkung:** Aus dieser Umgebung konnten die Seiten nicht direkt geöffnet werden; alle Fakten stammen aus Suchergebnissen (Snippets von App-Store- und Anbieterseiten). Preise vor einer Entscheidung direkt auf den Seiten prüfen. Rohdaten: `competitors.csv`.

### 1. Wer ist da (nach Nähe zum Angebot sortiert)

| Anbieter | Typ | Vergleichbarer Preis | Was | Bewertung |
| --- | --- | --- | --- | --- |
| [Immo Cashflow](https://apps.apple.com/at/app/immo-cashflow/id6553989584) (Primus Vision UG) | direkt | **AT-Store: 19,99 €/Jahr** oder 39,99 € einmalig; DE: 3,99 €/Monat | Cashflow-/Renditerechner-App | 4,4-4,5 ★ aus 7-8 ([Rezensionen](https://apps.apple.com/de/app/immo-cashflow/id6553989584?see-all=reviews&platform=iphone)) |
| [Optifin Vorsorgewohnungs-Rechner](https://www.optifin.at/vorsorgewohnungs-rechner/) | direkt | kostenlos | AT-Rechner: Finanzierung, Steuer, Cashflow, Vorsteuer, ImmoESt; nach eigener Aussage einziger mit Mietpreisdeckel 2026 | keine |
| [Immo Portfolio](https://mwm.ai/apps/immo-portfolio/6737453391) (Primus Vision UG) | direkt | 1 Objekt gratis, weitere per Einmalkauf (Preis nicht gefunden) | Portfolio-Cashflow bis EK-Rendite | keine gefunden |
| [ImmoFluss](https://www.immo-fluss.de/) | direkt | 1. Immobilie gratis, Abo-Preis nicht gefunden | Vermieter-App mit Kredit-/Restschuld-Tracking; Steuerexport nur deutsche Anlage V ([Store](https://apps.apple.com/de/app/immofluss/id6748078139)) | 4,6 ★ aus 9 |
| [Parqet](https://parqet.com/en/blog/track-real-estate) | indirekt | Plus 11,99 €/Monat ([broker-test](https://www.broker-test.at/news/parqet-erhoeht-preise-ab-1-august-2025-jetzt-noch-schnell-bestandsabo-holen/)); Jahr ca. 75-100 € ([mydealz](https://www.mydealz.de/deals/parqet-plus-mit-25-rabatt-neujahrs-angebot-2705722)) | Wertpapier-Tracker, Immobilien manuell, Kredit über Cash-Konto ([broker-test](https://www.broker-test.at/news/parqet-portfolio-tracker-erweitert-sich-auf-immobilien-uhren-und-sachwerte/)) | – |
| [Soldd](https://www.theproptechscout.com/listing/soldd/) | indirekt | ab 39,99 €/Monat (altes Listing) | bewertet willhaben-Inserate nach Rendite ([Trending Topics](https://www.trendingtopics.eu/soldd/)) | – |
| [ImmoScout24.at Renditerechner](https://www.immobilienscout24.at/wissen/finanzierung/renditerechner.html) | indirekt | kostenlos | Brutto-/Netto-Rendite | – |
| Deutsche Gratis-Rechner ([Interhyp](https://www.interhyp.de/kapitalanlagerechner/), [IMMORath](https://immorath.de/finanzieren/cashflow-rechner/), [cashflowrechner.de](https://cashflowrechner.de/), [RenditeRechner24](https://renditerechner24.de/kalkulationstool-immobilie-rendite-profitabilitaet-finanzierung-kostenlos-als-excel)) | indirekt | kostenlos | Cashflow mit **deutscher** Steuerlogik | – |
| [Bank-Kreditrechner](https://www.raiffeisen.at/stmk/de/immobilien/rechner-tools.html) + Bankberater, Kreditvermittler, Vorsorgewohnungs-Anbieter ([Standard](https://www.derstandard.at/story/2660057/die-rente-zahlt-der-mieter)) | Ersatz | für Käufer gratis | Rechnung als Teil von Kredit/Verkauf | – |
| Excel (selbst oder [Vorlage 18,90 €](https://www.digistore24.com/product/651735)) | Ersatz | 0-19 € einmalig | eigene Tabelle | – |

### 2. Preisspanne (vergleichbares Produkt: Rechner/Tracker für Privatinvestoren)

- **Niedrigster:** 0 € (Optifin, ImmoScout24, deutsche Rechner, Excel, Banken).
- **Median der bezahlten Angebote:** rund 20 € pro Jahr (Immo Cashflow 19,99 €/Jahr; Excel-Vorlage 18,90 € einmalig; Immo Cashflow einmalig 39,99 €).
- **Höchster:** Soldd ab ca. 360 €/Jahr (jährliche Abrechnung, altes Listing); Parqet Plus ca. 75-144 €/Jahr (allerdings für Wertpapiere, nicht für Immobilien gebaut).
- **Marilles 19 €/Jahr liegt exakt auf dem Preis des direktesten Konkurrenten** (Immo Cashflow, AT-Store 19,99 €/Jahr).

### 3. Positionierungs-Karte

Achse 1: **Österreich-Genauigkeit** (AT-Nebenkosten, AfA 1,5 %, Liebhaberei, Mietpreisdeckel). Achse 2: **Vor dem Kauf ↔ nach dem Kauf** (Deal-Prüfung vs. Portfolio-Tracking).

```
                       hohe AT-Genauigkeit
                              |
           Optifin (gratis)   |   [ Marille: beides, AT ]
                              |
   VOR DEM KAUF --------------+-------------- NACH DEM KAUF
                              |
  Immo Cashflow, Soldd,       |   Immo Portfolio, ImmoFluss,
  ImmoScout24, DE-Rechner     |   Parqet (manuell)
                              |
                      generisch / deutsch
```

Banken/Kreditvermittler sitzen „vor dem Kauf, AT-genau, aber nicht neutral“: Sie rechnen im Interesse ihres Kredits oder Produkts.

### 4. Beschwerden (Bewertungen sind sehr dünn, alle Themen „thin“)

Keiner der Anbieter hat mehr als 9 öffentliche Bewertungen gefunden. Es gibt also **keinen belastbaren Beschwerdekorpus**. Was es gibt:

1. **Bezahlschranke an der falschen Stelle** (thin, 1 Rezension): Bei Immo Cashflow muss man für das Bearbeiten eines Objekts zahlen, sonst neu eingeben ([Rezensionen](https://apps.apple.com/de/app/immo-cashflow/id6553989584?see-all=reviews&platform=iphone)).
2. **Rechnungen der Verkäufer sind geschönt** (thin, aber Verbraucherschutz): Die AK kritisiert, dass Verkaufsunterlagen oft Mietrenditen auf den Nettokaufpreis mit statischen Annahmen bewerben ([AK 2018](https://www.arbeiterkammer.at/service/presse/Geldanlage_Vorsorgewohnung_2018.pdf)); die AK Wien hält Renditeversprechen von 3,5-3,9 % für überzogen und warnt vor Klumpenrisiko ([vienna.at](https://www.vienna.at/arbeiterkammer-wien-warnt-vor-vorsorgewohnungen/5758737)).
3. **Immobilien in Parqet sind Handarbeit** (thin): Wert manuell, Finanzierung nur als Cash-Konto-Umweg ([broker-test](https://www.broker-test.at/news/parqet-portfolio-tracker-erweitert-sich-auf-immobilien-uhren-und-sachwerte/)).
4. **Deutsche Tools passen nicht zu Österreich** (abgeleitet aus Beschreibungen, keine Beschwerde): ImmoFluss exportiert nur die deutsche Anlage V; IMMORath rechnet die deutsche 15-%-Grenze.

### 5. Die Lücke

**Es gibt eine Lücke, aber sie ist schmal und nicht der Preis.**

- Niemand verbindet **Prüfung vor dem Kauf und Tracking nach dem Kauf mit österreichischer Logik**. Optifin ist AT-genau, aber nur ein Rechner (und hinter ihm steht ein Finanzierungsgeschäft). Die Tracker (ImmoFluss, Immo Portfolio, Parqet) sind deutsch oder generisch. Marille ist laut den Screenshots das einzige gefundene Produkt, das „In Portfolio übernehmen“ als Übergang vom Deal zum Besitz anbietet.
- **Neutralität:** Die Rechnungen, die ein Erstinvestor heute bekommt, kommen vom Verkäufer oder der Bank. Ein unabhängiger Kauf-Check gegen geschönte Prospekte (AK-Kritik) ist eine Lücke mit Beleg.
- **Kein Platz über den Preis:** Gratis gibt es reichlich (Optifin, ImmoScout24, Banken, Excel), und 19,99 €/Jahr hat Immo Cashflow schon. 19 € ist kein Unterscheidungsmerkmal.

### 6. Die Bedrohung

- **Optifin** am schnellsten: hat schon den AT-genauen Rechner gratis und verdient an der Finanzierung; könnte ein Login mit gespeicherten Objekten ergänzen.
- **Primus Vision UG** (Immo Cashflow + Immo Portfolio): hat beide Hälften (Deal und Portfolio) als zwei Apps, bereits im AT-Store zu 19,99 €/Jahr. Zusammenlegen plus AT-Steuerlogik wäre ein kleiner Schritt.
- **Parqet**: hat die Nutzer, die „alles an einem Ort“ wollen; eine Kredit-/Restschuld-Funktion würde Marilles Tracking-Hälfte für viele überflüssig machen.
- **Banken/Kreditvermittler** können jeden Rechner gratis als Lockmittel anbieten.

### Achtung: Namenskonflikt
Der Arbeitsname **„Immo-Cashflow“ ist bereits ein App-Name** ([Immo Cashflow im AT-Store](https://apps.apple.com/at/app/immo-cashflow/id6553989584)). Der Produktname „Marille“ hat dieses Problem nicht; `/founder-brand` prüft ihn.

## The buyer panel

**9 buy · 11 pass** (45% buy) out of 20 simulated buyers. Seed 555280, so the same cards can be dealt again.

These are simulated buyers, not customers. Use this to find objections and weak spots, then confirm the big ones with real people before you spend.

### By segment

| group | buyers | buy rate |
| --- | ---: | ---: |
| Sucht gerade die erste Anlagewohnung (Besichtigungen laufen) | 11 | 64% |
| Überlegt noch, ob eine Anlagewohnung überhaupt in Frage kommt | 4 | 25%  (thin) |
| Hat die erste Anlagewohnung in den letzten 12 Monaten gekauft | 5 | 20%  (thin) |

### By buying behaviour

| group | buyers | buy rate |
| --- | ---: | ---: |
| Bereits Parqet-Nutzer | 2 | 100%  (thin) |
| Finanz-Content-Konsument | 4 | 100%  (thin) |
| Vorsichtiger Prüfer | 3 | 67%  (thin) |
| Excel-Bastler | 4 | 25%  (thin) |
| Verlässt sich auf Profis | 4 | 0%  (thin) |
| Gratis-Nutzer | 3 | 0%  (thin) |

### By income

| group | buyers | buy rate |
| --- | ---: | ---: |
| under $54,000 | 4 | 75%  (thin) |
| $54,000 to $69,000 | 8 | 38% |
| $69,000 and up | 8 | 38% |

### Why they pass

| reason | buyers | in their words |
| --- | ---: | --- |
| habit | 8 | "Ich hab mir für meine erste Wohnung eh schon eine Excel gebaut, mit Grunderwerbsteuer, Grundbuch, Pfandrecht und AfA. Für die Besichtigung nächste Woche schau ich mir euren Gratis-Beispielreport an, gleich meine Formeln damit ab und rechne dann in meiner eigenen Tabelle weiter." (P003) · "Ehrlich gesagt rechne ich so etwas nicht selbst. Mein Kreditvermittler und die Bank legen mir die Rate und die Nebenkosten sowieso hin, und der Makler hat eine Renditeberechnung im Exposé. Ein weiteres Tool, in das ich alles selbst eintippen muss, passt nicht zu mir." (P005) |
| timing | 2 | "Meine Wohnung habe ich schon gekauft, der Kauf-Check vor der Unterschrift kommt für mich ein Jahr zu spät. Den Cashflow rechne ich eh schon in meiner eigenen Excel nach, und für ein reines Portfolio-Tracking einer einzigen Wohnung gebe ich keine Kreditdaten an ein Ein-Personen-Startup." (P001) · "Ich weiß ja noch nicht mal, ob eine Anlagewohnung für mich überhaupt in Frage kommt, und hab keine konkrete Wohnung, die ich durchrechnen müsste. Den Beispiel-Report schau ich mir vielleicht gratis an und bau mir die Positionen dann in meine eigene Tabelle." (P009) |
| need | 1 | "Ich hab die Wohnung schon gekauft, der Kauf-Check kommt für mich zu spät, und gerechnet haben damals eh die Bankberaterin und der Makler. Wie es jetzt läuft, sehe ich in meiner Excel-Tabelle und am Konto, dafür brauche ich kein eigenes Tool." (P002) |

### Why they buy

| reason | buyers | in their words |
| --- | ---: | --- |
| need | 4 | "Ich bin gerade mitten in den Besichtigungen und meine Excel hat sicher Lücken bei Nebenkosten und Steuer. 19 € mit 30 Tagen Geld-zurück ist weniger als ein Abendessen, und wenn der Excel-Export meine Tabelle bestätigt oder korrigiert, hat es sich schon gelohnt." (P004) · "Ich besichtige gerade Wohnungen, und 19 € sind nichts gegen einen Fehler bei einem Kauf um 250.000 €. Ich lass meine Excel-Tabelle gegen den Export laufen, und wenn sie sich nicht unterscheiden, hol ich mir einfach das Geld zurück." (P007) |
| timing | 4 | "Ich hab nächsten Monat das Bankgespräch und besichtige gerade, da kommt mir ein PDF mit Beleihungsauslauf und allen Nebenkosten genau recht. Ich schau mir zuerst den Beispiel-Report und das Impressum an, und wenn die Zahlen mit meiner eigenen Rechnung zusammenpassen, riskiere ich die 19 Euro, die krieg ich ja per E-Mail zurück." (P011) · "Ich hab nächste Woche eine Besichtigung und rechne gerade in einer zusammengebastelten Excel herum. 19 € mit 30 Tagen Geld-zurück probier ich aus wie jede neue Finanz-App, vor allem wenn ich vorher den Beispiel-Report anschauen kann und mit dem PDF besser vorbereitet ins Bankgespräch gehe." (P013) |
| convenience | 1 | "Die erste Wohnung hab ich schon, aber ich scroll eh jeden Abend durch willhaben für die zweite. 19 € im Jahr mit Geld-zurück ist weniger als ein Abendessen, also teste ich es, lass meine bestehende Wohnung durchrechnen und vergleich das mit meiner Excel." (P010) |

### What would flip a no

- Wenn ich konkret die zweite Wohnung suche und der Beispiel-Report auf der Website meine eigene Rechnung auf den Euro bestätigt, plus ein paar echte Bewertungen von anderen Anlegern aus Wien.
- Wenn meine Bankberaterin oder mein Steuerberater es mir empfiehlt oder selbst damit arbeitet, oder wenn es mir konkret bei der Steuererklärung für die Vermietung hilft.
- Wenn mir der Vergleich mit dem Beispielreport zeigt, dass meine Tabelle bei der Steuer oder beim Cashflow falsch rechnet, oder wenn das Tool Daten liefert, die ich selbst nicht habe, zum Beispiel realistische Vergleichsmieten und Marktwerte für die konkrete Wiener Lage.
- Wenn mein Kreditvermittler oder ein Freund, der schon eine Anlagewohnung hat, sagt, dass die Bankrechnung oft zu schön ist und ich das vorher gegenprüfen soll, dann zahle ich die 19 Euro vor der Besichtigung ohne nachzudenken.
- Wenn ich meine eigene Wohnung gratis einmal durchrechnen könnte, ohne Kreditdaten zu speichern, und dabei rauskommt, dass ich bei der Steuer oder Tilgung etwas übersehen hab, das mich wirklich Geld kostet.
- Wenn ich meine eigene Wohnung einmal gratis durchrechnen könnte und dabei sehe, dass die Bank oder mein Rechner etwas Wichtiges übersehen hat, zum Beispiel bei der Steuer oder beim Cashflow.
- Wenn ich eine konkrete Wohnung im Auge hätte und vor der Unterschrift stehe, wäre mir die Steuer-Rechnung nach österreichischen Regeln die 19 € wert, weil ich das selbst nicht sicher hinbekomme.
- Wenn mein Bankberater oder Makler mir den Report selbst empfiehlt oder damit arbeitet, oder wenn ich die Daten meiner schon gekauften Wohnung einfach aus dem Kreditvertrag übernehmen könnte und es mir in einfachen Worten sagt, ob sie sich rechnet.
- Wenn mein Bankberater oder Kreditvermittler sagt, dass er mit so einem Report arbeitet oder ihn gern sieht, oder wenn ich eine Wohnung vom Inserat gratis einmal durchrechnen könnte.
- Wenn meine Bank beim Finanzierungsgespräch sagt, dass sie so einen PDF-Report mit Beleihungsauslauf und Steuerrechnung gern sieht, oder wenn ich beim Gegenchecken merke, dass meine Tabelle bei der Steuer falsch rechnet, dann kauf ich es vor dem Termin.
- Wenn ich nach dem Beispiel-Report merke, dass die Gratis-Rechner und die Bank wichtige Kosten oder die Steuer weglassen und ich konkret eine Wohnung im Auge habe, würde ich es mit der Geld-zurück-Garantie vor dem Bankgespräch probieren.

Buyers say they would buy **1.0 times** in the first month on average.

20 buyers gave all four price answers. Run founder-pricing's van_westendorp.py on the answers folder.

## Pricing

Grundlage: Panel v2 (20 simulierte Erstinvestoren, `panel/answers`), `pricing-curve.md`, `competitors.md`. **Die Marge fehlt noch**: Es gibt noch keine `numbers.json`; der CFO-Schritt rechnet sie nach, sobald die Kosten bekannt sind.

### 1. Der Preis

**Empfehlung: bei 19 € pro Jahr starten, 29 € pro Jahr als zweiten Preis testen.**

- **Panel (Van Westendorp, simuliert):** akzeptabler Bereich 5 € bis 49 € pro Jahr. Indifferenzpreis (IPP) 19,09 €: genau dort, wo gleich viele „günstig“ wie „teuer“ sagen. Mediane: zu billig 3 €, günstig 10 €, wird teuer 39 €, zu teuer 69 €. 19 € liegt also sicher im Bereich, mit Luft nach oben bis etwa 39 €.
- **Konkurrenz:** Der direkteste Konkurrent, Immo Cashflow, kostet im AT-Store 19,99 €/Jahr oder 39,99 € einmalig ([App Store](https://apps.apple.com/at/app/immo-cashflow/id6553989584)). Optifin, ImmoScout24, Banken und Excel sind gratis. Parqet Plus kostet ca. 75-144 €/Jahr, allerdings für Wertpapiere.
- **Was das Panel sagt:** Der Preis hat **keinen einzigen** Käufer abgehalten. Zwei Käufer fanden 19 € eher **zu billig, um verlässlich zu sein** (P011, P020). Der eigentliche Bremsklotz ist nicht der Preis, sondern „keine Gratisversion, ich kann vorher nicht prüfen, ob es stimmt“ (in 14 von 20 Einwänden).
- **Marge:** offen. Bei einem Software-Abo sind die variablen Kosten pro Kunde vermutlich klein (Zahlungsgebühren, Anteil an Hosting/KI-Kosten), aber das rechnet `/founder-cfo` mit deinen echten Zahlen.

### 2. Die Leiter

Das Panel zeigt zwei Momente mit unterschiedlichem Wert: **vor dem Kauf** (Deal prüfen, PDF für die Bank) und **nach dem Kauf** (Portfolio). Eine Leiter, die daran anknüpft, ohne Gratisversion:

| Stufe | Inhalt | Preis (zu testen) | Grund zum Aufsteigen |
| --- | --- | --- | --- |
| Beispiel-Report | Ein vollständiger Musterreport einer echten Wiener Wohnung, öffentlich, ohne Anmeldung | 0 € (kein Produkt, sondern Beweis) | zeigt, dass die AT-Zahlen stimmen, beantwortet „Katze im Sack“ |
| Jahr | Alles: Deal-Analysen, PDF-Reports, Portfolio | 19 € (Test: 29 €) | Kernprodukt |
| Jahr + Prüfung (später) | wie Jahr, plus Rechenlogik von Steuerberatung bestätigt oder ein Report-Check vor dem Bankgespräch | offen, erst mit echten Kosten | für die, die zu viel Angst vor einem falschen PDF haben (P011, P020) |

Die dritte Stufe ist eine Idee aus den Einwänden, kein Beschluss; sie braucht eine Kostenschätzung (Steuerberatung) und wird bei `/founder-offer` und `/founder-ops` geprüft.

### 3. Das Eröffnungsangebot

**„Gründungsmitglied“:** Die ersten 100 Kunden zahlen 19 € pro Jahr dauerhaft, solange sie verlängern. Danach gilt der reguläre Preis (19 € oder 29 €, je nach Test). Ende: wenn 100 Plätze vergeben sind oder spätestens an einem festen Datum, das bei `/founder-launch` gesetzt wird. Kein „statt X €“-Preis, solange X nie verlangt wurde.

### 4. Was mit echten Käufern zu testen ist

- **19 € vs. 29 € pro Jahr:** zwei Varianten der Landingpage (zufällig zugeteilt) mit echtem Bezahl-Button oder Vorverkauf. Messen: Anteil der Besucher, die bezahlen.
- **Mit vs. ohne öffentlichen Beispiel-Report:** prüft die These, dass Vertrauen und Nachprüfbarkeit mehr verkaufen als ein niedriger Preis.
- Mindestens je 100 echte Besucher pro Variante, bevor man etwas abliest.

### 5. Die Preis- und Kauf-Einwände im Wortlaut (Panel, simuliert)

1. „Keine Gratisversion. Ich soll zahlen, bevor ich sehe, ob mir das mehr bringt als die kostenlosen Rechner und das, was mir die Bank sowieso zeigt.“ (P019)
2. „19 Euro im Jahr für Steuer, Kaufnebenkosten und Bank-Kennzahlen klingt fast zu billig. Wenn die Berechnung falsch ist und ich mit einem falschen PDF zur Bank gehe, kostet mich das viel mehr als 19 Euro.“ (P011)
3. „19 Euro sind so billig, dass ich mich frage, ob die Steuerberechnung und die Kaufnebenkosten wirklich stimmen oder ob das ein Hobbyprojekt ist, das in einem Jahr wieder weg ist.“ (P020)

Simulierte Antworten wählen aus, was getestet wird; sie sind kein Beweis.

## The offer

Methode: die Offers-Linse (`founder-board/lenses.md`), angewandt auf die Einwände aus Panel v2 (`archive-v2/panel/results.md`) und die Wettbewerbsanalyse. Alter Pitch: `pitch-v1.md`, neuer Pitch: `pitch.md`.

### 1. Problemliste (in Käuferworten, aus Panel und Wettbewerb)

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

### 2. Lösungen, bewertet

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

### 3. Der Stack

- **Name:** Marille Kauf-Check.
- **Kern (das Ergebnis):** „Du weißt vor der Unterschrift, ob deine erste Anlagewohnung dich jeden Monat Geld kostet oder dir Geld bringt, gerechnet nach österreichischen Regeln.“ Dazu PDF für die Bank und das Portfolio nach dem Kauf.
- **Bonus 1, Beispiel-Report ohne Anmeldung** → tötet „Katze im Sack“.
- **Bonus 2, Formel und Quelle bei jeder Zahl** → tötet „Blackbox“ und „stimmen die AT-Zahlen?“.
- **Bonus 3, Excel-Export** → tötet „mein Excel reicht“ (Marille wird zum Prüfwerkzeug für die eigene Tabelle).
- **Vertrauen:** Gründer mit Namen, Impressum, EU-Server.
- **Garantie:** 30 Tage Geld zurück ohne Begründung.
- **Knappheit (echt):** die ersten 100 Gründungsmitglieder behalten 19 €/Jahr, solange sie verlängern.

### 4. Was die Garantie kostet

Bei 50 Kunden × 19 € = 950 € Umsatz. Erstattet wird der Preis; die Stripe-Gebühr von etwa 0,54 € pro Zahlung (1,5 % + 0,25 € für EWR-Standardkarten laut [ki-syndikat.de](https://www.ki-syndikat.de/tools/stripe/), offizielle Seite prüfen) bekommt man bei einer Erstattung nach meinem Wissen nicht zurück; bitte in Stripe prüfen.

| Erstattungsquote | erstattete Kunden | Umsatzverlust |
| ---: | ---: | ---: |
| 10 % | 5 | ca. 98 € |
| 20 % | 10 | ca. 195 € |
| 30 % | 15 | ca. 293 € |

Die Quote ist unbekannt. Der CFO rechnet sie als Was-wäre-wenn.

### 5. Wertgleichung (1-10, vorher → nachher)

| Element | vorher | nachher | was es bewegt |
| --- | ---: | ---: | --- |
| Wunschergebnis | 6 | 7 | Ergebnis statt Funktionsliste („vor der Unterschrift wissen“) |
| Wahrgenommene Wahrscheinlichkeit | 3 | 6 | Beispiel-Report, Formeln mit Quelle, Impressum, Garantie |
| Zeit bis zum Ergebnis | 6 | 6 | unverändert (Eingabe bleibt händisch) |
| Aufwand | 5 | 6 | Excel-Export erspart den Doppelabgleich; Eintippen bleibt |

### 6. Re-Test (gleiche 20 Käufer, Seed 555280)

- **Vorher (Pitch v2): 8 von 20 (40 %). Nachher: 9 von 20 (45 %).** Ein Käufer kippt zu Ja (P011: Beispiel-Report, Impressum und Garantie räumen das Vertrauensproblem aus). Keiner kippt zu Nein.
- **„Keine Gratisversion“ fällt von 14 auf 4 Einwände.** Der Beispiel-Report wirkt genau dort, wo er soll.
- **Die Vorsichtigen Prüfer steigen von 33 % auf 67 %.**
- **Was sich nicht bewegt:** Wer sich auf Bank und Kreditvermittler verlässt (0 von 4), Gratis-Nutzer (0 von 3) und wer schon gekauft hat (1 von 5). Das ist kein Angebotsproblem, sondern Markt: diese Leute haben keinen Moment, in dem sie den Check brauchen, oder trauen sich das Rechnen nicht zu.
- **Neuer Einwand:** zwei Käufer (P015, P016) fragen gezielt, ob der **Mietpreisdeckel/Richtwert bei Altbau** berücksichtigt ist.

**Schluss:** Das Angebot hat die Vertrauenshürde gesenkt, die Kaufrate aber kaum gehoben. Die Grenze liegt beim Segment: verkauft wird an Leute **mitten in Besichtigungen** (64 %), nicht an Leute, die schon gekauft haben oder Profis rechnen lassen. Marketing sollte genau diesen Moment suchen.

### 7. Vor dem Launch zu bauen (sonst darf der Pitch es nicht versprechen)

- [ ] Beispiel-Report einer echten Wiener Wohnung öffentlich (ohne Anmeldung)
- [ ] Formel und Quelle bei jeder Zahl
- [ ] Excel/CSV-Export
- [ ] Impressum, Datenschutzerklärung, Gründer-Seite
- [ ] Supabase-Region prüfen: liegt das Projekt in der EU? (sonst „EU-Server“ streichen)
- [ ] Stripe-Abo mit 30-Tage-Erstattung; Widerrufsrecht für digitale Inhalte mit Anwalt/WKO klären
- [ ] Klären, ob Marille den Mietpreisdeckel/Richtwert schon rechnet

## The numbers

**Lesehilfe:** Das Tool schreibt `$`, gemeint sind **Euro**. Weil Marille Jahresabos verkauft und kein Café ist, steht „a day“ hier für **neue zahlende Kunden pro Monat** (`days_per_month = 1`). Umsatz = Zahlung bei Abschluss (Kassensicht); Verlängerungen kommen erst ab Monat 13 und sind nicht in Jahr 1.

- **Die Marge:** Jedes Abo lässt nach Stripe-Gebühren **18,33 € (96 %)** übrig. Die Fixkosten sind mit 31 € im Monat winzig (inkl. Domain), Break-even liegt bei **knapp 2 neuen Kunden pro Monat**. Bei deinem Ziel von 50 Kunden in Jahr 1 bleiben **543 € Betriebsergebnis** auf 950 € Umsatz, nach 500 € Werbung **+43 €**.
- **Die Zeile, die alles entscheidet: Werbung pro Kunde.** Mit 500 € Werbung kostet jeder der 50 Kunden 10 € Werbung, Ergebnis Jahr 1 **+43 €**, Startgeld in Monat 12 zurück. Mit 1.000 € Werbung kostet jeder Kunde 20 € Werbung, also **mehr, als er in Jahr 1 einbringt (18,33 €)**: Ergebnis **-457 €**, Startgeld nicht in Jahr 1 zurück. Bei 19 € darf ein Kunde höchstens rund 18 € Werbung kosten, sonst rechnet er sich erst mit der Verlängerung.
- **Cash:** 500 € (oder 1.000 € mit vollem Werbebudget), weil die Werbung vor den ersten Verkäufen bezahlt wird. Bisher ausgegebene ca. 300 € für Abos sind darin nicht enthalten (schon ausgegeben).
- **Deine Zeit:** gerechnet mit 0 €. Zur Einordnung: 5 h/Woche sind rund 260 Stunden im Jahr; 43 € Ergebnis sind etwa **0,17 € pro Stunde**. Das ist wichtig, weil es zeigt: Bei 50 Kunden ist Marille ein Projekt, noch kein Einkommen.
- **Garantie:** 20 % Erstattungen wirken wie „Volume -20 %“: Betriebsergebnis 360 €, nach 500 € Werbung **-140 €**.

**Drei Wege, die Marge zu verbessern (aus dem Tool gerechnet):**
1. **Preis 29 € statt 19 €:** Beitrag 28,33 €, Betriebsergebnis Jahr 1 **1.043 €** (+500 €). Liegt im akzeptablen Bereich des Panels (5-49 €). Mit 39 €: **1.543 €**.
2. **Werbung durch Partner und Content ersetzen** (Kreditvermittler, Finanz-Communities, eigener Beispiel-Report): jeder Euro Werbung, der wegfällt, geht 1:1 ins Ergebnis.
3. **Verlängerungen** (nicht im Modell): Jeder verlängernde Kunde bringt in Jahr 2 nochmals 18,33 € ohne Werbekosten. Das ist der Hebel, für den das Portfolio da ist.

**Board-Bedingungen zum Geld (`board.md`):**
- „Unit Economics, die aufgehen“: **teilweise erfüllt.** Pro Kunde ja (96 % Beitrag, Fixkosten minimal). Insgesamt nur knapp und nur, wenn ein Kunde weniger als ~18 € Werbung kostet.
- „19 € tragen kaum Kundengewinnung, Steuerprüfung und Betrieb“: **bestätigt.** Eine Steuerberater-Prüfung der Rechenlogik ist in diesen Zahlen nicht drin; schon wenige hundert Euro dafür machen Jahr 1 negativ.

**Offene Kosten (nicht im Modell, weil noch nicht aktiviert):** Steuerberater, WKO-Grundumlage, Versicherung, Supabase-Bezahltarif ab mehr Nutzern. Bitte Preise nennen, sobald du sie hast.

**Steuern:** Die Beträge sind ohne Umsatzsteuer gerechnet. In Österreich gibt es eine Kleinunternehmerregelung (bei diesem Umsatz vermutlich anwendbar, dann keine USt auf 19 €). Ob und wie (Gewerbe, Einkommensteuer, SVS) muss ein Steuerberater bestätigen. Das hier ist keine Steuer-, Rechts- oder Finanzberatung.

---

## Unit economics: Marille (Kauf-Check + Portfolio, 19 € pro Jahr)

Every number below comes from the input file. Nothing is looked up or guessed.

### One Jahresabo (neuer zahlender Kunde)

| line | per Jahresabo (neuer zahlender Kunde) |
| --- | ---: |
| Price | $19.00 |
| Stripe Kartengebühr (1,5 % + 0,25 €) | -$0.54 |
| Stripe Billing für Abos (ca. 0,7 %, Schätzung) | -$0.13 |
| **Contribution** (what each Jahresabo (neuer zahlender Kunde) leaves to pay the fixed costs) | **$18.33** (96%) |

### The margin that matters

Fixed costs: $31 a month (Claude-Abo $22, Netlify $8, Supabase (Gratis-Tarif) $0, Domain .at (OVHcloud Verlängerung 13,48 €/Jahr inkl. Starter-E-Mail) $1).

- **Break-even: 2 Jahresabo (neuer zahlender Kunde)s a day.** Below that you lose money every month.
- **Profit margin at your plan** (5 a day): **64%** of every sale, after every cost.

### Year 1, month by month

| month | Jahresabo (neuer zahlender Kunde)s a day | revenue | profit | cumulative (after $500 startup) |
| ---: | ---: | ---: | ---: | ---: |
| 1 | 2 | $38 | $6 | -$494 |
| 2 | 3 | $57 | $24 | -$471 |
| 3 | 3 | $57 | $24 | -$447 |
| 4 | 4 | $76 | $42 | -$405 |
| 5 | 4 | $76 | $42 | -$362 |
| 6 | 4 | $76 | $42 | -$320 |
| 7 | 5 | $95 | $61 | -$260 |
| 8 | 5 | $95 | $61 | -$199 |
| 9 | 5 | $95 | $61 | -$139 |
| 10 | 5 | $95 | $61 | -$78 |
| 11 | 5 | $95 | $61 | -$17 |
| 12 | 5 | $95 | $61 | $43 |

- **Year 1 operating profit: $543** on $950 of revenue.
- After the $500 startup spend: $43.
- Startup money earned back: month 12.
- Cash you need before it pays for itself: **$500**.

### What if

| scenario | margin at plan | break-even a day | year 1 profit |
| --- | ---: | ---: | ---: |
| Base plan | 64% | 2 | $543 |
| Price -10% | 60% | 2 | $448 |
| Volume -20% | 56% | 2 | $360 |
| Unit costs +15% | 63% | 2 | $538 |

No red flags in these numbers. They are only as good as the inputs: check every cost against a real quote.

## Marketing

Grundlage: `panel/results.md` (Angebots-Re-Test), `competitors.md`, `offer.md`, `pricing.md`, `cfo.md`. Rahmen vom Gründer: **kein Gesicht zeigen**, eventuell Instagram mit Grafiken, Reddit; Werbebudget 500-1.000 €; Preis-Test **19 € vs. 29 €**.

### 1. Positionierung

Wer am meisten kauft: **Erstinvestoren mitten in Besichtigungen, mit Bankgespräch in Sicht** (64 % Kaufrate im Re-Test, gegenüber 20-25 % bei allen anderen). Gründe in ihren Worten: „Bankgespräch nächsten Monat“, „mein Excel hat die Nebenkosten und die Steuer nur grob“.

Drei Versionen:

A. **Für Erstinvestoren vor der Unterschrift**, die nicht wissen, ob die Wohnung sie jeden Monat Geld kostet, ist Marille der **unabhängige Kauf-Check**, der nach österreichischen Regeln rechnet und jede Zahl offenlegt, anders als die Rechnung von Bank, Bauträger oder Makler, die etwas verkaufen wollen.

B. Für Erstinvestoren vor dem Bankgespräch, die ihr eigenes Excel nicht ganz trauen, ist Marille der Prüf-Report, der die eigene Tabelle gegencheckt, anders als Gratis-Rechner, die nur eine Zahl ausspucken.

C. Für Leute, die gerade auf willhaben Anlagewohnungen scrollen, ist Marille der Schnell-Check, der in Minuten sagt, ob ein Inserat sich rechnet, anders als ein Abend in Excel.

**Empfehlung: A.** Belege: Die Lücke „Neutralität“ aus `competitors.md` (AK-Kritik an geschönten Verkaufsrechnungen); der stärkste Hebel im Re-Test war Vertrauen (Vorsichtige Prüfer 33 % → 67 %); B ist die beste **Botschaft für Excel-Bastler** und wird als Hook genutzt. C verspricht Geschwindigkeit, die das Produkt (händische Eingabe) noch nicht liefert.

### 2. Kanäle

| Kanal | warum es passt | Kosten | woran man sieht, dass es wirkt | Start? |
| --- | --- | --- | --- | --- |
| **Reddit** (österreichische Finanz- und Wien-Subreddits; Existenz und Regeln jedes Subreddits vorher prüfen) | anonym möglich; dort fragen Leute „rechnet sich diese Vorsorgewohnung?“; Werbung nur, wo die Regeln es erlauben; Faustregel 90 % echte Hilfe, 10 % Eigenes ([redship](https://redship.io/blog/reddit-self-promotion-rules)) | 0 € + Zeit | Besuche mit Reddit-Quelle; Käufe davon | ✅ |
| **Instagram mit Grafiken** (Karussells: „Diese Wiener Wohnung durchgerechnet“) | kein Gesicht nötig; Finanz-Content-Konsumenten kauften im Panel 4 von 4 | 0 € + Zeit | Profilbesuche → Link-Klicks → Käufe | ✅ |
| **Beispiel-Report als Landingpage (SEO)** | wer „Vorsorgewohnung Rechner“ sucht, ist genau im richtigen Moment; Optifin rankt dort schon | 0 € + Zeit; wirkt erst nach Monaten | Google-Search-Console-Klicks | ✅ (Basis für alles) |
| **Google Search Ads** auf „Vorsorgewohnung Rechner/Cashflow“ | Kaufmoment; kurzer Test mit hartem Limit | Klickpreise unbekannt; Test-Limit 200 € | Kosten pro zahlendem Kunden < 18 € (19 €) bzw. < 28 € (29 €) | ⏳ Woche 3, nur Test |
| Kreditvermittler/Makler als Partner | erreichen genau diese Käufer, aber du willst Neutralität; Interessenkonflikt | Provision | – | ❌ vorerst, widerspricht Positionierung A |
| TikTok/YouTube mit Gesicht | Gründer will kein Gesicht zeigen | – | – | ❌ |
| Meta-/Reddit-Ads | zu teuer für 18-28 € Beitrag ohne Testdaten | – | – | ❌ bis organisch etwas funktioniert |

### 3. Die 30-Tage-Kampagne

**Launch-Termin (Vorschlag, wird in `/founder-launch` festgelegt): Montag, 11. Jänner 2027.** Begründung: Vor dem Start müssen Beispiel-Report, Formeln, Export und Impressum fertig sein (`offer.md`); im Jänner planen viele ihre Finanzen. Gründungsmitglieder-Angebot: 19 €/Jahr dauerhaft für die ersten 100, **endet am 11. Februar 2027 oder bei 100 Plätzen**. Preis-Test: nach dem Gründungs-Kontingent 29 €.

| Datum | Kanal | Was |
| --- | --- | --- |
| Mo 28.12. | Reddit | Account aufbauen: 3 hilfreiche Antworten auf Fragen zu Vorsorgewohnungen, ohne Link |
| Di 29.12. | Instagram | Profil anlegen, Bio: „Wohnungen durchgerechnet. Österreichisch. Ohne Verkaufsinteresse.“ |
| Mi 30.12. | Website | Beispiel-Report (echte Wiener Wohnung) online, Warteliste |
| Do 31.12. | Instagram | Post 1: Hook 1 (Kaufnebenkosten einzeln) |
| Sa 2.1. | Reddit | 3 Antworten mit Rechenweg, kein Link |
| Mo 4.1. | Instagram | Post 2: Hook 3 (Cashflow negativ, Vermögen positiv) |
| Di 5.1. | Reddit | Eigener Beitrag (falls Regeln erlauben): „Ich habe eine Wiener Vorsorgewohnung komplett durchgerechnet, hier jede Position“, Link nur zum Beispiel-Report, offen als Gründer gekennzeichnet |
| Mi 6.1. | Instagram | Post 3: Hook 5 (Beleihungsauslauf erklärt) |
| Fr 8.1. | E-Mail | Warteliste: „Montag geht's los, Gründungsmitglieder 19 €“ |
| Sa 9.1. | Instagram | Post 4: Hook 2 (Excel gegenchecken) |
| **Mo 11.1.** | alle | **Launch**: Instagram-Post, Reddit-Kommentar im eigenen Thread, Warteliste-Mail |
| Di 12.1. | Instagram | Story-Serie: Score von 0-100 erklärt (Hook 6) |
| Do 14.1. | Reddit | Antworten auf Fragen; Erkenntnisse aus dem Launch teilen |
| Fr 15.1. | Instagram | Post 5: Hook 4 (Mietpreisdeckel Altbau) |
| Mo 18.1. | Google Ads | Test startet: 200 € Limit, 2 Anzeigen (Hook 7, Hook 8) |
| Di 19.1. | Instagram | Post 6: „Wohnung des Monats durchgerechnet“ (neues Inserat, anonymisiert) |
| Do 21.1. | Reddit | Antworten; kein neuer Eigenbeitrag (90/10) |
| Fr 22.1. | Instagram | Post 7: Hook 9 (Gründungsmitglied) |
| Mo 25.1. | alle | Zwischenstand auswerten (Abschnitt 5); stoppen, was nicht wirkt |
| Mi 27.1. | Instagram | Post 8: Hook 10 (Fragen fürs Bankgespräch) |

**Wenn es nichts Neues gibt:** „Wohnung des Monats“ (ein öffentliches Inserat durchgerechnet), „Begriff der Woche“ (AfA, Beleihungsauslauf, DSCR), „Was sich 2026/27 geändert hat“ (Gebühren, Mietpreisdeckel), Einblicke in die Rechenlogik (Formel einer Kennzahl).

### 4. Zehn Hooks (jeder beantwortet einen Panel-Einwand)

1. „Diese Wohnung kostet 142.000 €. Die Rechnung kostet dich 158.130 €. Hier ist jede Position.“ → Kaufnebenkosten, Blackbox
2. „Dein Excel sagt plus? Leg es neben diesen Report und schau, Zeile für Zeile, wo es abweicht.“ → „Mein Excel reicht“
3. „Cashflow -60 € im Monat und trotzdem +137 € Vermögen. So geht das.“ → Verständnis
4. „Altbau in Wien? Dann bestimmt der Mietpreisdeckel deine Rendite, nicht der Makler.“ → AT-Genauigkeit
5. „Beleihungsauslauf 126 %: was die Bank damit meint, bevor du hingehst.“ → „Bank rechnet eh“
6. „Score 59,9 von 100. So entsteht die Zahl, Formel für Formel.“ → Blackbox
7. Anzeige: „Vorsorgewohnung durchrechnen: österreichische Nebenkosten, Cashflow nach Steuer, PDF für die Bank.“ → Suchmoment
8. Anzeige: „Bevor du unterschreibst: unabhängiger Kauf-Check. Beispiel-Report ohne Anmeldung.“ → Vertrauen, keine Gratisversion
9. „Die ersten 100 zahlen dauerhaft 19 € im Jahr. Danach nicht mehr.“ → echtes Eröffnungsangebot
10. „7 Fragen, die du der Bank vor der Unterschrift stellen solltest.“ → Bankgespräch

Hook 1, 3, 5 und 6 nutzen Zahlen aus dem Beispiel-Report Hasnerstraße 68; nur mit Einwilligung bzw. anonymisiert verwenden. Keine Panel-Zitate in Werbung, keine erfundenen Bewertungen, keine Renditeversprechen.

### 5. Budget und Zahlen

**Budget (Basis 500 €):** 200 € Google-Search-Test, 0 € Reddit/Instagram (organisch), 300 € Reserve, die nur in den Kanal geht, der den Test besteht. Obergrenze 1.000 €.

**Höchstens zahlbar für einen Kunden (CAC):** Beitrag pro Kunde × Käufe im ersten Jahr. Panel: 1,0 Käufe pro Käufer im ersten Monat, Jahresabo = 1 Kauf/Jahr.
- bei 19 €: 18,33 € × 1 = **max. 18 €**
- bei 29 €: 28,33 € × 1 = **max. 28 €**
- Abzüglich Garantie-Erstattungen (unbekannte Quote) ist der echte Spielraum kleiner. Verlängerungen würden ihn erhöhen, sind aber unbelegt.

**Drei Zahlen, jede Woche:**
| Zahl | Ziel | „Etwas ändern“, wenn |
| --- | --- | --- |
| Besucher auf der Beispiel-Report-Seite | 100+/Woche ab Launch | < 50 zwei Wochen in Folge |
| Anteil Besucher, die zahlen | ≥ 2 % | < 1 % nach 200 Besuchern |
| Werbekosten pro zahlendem Kunden | < 18 € (19 €) / < 28 € (29 €) | darüber nach 100 € Ausgaben → Anzeige stoppen |

Das sind Werbe- und Rechtsfragen in Österreich (UWG, Preisangaben, Widerrufsrecht bei digitalen Inhalten): vorher prüfen, keine Rechtsberatung.

## Brand

Grundlage: Positionierung A aus `marketing.md` („unabhängiger Kauf-Check nach österreichischen Regeln, jede Zahl offengelegt“), `competitors.md`, Panel-Re-Test, Screenshots der App vom 18.10.2026. Die App heißt schon **Marille**; dieser Schritt prüft, ob der Name trägt, statt ihn zu ersetzen.

### 1. Namenskandidaten

| # | Name | Stil | was er sagt | laut / als Icon | Risiko |
| --- | --- | --- | --- | --- | --- |
| 1 | **Marille** | evokativ, österreichisch | Marille ist das österreichische Wort für Aprikose: sofort „von hier“, warm, nicht bankig | weich, zweisilbig, leicht zu merken; „M“ als Icon | Alltagswort, daher schwer allein als Marke zu schützen; keine Aussage über Immobilien; viele Gastro-/Produkt-Treffer bei Suchen |
| 2 | Immo-Cashflow | beschreibend | genau was es tut | sperrig | **schon App-Name** ([Immo Cashflow](https://apps.apple.com/at/app/immo-cashflow/id6553989584)) → raus |
| 3 | Kaufcheck | beschreibend | der Moment vor der Unterschrift | klar, aber generisch | kaum schützbar |
| 4 | Gegenrechnung | beschreibend-evokativ | prüft die Rechnung von Bank/Makler | lang | lang für ein Icon |
| 5 | Grundbuch | Ort/Begriff | österreichischer Rechtsbegriff | stark | Behördenbegriff, verwechselbar, nicht schützbar |
| 6 | Zinshaus | Ort | Wiener Immobilienkultur | gut | falsche Zielgruppe (Zinshaus ≠ Erstinvestor) |
| 7 | Vorsorgerei | erfunden | Vorsorgewohnung + Handwerk | verspielt | klingt nach Versicherung |
| 8 | Klarrechnung | erfunden | Klarheit, Offenlegung | eindeutig | prüfen, ob belegt |
| 9 | Belegt | evokativ | „jede Zahl belegt“ | kurz | Alltagswort, Doppelbedeutung |
| 10 | Marille Kauf-Check | Marke + Produkt | warmer Name + was es tut | gut, auch als Ad-Headline | erbt die Risiken von 1 |

**Shortlist:** Marille (behalten), Marille Kauf-Check (als Produktname, nicht als Firmenname), Klarrechnung (Ausweichname, falls Marille markenrechtlich nicht geht).

**Empfehlung:** **Marille** als Marke, **„Marille Kauf-Check“** als Name des Angebots. Der Name passt zur Positionierung (österreichisch, nicht Bank, nicht Makler) und ist bereits in der App, im PDF und im Logo.

### 2. Prüfungen, die du selbst machen musst

Ich kann nur öffentlich suchen; aus diesem Container sind auch Domains nicht erreichbar. Eine Markenanwältin oder ein Markenanwalt bestätigt das Ergebnis, und **nichts ist geschützt, bevor du es anmeldest**.

- **Marke:** Suche nach „Marille“ in
  - Österreich: [see.ip / Österreichisches Patentamt](https://see.ip.gv.at)
  - EU: [EUIPO eSearch](https://euipo.europa.eu/eSearch/) und [TMview](https://www.tmdn.org/tmview/)
  - **Klassen:** 9 (herunterladbare Software/Apps), 36 (Finanzdienstleistungen, Immobilienwesen), 42 (Software as a Service).
  - Bei einer Websuche fand ich keine Finanz-/Immo-App namens Marille; das ersetzt keine Registersuche.
- **Domains:** marille.at, marille.app, marille.com, und als Ausweichen getmarille.at, marille-check.at, kaufcheck-marille.at. Prüfen z. B. bei [nic.at](https://www.nic.at). Heute läuft die App auf `marille.netlify.app`; für Impressum, Vertrauen und E-Mail brauchst du eine eigene Domain (Kosten nennen, dann kommt sie in den CFO).
- **Handles:** Instagram, Reddit, TikTok, X, YouTube: `@marille`, `@marille.at`, `@marille_kaufcheck`.
- **Verwechslung:** Kein Konkurrent aus `competitors.md` heißt ähnlich. „Immo Cashflow“ als Arbeitsname nicht mehr verwenden.

### 3. Versprechen und Stimme

**Versprechen (in einem Satz):** Bei Marille siehst du jede Zahl, woher sie kommt und was sie für dein Konto heißt, bevor du unterschreibst.

**Tagline (drei Optionen):**
1. **„Erst rechnen, dann unterschreiben.“** (empfohlen)
2. „Jede Zahl belegt. Österreichisch gerechnet.“
3. „Deine Wohnung, ehrlich durchgerechnet.“

**Stimme:**

| Adjektiv | so | nicht so |
| --- | --- | --- |
| **ehrlich** | „Diese Wohnung kostet dich 60 € im Monat.“ | „Top-Investment mit Potenzial!“ |
| **erklärend** | „Beleihungsauslauf heißt: so viel leiht dir die Bank im Verhältnis zum Wert, den sie der Wohnung gibt.“ | „LTV 126 % – kritisch.“ ohne Erklärung |
| **ruhig österreichisch** | du-Form, „Jänner“, „Grundbuch“, keine Anglizismen, wo es ein Wort gibt | Hype, Ausrufezeichen, „Cashflow-Maschine“ |

**Vorher/nachher (eine Zeile aus `pitch.md`):**
- vorher: „Du siehst jede Kaufnebenkosten-Position einzeln (…), deinen Cashflow nach Kreditrate und Steuer, was die Tilgung an Vermögen aufbaut, Bank-Kennzahlen wie Beleihungsauslauf und einen Score von 0 bis 100.“
- nachher: „Du siehst, was die Wohnung wirklich kostet, was dir jeden Monat bleibt, und warum. Jede Zahl lässt sich aufklappen.“

### 4. Der Look (Brief)

Die App hat schon eine klare Richtung (Pergament-Hintergrund, Waldgrün, Gold, Serifen-Überschriften). Dieser Brief schreibt sie fest und korrigiert den Kontrast.

**Farben** (Hex-Werte als Vorschlag, nah an den Screenshots; an die echten App-Werte anpassen):

| Farbe | Hex | Aufgabe | Kontrast (WCAG) |
| --- | --- | --- | --- |
| Tinte | #1E2420 | Text | 14,2:1 auf Pergament ✅ AAA |
| Pergament | #F7F2E7 | Hintergrund | – |
| Waldgrün | #2E5E3E | Aktionen, positive Zahlen | 6,8:1 auf Pergament ✅ AA; Weiß auf Waldgrün 7,5:1 ✅ |
| Marillengold | #B8892E | Akzent, Flächen, Linien | **2,8:1 auf Pergament ❌ nicht für Text**; Tinte auf Gold 5,0:1 ✅ |
| Warnrot | #A3343A | negative Zahlen | 6,1:1 auf Pergament ✅ |

⚠️ Im PDF-Report steht die Gesamtinvestition in Gold auf hellem Grund. Gold als Textfarbe auf Pergament fällt durch AA; für Zahlen Tinte oder Waldgrün nehmen, Gold nur für Flächen und Linien. Rot/Grün nie als einzige Unterscheidung (Vorzeichen +/− immer mitschreiben, wie es die App schon tut).

**Schrift** (beide kostenlos, SIL Open Font License, über [Google Fonts](https://fonts.google.com)):
- Überschriften: **Cormorant Garamond** oder **Playfair Display** (Serife, passt zu den Screenshots).
- Text und Zahlen: **DM Sans** (gut lesbare Ziffern). Für Tabellen „tabular figures“ einschalten.
Falls die App schon andere Schriften nutzt: Lizenz prüfen, sonst diese.

**Logo-Brief:**
- Muss sagen: österreichisch, ruhig, vertrauenswürdig; kein Bank-Look, kein Hausdach-Klischee.
- Muss funktionieren: als 32-px-App-Icon, als Favicon, im PDF-Kopf, auf Instagram-Grafiken.
- Heute: Wortmarke „Marille.“ mit goldenem Punkt. Das funktioniert als Wortmarke; fürs Icon fehlt ein Zeichen (z. B. ein „M“ oder eine reduzierte Marillen-Form im Waldgrün).
- Vermeiden: Häuser, Schlüssel, Euro-Zeichen, Pfeile nach oben (Renditeversprechen).
- Ich habe hier kein Bildwerkzeug; erzeugte Entwürfe wären Konzepte, kein fertiges Logo.

**Die ersten fünf Berührungspunkte:**
1. **Startseite:** Tagline, ein Satz zum Ergebnis, Button „Beispiel-Report ansehen (ohne Anmeldung)“, darunter Gründer mit Namen und Impressum-Link.
2. **Beispiel-Report:** derselbe Look wie das PDF, mit aufklappbaren Formeln.
3. **Kaufbestätigung (E-Mail):** „Danke. Du bist Gründungsmitglied Nr. X und zahlst 19 € pro Jahr, solange du verlängerst. 30 Tage Geld zurück: einfach auf diese Mail antworten.“
4. **Erster Instagram-Post:** Hook 1 (Kaufnebenkosten einzeln, Hasnerstraße-Zahlen, anonymisiert).
5. **Antwort auf die erste Beschwerde:** Danke, Fehler benennen, Rechenweg zeigen, korrigieren oder Geld zurück anbieten, innerhalb von 24 Stunden.

## Operations

Ein Gründer, 5 Stunden pro Woche, eine Web-App. Es gibt keinen Laden und keine Lieferung; „Betrieb“ heißt hier: Zahlungen, Support, Richtigkeit der Zahlen, Daten, Recht.

### 1. Der wiederkehrende Ablauf (Woche statt Tag)

Kunde sieht es = 👁

| wann | was | 👁 |
| --- | --- | --- |
| laufend, automatisch | Besucher sieht Beispiel-Report → zahlt per Stripe → Konto wird freigeschaltet → Bestätigungs-E-Mail | 👁 |
| täglich, 10 min | Support-Postfach lesen; Erstattungswünsche sofort erledigen (Garantie) | 👁 |
| täglich, 5 min | Stripe-Dashboard: neue Zahlungen, fehlgeschlagene Zahlungen | |
| wöchentlich, 1 h | Marketing: 2 Instagram-Grafiken, Reddit-Antworten (`marketing.md`) | 👁 |
| wöchentlich, 30 min | Die drei Zahlen aus `marketing.md` eintragen | |
| wöchentlich, 2-3 h | Produkt: Fehler beheben, eine Verbesserung | 👁 |
| monatlich, 30 min | Gesetzes- und Gebührenänderungen prüfen (Grunderwerbsteuer, Eintragungsgebühr, Mietpreisdeckel, AfA); Beispiel-Report aktualisieren | 👁 |
| monatlich, 15 min | Belege ablegen (Stripe-Auszahlungen, Abo-Rechnungen) | |

**Zeitbudget:** Das sind schon ca. 4-5 Stunden pro Woche. Bauen (Beispiel-Report, Formeln, Export) passt **vor** dem Launch, danach bleibt wenig Luft.

### 2. Lieferanten (die „Zutaten“ einer Software)

| Bedarf | Anbieter | Preis | Bemerkung |
| --- | --- | --- | --- |
| Zahlungen | Stripe (gewählt) | 1,5 % + 0,25 € pro EWR-Standardkarte ([Drittquelle](https://www.ki-syndikat.de/tools/stripe/)); EPS 1,6 % + 0,25 € ([alloq](https://alloq.digital/de/blog/stripe-integration-oesterreich/)) | Abo-Gebühr (Stripe Billing) im Dashboard prüfen |
| Hosting | Netlify (heute) | 8 €/Monat (Gründer) | – |
| Datenbank/Login | Supabase (EU-Region, Gratis-Tarif) | 0 € (Gründer) | Gratis-Tarif hat Grenzen; ab wann ein Bezahltarif nötig ist, auf der Supabase-Preisseite prüfen |
| Domain + E-Mail | OVHcloud oder Hostinger | .at ab 12,08 € im 1. Jahr, 13,48 € Verlängerung, Starter-E-Mail inkl. ([OVHcloud](https://www.ovhcloud.com/de/domains/tld/at/)); Hostinger 11,99 € im 1. Jahr ([Hostinger](https://www.hostinger.com/at/tld/at-domain)) | ab 1.10.2026 Telefonnummer bei Neuregistrierung Pflicht ([nic.at](https://www.nic.at/en/news/nic-at/nisg-2026-whats-changing-for-at-domains-as-of-1-october-2026)) |
| Entwicklung | Claude (heute) | 22 €/Monat (Gründer) | – |
| Steuerberatung | Angebot einholen | **offen** | Fixpreis für EPU-Gründung + Jahresabschluss anfragen |
| Rechtstexte (AGB, Datenschutz, Widerruf) | Generator der WKO oder Anwalt | **offen** | WKO-Mitglieder haben Musterverträge |

`numbers.json` ist um die Domain (1,12 €/Monat) ergänzt; der CFO-Bericht ist neu gerechnet (Jahr 1: 543 € vor Werbung, +43 € nach 500 € Werbung).

### 3. Menschen

| Rolle | wer | Stunden | Lohn |
| --- | --- | --- | --- |
| alles | Gründer | 5 h/Woche | 0 € (Wunsch des Gründers) |
| Rechenlogik-Prüfung | Steuerberatung (extern, einmalig) | – | Angebot offen |

**Erster Monat nach Launch:** 1 h Support/Zahlungen, 2 h Marketing, 2 h Produkt. Wenn Support mehr als 1 h pro Woche braucht, ist das das Signal, die Hilfe-Texte zu verbessern, nicht mehr Stunden.

### 4. Routinen (SOPs)

**A. Neuer Kunde (automatisch, einmal testen)**
1. Kunde zahlt bei Stripe. 2. Stripe-Webhook schaltet das Konto frei. 3. Bestätigungs-E-Mail mit Gründungsmitglied-Nummer und Garantie-Hinweis. 4. Test: einmal im Monat selbst mit Testkarte durchspielen.

**B. Erstattung (Garantie)**
1. Kunde schreibt innerhalb von 30 Tagen. 2. Ohne Rückfrage in Stripe erstatten. 3. Antwort: „Erledigt. Darf ich fragen, was gefehlt hat?“ 4. Grund in eine Liste eintragen. 5. Konto zum Ende der Laufzeit sperren, Daten auf Wunsch löschen.

**C. Rechenfehler gemeldet** (der wichtigste Ablauf)
1. Innerhalb von 24 h antworten: Danke, prüfe ich. 2. Nachrechnen mit Quelle. 3. Wenn Fehler: korrigieren, allen betroffenen Kunden schreiben, im Changelog sichtbar machen, Erstattung anbieten. 4. Wenn kein Fehler: Rechenweg und Quelle schicken. 5. Testfall ergänzen, damit der Fehler nicht wiederkommt.

**D. Monatliche Regel-Prüfung**
1. Grunderwerbsteuer, Eintragungsgebühr, Pfandrecht, AfA-Sätze, Mietpreisdeckel/Richtwert auf den offiziellen Seiten prüfen. 2. Bei Änderung: App anpassen, Datum „Stand“ im Report aktualisieren, Instagram-Post dazu.

**E. Ausfall**
1. Netlify-/Supabase-Statusseite prüfen. 2. Kurze Notiz auf der Startseite. 3. Betroffene Kunden informieren, wenn länger als 24 h.

### 5. Werkzeuge

| Aufgabe | Werkzeug | Preis |
| --- | --- | --- |
| Zahlung, Abo, Rechnung | Stripe Checkout + Billing + Kundenportal (Kündigung selbst) | Gebühren wie oben |
| Hosting/Datenbank | Netlify, Supabase (EU) | 8 € / 0 € |
| E-Mail | im Domain-Paket | inkl. |
| Buchhaltung | Einnahmen-Ausgaben-Liste (Tabelle) reicht bei diesem Umsatz; Steuerberatung fragen | 0 € |
| Kennzahlen | Netlify Analytics oder ein datensparsames Tool | prüfen |

### 6. Gewerbe, Steuer, Recht (Checkliste)

Regeln ändern sich und hängen vom Einzelfall ab. Jeden Punkt bei der Behörde, der WKO oder einer Steuerberatung bestätigen. Keine Rechtsberatung.

- [ ] **Gewerbe anmelden:** Software verkaufen ist als freies Gewerbe „Dienstleistungen in der automatischen Datenverarbeitung und Informationstechnik“ möglich, ohne Befähigungsnachweis ([WKO](https://www.wko.at/wien/information-consulting/unternehmensberatung-buchhaltung-informationstechnologie/it-dienstleistung/unternehmensgruendung)); online über GISA ([Land OÖ](https://www.land-oberoesterreich.gv.at/543382.htm)). Vorher NeuföG-Bestätigung holen, sonst keine Gebührenbefreiung.
- [ ] **⚠️ Abgrenzung zur Beratung:** Marille zeigt einen Investment-Score und Texte wie „Geh früh ins Bankgespräch“. Klären, dass das eine Rechenhilfe ist und keine Vermögens-, Anlage- oder Kreditberatung (die in Österreich reglementiert sind). Ich habe dazu keine Primärquelle gefunden; **bei der WKO oder einem Anwalt fragen, bevor du verkaufst.** Haftungsausschluss in AGB und im Report.
- [ ] **Finanzamt:** Betriebseröffnung innerhalb eines Monats nach Gewerbeanmeldung anzeigen ([TPA](https://www.tpa-group.at/app/uploads/2023/07/TPA-Steuerberatung-Start_up_Schritte_eigenes_Unternehmen_2022.pdf)).
- [ ] **Umsatzsteuer:** Kleinunternehmerregelung bis 55.000 € Bruttoumsatz ([USP](https://www.usp.gv.at/themen/steuern-finanzen/umsatzsteuer-ueberblick/weitere-informationen-zur-umsatzsteuer/weitere-steuertatbestaende-und-befreiungen/kleinunternehmen.html), [WKO](https://www.wko.at/vlbg/steuern/kleinunternehmerregelung-in-oesterreich-und-der-eu)). Bei digitalen Leistungen an Privatkunden in anderen EU-Ländern gelten eigene Regeln: fragen.
- [ ] **Sozialversicherung (SVS):** Ausnahme von der Pflichtversicherung möglich bei Einkünften unter 6.613,20 € und Umsatz unter 55.000 € (2026, [WKO Wien](https://www.wko.at/wien/gruendung/sozialversicherung-fuer-gruendung-in-wien-svs.pdf)); Antrag nötig.
- [ ] **WKO-Mitgliedschaft und Grundumlage:** mit Gewerbe automatisch; Höhe bei der WKO erfragen (**offen**, kommt in den CFO).
- [ ] **Impressum** (E-Commerce-Gesetz, Mediengesetz), **Datenschutzerklärung** (DSGVO), **AGB**, **Widerrufsbelehrung** für digitale Inhalte.
- [ ] **DSGVO:** Verarbeitungsverzeichnis; Auftragsverarbeitungsverträge mit Supabase, Netlify, Stripe; Löschung auf Wunsch.
- [ ] **Versicherung:** Vermögensschaden-/Berufshaftpflicht für Software, falls eine falsche Berechnung Schaden verursacht: **Angebot einholen (offen)**.

### 7. Risikoregister

| # | Risiko | Wahrsch. | Schaden | Plan |
| --- | --- | --- | --- | --- |
| 1 | **Rechenfehler** in Steuer, Nebenkosten oder Mietpreisdeckel | mittel | hoch (Vertrauen ist das Produkt) | Testfälle gegen echte Kaufverträge; SOP C; Steuerberater-Prüfung, sobald leistbar |
| 2 | Gesetz/Gebühr ändert sich, App rechnet alt | mittel | hoch | SOP D monatlich; „Stand“-Datum im Report |
| 3 | Marille gilt rechtlich als Beratung | niedrig-mittel | hoch | vor Launch WKO/Anwalt; Formulierungen als Rechenhilfe |
| 4 | Zu wenig Besucher | hoch | mittel | Wochenzahlen aus `marketing.md`; nach 2 Wochen < 50 Besucher Kanal wechseln |
| 5 | Datenpanne (Kreditdaten) | niedrig | hoch | Supabase Row-Level-Security prüfen; nur nötige Daten speichern; Meldepflicht 72 h kennen |
| 6 | Gründer hat keine Zeit (Job, Krankheit) | mittel | mittel | Autopilot: Zahlung und Zugang laufen ohne dich; Support-Antwortzeit auf der Website ehrlich nennen |
| 7 | Supabase-Gratis-Tarif reicht nicht mehr | niedrig bei 50 Kunden | niedrig | Grenzen kennen; Bezahltarif in CFO, sobald nahe |
| 8 | Konkurrent kopiert (Optifin, Primus Vision, Parqet) | mittel | mittel | Vorsprung über Offenlegung und Vertrauen, nicht Funktionen |
| 9 | Viele Erstattungen | mittel | mittel | Gründe sammeln; ab 20 % Angebot oder Zielgruppe ändern |
| 10 | Reddit-Beiträge als Spam entfernt, Account gesperrt | mittel | niedrig | Regeln jedes Subreddits lesen; 90/10; offen als Gründer auftreten |

### Offene Fragen (bitte Angebote/Zahlen einholen)

1. Steuerberatung: Fixpreis Gründung + Jahresabschluss.
2. WKO-Grundumlage für dein Gewerbe.
3. Haftpflichtversicherung: Prämie.
4. Abgrenzung Rechenhilfe vs. Beratung: Auskunft WKO/Anwalt.

## Launch plan

Start: **Montag, 11. Jänner 2027** (vom Gründer bestätigt). Heute: Sonntag, 18. Oktober 2026. Das sind 12 Wochen mit je 5 Stunden, also rund **60 Stunden**. Owner jeder Aufgabe ist der Gründer, außer es steht etwas anderes dabei.

### 1. Der echte Test zuerst: Vorverkauf für Gründungsmitglieder

**Was:** eine Landingpage mit dem Beispiel-Report (ohne Anmeldung), Preis und Button „Jetzt Gründungsmitglied werden“. Bezahlt wird sofort per Stripe; der Zugang startet am 11. Jänner. Wenn der Launch nicht stattfindet, gibt es das Geld zurück (so auf der Seite schreiben).

**Preis-Test:** Besucher werden zufällig auf **19 €** oder **29 €** pro Jahr verteilt (`pricing.md`). Gründungsmitglieder behalten ihren Preis, solange sie verlängern.

**Zeitraum:** Montag, 16. November, bis Sonntag, 13. Dezember 2026 (4 Wochen).

**Erfolgslinie (vorher festgelegt):**
- ✅ **Weiter wie geplant:** mindestens **10 bezahlte Vorbestellungen** und mindestens **2 %** der Besucher zahlen, bei mindestens 300 Besuchern.
- ⚠️ **Nachschärfen:** 5-9 Vorbestellungen oder 1-2 % → Hooks und Kanäle tauschen (`/founder-marketing`), Launch bleibt.
- ❌ **Zurück an den Start:** unter 5 Vorbestellungen bei 300+ Besuchern → zurück zu `/founder-offer` oder `/founder-pricing`, Launch verschieben.
- Bei weniger als 300 Besuchern ist das Ergebnis nicht aussagekräftig: Problem ist dann die Reichweite, nicht das Angebot.

**Vergleich mit dem Panel:** Das Panel ergab 45 % Kaufbereitschaft bei Leuten, die den Pitch lesen und genau in der Zielgruppe sind. Das ist **nicht** mit der Besucher-Quote vergleichbar (die meisten Besucher sind nicht mitten in einer Besichtigung). Vergleichbar ist: Welche Einwände kommen in Mails und Kommentaren, und welcher Preis gewinnt. Wenn echte Käufer deutlich schlechter abschneiden, gilt der echte Käufer.

### 2. Countdown (Wochenblöcke)

🔴 = kritischer Pfad (verschiebt den Launch, wenn es rutscht)

| Woche ab | Aufgabe | Deadline |
| --- | --- | --- |
| **Mo 19.10.** | 🔴 WKO-Gründerservice anfragen: Gewerbe IT-Dienstleistung + **Abgrenzung Rechenhilfe vs. Beratung** (`ops.md`) | Fr 23.10. |
| | Markenregister prüfen: „Marille“ in Klassen 9, 36, 42 (`brand.md`) | So 25.10. |
| | Domain registrieren (marille.at o. ä.), E-Mail einrichten | So 25.10. |
| **Mo 26.10.** | 🔴 NeuföG-Bestätigung, Gewerbe über GISA anmelden | Fr 30.10. |
| | Steuerberatung: 2 Angebote anfragen (Fixpreis Gründung + Jahr) | Fr 30.10. |
| **Mo 2.11.** | 🔴 Impressum, Datenschutzerklärung, AGB mit Haftungsausschluss, Widerrufsbelehrung | So 8.11. |
| | Betriebseröffnung beim Finanzamt (innerhalb 1 Monat nach Gewerbe) | So 8.11. |
| | SVS-Ausnahme beantragen, falls zutreffend | So 8.11. |
| **Mo 9.11.** | 🔴 Beispiel-Report öffentlich (Wiener Wohnung, anonymisiert oder mit Erlaubnis) | Mi 11.11. |
| | 🔴 Stripe live: Checkout mit 19 €/29 €-Varianten, Testzahlung | Fr 13.11. |
| | Landingpage mit Gründer-Seite, Tagline „Erst rechnen, dann unterschreiben.“ | So 15.11. |
| **Mo 16.11.** | **Vorverkauf startet**; Reddit-Account aufbauen (nur Hilfe, keine Links) | laufend |
| | Instagram-Profil, 2 Grafiken/Woche | laufend |
| **Mo 23.11.** | Bauen: **Formel und Quelle bei jeder Zahl** | So 6.12. |
| **Mo 30.11.** | Reddit-Beitrag mit Beispiel-Report (wenn Subreddit-Regeln es erlauben) | Di 1.12. |
| **Mo 7.12.** | Bauen: **Excel/CSV-Export** | So 20.12. |
| | **Vorverkauf endet So 13.12.** → Auswertung gegen Erfolgslinie | Mo 14.12. |
| **Mo 14.12.** | 🔴 **Entscheidung**: weiter / nachschärfen / zurück (Abschnitt 1) | Mo 14.12. |
| **Mo 21.12.** | Testfälle gegen 2-3 echte Kaufverträge (eigene Wohnungen); Fehler beheben | So 27.12. |
| **Mo 28.12.** | Marketing-Kalender startet (`marketing.md`, L-14) | laufend |
| **Mo 4.1.** | 🔴 **Soft Open:** Vorbesteller bekommen Zugang 1 Woche früher, Feedback einsammeln | Fr 8.1. |
| | Bestätigungs-Mail, Erstattungs-Ablauf, Kundenportal testen (SOP A, B) | Fr 8.1. |
| **Mo 11.1.** | **Launch** | |

**Puffer:** Wenn bis Mo 14.12. Formeln **oder** Export nicht fertig sind: Launch mit dem, was fertig ist, und den Pitch ehrlich anpassen (nichts versprechen, was es nicht gibt). Wenn die WKO-Auskunft zur Beratung negativ ist: Launch verschieben, bis die Formulierungen geklärt sind.

### 3. Launch-Tag: Montag, 11. Jänner 2027

Zeiten anpassen, falls du tagsüber arbeitest; die Reihenfolge ist wichtiger als die Uhrzeit.

| Zeit | was | Kanal |
| --- | --- | --- |
| 07:00 | Zahlung mit echter Karte testen, Erstattung testen | Stripe |
| 07:30 | Startseite: Gründungsmitglied-Zähler „X von 100“ (echte Zahl) | Website |
| 08:00 | Mail an Warteliste und Vorbesteller: „Ab heute offen“ | E-Mail |
| 08:15 | Launch-Post (Hook 1) | Instagram |
| 12:00 | Antworten auf Reddit im eigenen Thread; keine neuen Werbeposts | Reddit |
| 12:30 | Support-Postfach, Erstattungen sofort | E-Mail |
| 18:00 | Story: Score erklärt (Hook 6) | Instagram |
| 21:00 | Zahlen notieren: Besucher, Käufe, Erstattungen, Fragen | Tabelle |

**Wenn etwas bricht** (aus dem Risikoregister in `ops.md`):
- Zahlung geht nicht → Stripe-Status prüfen, Hinweis auf Startseite, Warteliste-Link statt Kauf.
- Rechenfehler gemeldet → SOP C (24 h, Korrektur öffentlich, Erstattung anbieten).
- App down → Netlify/Supabase-Status, Notiz auf Startseite.

### 4. Die ersten 30 Tage

**Jede Woche (Montag) eintragen:**

| Zahl | Ziel | Auslöser für eine Änderung |
| --- | --- | --- |
| neue zahlende Kunden pro Woche | ≥ 1 (Break-even ≈ 2 pro Monat; Ziel Jahr 1: 50, ca. 4-5 pro Monat) | 0 in zwei Wochen in Folge |
| Besucher Beispiel-Report | 100+ | < 50 zwei Wochen in Folge |
| Besucher → Kauf | ≥ 2 % | < 1 % nach 200 Besuchern |
| Werbekosten pro Kunde (ab Google-Test 18.1.) | < 18 € / < 28 € | darüber nach 100 € → Anzeige stoppen |
| Erstattungsquote | < 10 % | > 20 % |

**Rückblicke:**
- **Tag 7 (Mo 18.1.):** Kommt Verkehr an? Welche Hooks klicken? Welche Einwände kommen in Mails? Google-Test starten oder nicht?
- **Tag 14 (Mo 25.1.):** Welcher Preis (19 € / 29 €) gewinnt? Stoppen, was nicht wirkt. Gibt es Rechenfehler-Meldungen?
- **Tag 30 (Mi 10.2.):** Auf Kurs zu 50 Kunden in Jahr 1? Gründungsangebot endet am **Do 11.2.** (oder bei 100 Plätzen): Preis danach festlegen. Was bauen als Grund zu verlängern (Portfolio, E1b-Hilfe)? `numbers.json` mit echten Zahlen aktualisieren und `/founder-cfo` neu laufen lassen.

_The panel is simulated buyers and the numbers are projections from your inputs. Confirm demand with real customers and costs with real quotes before you spend. Not financial, legal or tax advice._
