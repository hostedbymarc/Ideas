# Betrieb: Marille

Ein Gründer, 5 Stunden pro Woche, eine Web-App. Es gibt keinen Laden und keine Lieferung; „Betrieb“ heißt hier: Zahlungen, Support, Richtigkeit der Zahlen, Daten, Recht.

## 1. Der wiederkehrende Ablauf (Woche statt Tag)

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

## 2. Lieferanten (die „Zutaten“ einer Software)

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

## 3. Menschen

| Rolle | wer | Stunden | Lohn |
| --- | --- | --- | --- |
| alles | Gründer | 5 h/Woche | 0 € (Wunsch des Gründers) |
| Rechenlogik-Prüfung | Steuerberatung (extern, einmalig) | – | Angebot offen |

**Erster Monat nach Launch:** 1 h Support/Zahlungen, 2 h Marketing, 2 h Produkt. Wenn Support mehr als 1 h pro Woche braucht, ist das das Signal, die Hilfe-Texte zu verbessern, nicht mehr Stunden.

## 4. Routinen (SOPs)

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

## 5. Werkzeuge

| Aufgabe | Werkzeug | Preis |
| --- | --- | --- |
| Zahlung, Abo, Rechnung | Stripe Checkout + Billing + Kundenportal (Kündigung selbst) | Gebühren wie oben |
| Hosting/Datenbank | Netlify, Supabase (EU) | 8 € / 0 € |
| E-Mail | im Domain-Paket | inkl. |
| Buchhaltung | Einnahmen-Ausgaben-Liste (Tabelle) reicht bei diesem Umsatz; Steuerberatung fragen | 0 € |
| Kennzahlen | Netlify Analytics oder ein datensparsames Tool | prüfen |

## 6. Gewerbe, Steuer, Recht (Checkliste)

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

## 7. Risikoregister

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

## Offene Fragen (bitte Angebote/Zahlen einholen)

1. Steuerberatung: Fixpreis Gründung + Jahresabschluss.
2. WKO-Grundumlage für dein Gewerbe.
3. Haftpflichtversicherung: Prämie.
4. Abgrenzung Rechenhilfe vs. Beratung: Auskunft WKO/Anwalt.
