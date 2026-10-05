<!-- ELUCENIA technical documentation · etilometro-ctb · es · no clinical/professional/rights approval -->

# Alcoholímetro: valor considerado (Resolución brasileña Contran 432)

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/etilometro-ctb)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Medición del alcoholímetro (MR)

`mr`

mg/L de aire · intervalo: 0–5

## Edición del método

CONTRAN 432/2013 Anexo I: error 0,032/8%/30%; truncamiento a 2 decimales; aplicación Brasil

## Fórmula documentada

VC = MR − EM, con dos decimales y descartando los demás (sin redondeo).

Error máximo admisible (EM): MR inferior a 0,40 mg/L = 0,032 mg/L; MR de 0,40 a 2,00 mg/L = 8% de MR; MR superior a 2,00 mg/L = 30% de MR.

Infracción (art. 165): MR ≥ 0,05 mg/L (VC ≥ 0,01). Delito (art. 306): MR ≥ 0,34 mg/L (VC ≥ 0,30 mg/L, equivalente a 6 dg/L en sangre).

## Límites y población

La Resolución 432/2013 distingue la medición realizada del valor considerado, tras descontar el error metrológico, y exige un instrumento aprobado y verificado. La clasificación también admite otros medios, incluidos sangre y un conjunto de signos psicomotores. Un cálculo de alcoholímetro aislado no constituye evaluación clínica, prueba de aptitud para conducir ni decisión jurídica; debe considerarse la vigencia del CTB y de la legislación metrológica en el caso.

## Referencias

- [Brasil. Conselho Nacional de Trânsito. Resolução Contran nº 432, de 23 de janeiro de 2013 (procedimentos de fiscalização do consumo de álcool, Anexo I).](https://www.gov.br/transportes/pt-br/assuntos/transito/conteudo-contran/resolucao-no-432-de-23-de-janeiro-de-2013)

- [Brasil. Lei nº 9.503, de 23 de setembro de 1997: Código de Trânsito Brasileiro (arts. 165, 276 e 306), texto compilado.](https://www.planalto.gov.br/ccivil_03/leis/l9503compilado.htm)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
