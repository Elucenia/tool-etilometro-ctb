<!-- ELUCENIA technical documentation · etilometro-ctb · it · no clinical/professional/rights approval -->

# Etilometro: valore considerato (risoluzione brasiliana Contran 432)

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/etilometro-ctb)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Misurazione con etilometro (MR)

`mr`

mg/L d’aria · intervallo: 0–5

## Edizione del metodo

CONTRAN 432/2013 allegato I: errore 0,032/8%/30%; troncamento a 2 decimali; Brasile

## Formula documentata

VC = MR − EM, a due decimali, eliminando gli altri (senza arrotondare).

Errore massimo ammesso (EM): MR inferiore a 0,40 mg/L = 0,032 mg/L; MR da 0,40 a 2,00 mg/L = 8% di MR; MR superiore a 2,00 mg/L = 30% di MR.

Infrazione (art. 165): MR ≥ 0,05 mg/L (VC ≥ 0,01). Reato (art. 306): MR ≥ 0,34 mg/L (VC ≥ 0,30 mg/L, equivalente a 6 dg/L nel sangue).

## Limiti e popolazione

La Risoluzione 432/2013 distingue la misurazione effettuata dal valore considerato, dopo la detrazione dell’errore metrologico, e richiede uno strumento approvato e verificato. La classificazione ammette anche altri mezzi, tra cui il sangue e un insieme di segni psicomotori. Un calcolo dell’etilometro da solo non costituisce una valutazione clinica, una prova di idoneità alla guida o una decisione giuridica; la validità del CTB e della legislazione metrologica deve essere considerata nel caso.

## Riferimenti

- [Brasil. Conselho Nacional de Trânsito. Resolução Contran nº 432, de 23 de janeiro de 2013 (procedimentos de fiscalização do consumo de álcool, Anexo I).](https://www.gov.br/transportes/pt-br/assuntos/transito/conteudo-contran/resolucao-no-432-de-23-de-janeiro-de-2013)

- [Brasil. Lei nº 9.503, de 23 de setembro de 1997: Código de Trânsito Brasileiro (arts. 165, 276 e 306), texto compilado.](https://www.planalto.gov.br/ccivil_03/leis/l9503compilado.htm)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Risultati documentati

Le informazioni seguenti conservano gli output del metodo per esempi sintetici. Non costituiscono una validazione clinica indipendente.

### 1

Infrazione amministrativa dell’art. 165 del CTB (misurazione ≥ 0,05 mg/L)

| Dettagli del risultato | |
| --- | --- |
| Misurazione effettuata (MR) | 0,05 mg/L |
| Errore massimo ammissibile (EM) | 0,032 mg/L (fisso, MR < 0,40) |
| Equivalente approssimativo nel sangue (VC × 2) | 0,02 g/L |


### 2

Infrazione amministrativa dell’art. 165 del CTB (misurazione ≥ 0,05 mg/L)

| Dettagli del risultato | |
| --- | --- |
| Misurazione effettuata (MR) | 0,33 mg/L |
| Errore massimo ammissibile (EM) | 0,032 mg/L (fisso, MR < 0,40) |
| Equivalente approssimativo nel sangue (VC × 2) | 0,58 g/L |


### 3

Infrazione dell’art. 165 del CTB e reato dell’art. 306 (valore considerato ≥ 0,30 mg/L)

| Dettagli del risultato | |
| --- | --- |
| Misurazione effettuata (MR) | 0,34 mg/L |
| Errore massimo ammissibile (EM) | 0,032 mg/L (fisso, MR < 0,40) |
| Equivalente approssimativo nel sangue (VC × 2) | 0,60 g/L |


### 4

Infrazione dell’art. 165 del CTB e reato dell’art. 306 (valore considerato ≥ 0,30 mg/L)

| Dettagli del risultato | |
| --- | --- |
| Misurazione effettuata (MR) | 0,64 mg/L |
| Errore massimo ammissibile (EM) | 0,051 mg/L (8% della MR) |
| Equivalente approssimativo nel sangue (VC × 2) | 1,16 g/L |


### 5

Infrazione dell’art. 165 del CTB e reato dell’art. 306 (valore considerato ≥ 0,30 mg/L)

| Dettagli del risultato | |
| --- | --- |
| Misurazione effettuata (MR) | 1,00 mg/L |
| Errore massimo ammissibile (EM) | 0,080 mg/L (8% della MR) |
| Equivalente approssimativo nel sangue (VC × 2) | 1,84 g/L |


### 6

Infrazione dell’art. 165 del CTB e reato dell’art. 306 (valore considerato ≥ 0,30 mg/L)

| Dettagli del risultato | |
| --- | --- |
| Misurazione effettuata (MR) | 2,50 mg/L |
| Errore massimo ammissibile (EM) | 0,750 mg/L (30% della MR) |
| Equivalente approssimativo nel sangue (VC × 2) | 3,50 g/L |


### 7

Al di sotto del valore che caratterizza un’infrazione con l’etilometro (misurazione < 0,05 mg/L)

| Dettagli del risultato | |
| --- | --- |
| Misurazione effettuata (MR) | 0,04 mg/L |
| Errore massimo ammissibile (EM) | 0,032 mg/L (fisso, MR < 0,40) |
| Equivalente approssimativo nel sangue (VC × 2) | 0,00 g/L |

I segni di alterazione della capacità psicomotoria (Allegato II della Risoluzione 432) caratterizzano anche l’infrazione, indipendentemente dall’etilometro.

