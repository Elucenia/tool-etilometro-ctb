<!-- ELUCENIA technical documentation · etilometro-ctb · de · no clinical/professional/rights approval -->

# Atemalkoholmessgerät: berücksichtigter Wert (brasilianische Contran-Resolution 432)

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/etilometro-ctb)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Atemalkoholmessung (MR)

`mr`

mg/L Luft · Bereich: 0–5

## Fassung der Methode

CONTRAN 432/2013 Anhang I: Fehler 0,032/8%/30%; Abschneiden auf 2 Dezimalstellen; Brasilien

## Dokumentierte Formel

VC = MR − EM, mit zwei Dezimalstellen; weitere werden abgeschnitten (ohne Rundung).

Maximal zulässiger Fehler (EM): MR unter 0,40 mg/L = 0,032 mg/L; MR von 0,40 bis 2,00 mg/L = 8% von MR; MR über 2,00 mg/L = 30% von MR.

Verstoß (Art. 165): MR ≥ 0,05 mg/L (VC ≥ 0,01). Straftat (Art. 306): MR ≥ 0,34 mg/L (VC ≥ 0,30 mg/L, entspricht 6 dg/L Blut).

## Grenzen und Population

Resolution 432/2013 unterscheidet gemessenen und nach Abzug des metrologischen Fehlers berücksichtigten Wert und verlangt ein zugelassenes, geprüftes Instrument. Die rechtliche Einstufung erlaubt auch andere Mittel, einschließlich Blut und einer Kombination psychomotorischer Zeichen. Eine isolierte Atemalkoholberechnung ist weder klinische Beurteilung noch Nachweis der Fahrtauglichkeit oder rechtliche Entscheidung; die geltende Fassung des CTB und der metrologischen Vorschriften muss fallbezogen berücksichtigt werden.

## Referenzen

- [Brasil. Conselho Nacional de Trânsito. Resolução Contran nº 432, de 23 de janeiro de 2013 (procedimentos de fiscalização do consumo de álcool, Anexo I).](https://www.gov.br/transportes/pt-br/assuntos/transito/conteudo-contran/resolucao-no-432-de-23-de-janeiro-de-2013)

- [Brasil. Lei nº 9.503, de 23 de setembro de 1997: Código de Trânsito Brasileiro (arts. 165, 276 e 306), texto compilado.](https://www.planalto.gov.br/ccivil_03/leis/l9503compilado.htm)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Dokumentierte Ergebnisse

Die folgenden Angaben bewahren die Ausgaben der Methode für synthetische Beispiele. Sie stellen keine unabhängige klinische Validierung dar.

### 1

Ordnungswidrigkeit nach Artikel 165 des CTB (Messwert ≥ 0,05 mg/L)

| Ergebnisdetails | |
| --- | --- |
| Durchgeführte Messung (MR) | 0,05 mg/L |
| Maximal zulässiger Fehler (EM) | 0,032 mg/L (fest, MR < 0,40) |
| Ungefährer Blutäquivalentwert (VC × 2) | 0,02 g/L |


### 2

Ordnungswidrigkeit nach Artikel 165 des CTB (Messwert ≥ 0,05 mg/L)

| Ergebnisdetails | |
| --- | --- |
| Durchgeführte Messung (MR) | 0,33 mg/L |
| Maximal zulässiger Fehler (EM) | 0,032 mg/L (fest, MR < 0,40) |
| Ungefährer Blutäquivalentwert (VC × 2) | 0,58 g/L |


### 3

Verstoß gegen Artikel 165 des CTB und Straftat nach Artikel 306 (berücksichtigter Wert ≥ 0,30 mg/L)

| Ergebnisdetails | |
| --- | --- |
| Durchgeführte Messung (MR) | 0,34 mg/L |
| Maximal zulässiger Fehler (EM) | 0,032 mg/L (fest, MR < 0,40) |
| Ungefährer Blutäquivalentwert (VC × 2) | 0,60 g/L |


### 4

Verstoß gegen Artikel 165 des CTB und Straftat nach Artikel 306 (berücksichtigter Wert ≥ 0,30 mg/L)

| Ergebnisdetails | |
| --- | --- |
| Durchgeführte Messung (MR) | 0,64 mg/L |
| Maximal zulässiger Fehler (EM) | 0,051 mg/L (8 % des MR) |
| Ungefährer Blutäquivalentwert (VC × 2) | 1,16 g/L |


### 5

Verstoß gegen Artikel 165 des CTB und Straftat nach Artikel 306 (berücksichtigter Wert ≥ 0,30 mg/L)

| Ergebnisdetails | |
| --- | --- |
| Durchgeführte Messung (MR) | 1,00 mg/L |
| Maximal zulässiger Fehler (EM) | 0,080 mg/L (8 % des MR) |
| Ungefährer Blutäquivalentwert (VC × 2) | 1,84 g/L |


### 6

Verstoß gegen Artikel 165 des CTB und Straftat nach Artikel 306 (berücksichtigter Wert ≥ 0,30 mg/L)

| Ergebnisdetails | |
| --- | --- |
| Durchgeführte Messung (MR) | 2,50 mg/L |
| Maximal zulässiger Fehler (EM) | 0,750 mg/L (30% der MR) |
| Ungefährer Blutäquivalentwert (VC × 2) | 3,50 g/L |


### 7

Unterhalb des Werts, der eine Ordnungswidrigkeit durch das Alkoholmessgerät kennzeichnet (Messung < 0,05 mg/L)

| Ergebnisdetails | |
| --- | --- |
| Durchgeführte Messung (MR) | 0,04 mg/L |
| Maximal zulässiger Fehler (EM) | 0,032 mg/L (fest, MR < 0,40) |
| Ungefährer Blutäquivalentwert (VC × 2) | 0,00 g/L |

Anzeichen einer Beeinträchtigung der psychomotorischen Leistungsfähigkeit (Anhang II der Resolution 432) kennzeichnen die Ordnungswidrigkeit ebenfalls, unabhängig vom Alkoholmessgerät.

