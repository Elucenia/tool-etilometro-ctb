<!-- ELUCENIA technical documentation · etilometro-ctb · pt-BR · no clinical/professional/rights approval -->

# Etilômetro: valor considerado (Resolução Contran 432)

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/etilometro-ctb)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Medição realizada pelo etilômetro (MR)

`mr`

mg/L de ar · intervalo: 0–5

## Edição do método

CONTRAN 432/2013 Anexo I:erro 0,032/8%/30%; truncamento 2 decimais; aplicação Brasil

## Fórmula documentada

VC = MR − EM, com duas casas decimais, desprezando as demais (sem arredondamento).

Erro máximo admissível (EM): MR inferior a 0,40 mg/L = 0,032 mg/L; MR de 0,40 até 2,00 mg/L = 8% da MR; MR acima de 2,00 mg/L = 30% da MR.

Infração (art. 165): MR ≥ 0,05 mg/L (VC ≥ 0,01). Crime (art. 306): MR ≥ 0,34 mg/L (VC ≥ 0,30 mg/L, equivalente a 6 dg/L de sangue).

## Limites e população

A Resolução 432/2013 distingue medição realizada e valor considerado, após desconto do erro metrológico, e exige instrumento aprovado e verificado. O enquadramento também admite outros meios, inclusive sangue e conjunto de sinais psicomotores. Um cálculo de etilômetro isolado não constitui avaliação clínica, prova de aptidão para dirigir ou decisão jurídica; a vigência do CTB e da legislação metrológica deve acompanhar o caso.

## Referências

- [Brasil. Conselho Nacional de Trânsito. Resolução Contran nº 432, de 23 de janeiro de 2013 (procedimentos de fiscalização do consumo de álcool, Anexo I).](https://www.gov.br/transportes/pt-br/assuntos/transito/conteudo-contran/resolucao-no-432-de-23-de-janeiro-de-2013)

- [Brasil. Lei nº 9.503, de 23 de setembro de 1997: Código de Trânsito Brasileiro (arts. 165, 276 e 306), texto compilado.](https://www.planalto.gov.br/ccivil_03/leis/l9503compilado.htm)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

As informações abaixo preservam as saídas do método para exemplos sintéticos. Não constituem validação clínica independente.

### 1

Infração administrativa do art. 165 do CTB (medição ≥ 0,05 mg/L)

| Detalhes do resultado | |
| --- | --- |
| Medição realizada (MR) | 0,05 mg/L |
| Erro máximo admissível (EM) | 0,032 mg/L (fixo, MR < 0,40) |
| Equivalente aproximado no sangue (VC × 2) | 0,02 g/L |


### 2

Infração administrativa do art. 165 do CTB (medição ≥ 0,05 mg/L)

| Detalhes do resultado | |
| --- | --- |
| Medição realizada (MR) | 0,33 mg/L |
| Erro máximo admissível (EM) | 0,032 mg/L (fixo, MR < 0,40) |
| Equivalente aproximado no sangue (VC × 2) | 0,58 g/L |


### 3

Infração do art. 165 do CTB e crime do art. 306 (valor considerado ≥ 0,30 mg/L)

| Detalhes do resultado | |
| --- | --- |
| Medição realizada (MR) | 0,34 mg/L |
| Erro máximo admissível (EM) | 0,032 mg/L (fixo, MR < 0,40) |
| Equivalente aproximado no sangue (VC × 2) | 0,60 g/L |


### 4

Infração do art. 165 do CTB e crime do art. 306 (valor considerado ≥ 0,30 mg/L)

| Detalhes do resultado | |
| --- | --- |
| Medição realizada (MR) | 0,64 mg/L |
| Erro máximo admissível (EM) | 0,051 mg/L (8% da MR) |
| Equivalente aproximado no sangue (VC × 2) | 1,16 g/L |


### 5

Infração do art. 165 do CTB e crime do art. 306 (valor considerado ≥ 0,30 mg/L)

| Detalhes do resultado | |
| --- | --- |
| Medição realizada (MR) | 1,00 mg/L |
| Erro máximo admissível (EM) | 0,080 mg/L (8% da MR) |
| Equivalente aproximado no sangue (VC × 2) | 1,84 g/L |


### 6

Infração do art. 165 do CTB e crime do art. 306 (valor considerado ≥ 0,30 mg/L)

| Detalhes do resultado | |
| --- | --- |
| Medição realizada (MR) | 2,50 mg/L |
| Erro máximo admissível (EM) | 0,750 mg/L (30% da MR) |
| Equivalente aproximado no sangue (VC × 2) | 3,50 g/L |


### 7

Abaixo do valor que caracteriza infração pelo etilômetro (medição < 0,05 mg/L)

| Detalhes do resultado | |
| --- | --- |
| Medição realizada (MR) | 0,04 mg/L |
| Erro máximo admissível (EM) | 0,032 mg/L (fixo, MR < 0,40) |
| Equivalente aproximado no sangue (VC × 2) | 0,00 g/L |

Sinais de alteração da capacidade psicomotora (Anexo II da Resolução 432) também caracterizam a infração, independentemente do etilômetro.

