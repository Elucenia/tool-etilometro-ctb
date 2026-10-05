<!-- ELUCENIA technical documentation · etilometro-ctb · en · no clinical/professional/rights approval -->

# Breathalyzer: legally considered value (Brazilian Contran Resolution 432)

[conditions, sources and permissions](https://elucenia.org/en/tools/etilometro-ctb)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Breathalyzer measurement (MR)

`mr`

mg/L of air · range: 0–5

## Method edition

CONTRAN 432/2013 Annex I: error 0.032/8%/30%; truncation to 2 decimals; Brazil scope

## Documented formula

VC = MR − EM, retaining two decimal places and discarding the rest (no rounding).

Maximum permissible error (EM): MR below 0.40 mg/L = 0.032 mg/L; MR from 0.40 to 2.00 mg/L = 8% of MR; MR above 2.00 mg/L = 30% of MR.

Offence (art. 165): MR ≥ 0.05 mg/L (VC ≥ 0.01). Crime (art. 306): MR ≥ 0.34 mg/L (VC ≥ 0.30 mg/L, equivalent to 6 dg/L in blood).

## Limits and population

Resolution 432/2013 distinguishes the measured reading from the considered value after deducting the metrological error and requires an approved, verified instrument. Classification also permits other means, including blood and a set of psychomotor signs. A breathalyzer calculation alone is not a clinical assessment, proof of fitness to drive or a legal decision; the validity of the CTB and metrological legislation must be considered for the case.

## References

- [Brasil. Conselho Nacional de Trânsito. Resolução Contran nº 432, de 23 de janeiro de 2013 (procedimentos de fiscalização do consumo de álcool, Anexo I).](https://www.gov.br/transportes/pt-br/assuntos/transito/conteudo-contran/resolucao-no-432-de-23-de-janeiro-de-2013)

- [Brasil. Lei nº 9.503, de 23 de setembro de 1997: Código de Trânsito Brasileiro (arts. 165, 276 e 306), texto compilado.](https://www.planalto.gov.br/ccivil_03/leis/l9503compilado.htm)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
