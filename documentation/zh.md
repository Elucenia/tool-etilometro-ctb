<!-- ELUCENIA technical documentation · etilometro-ctb · zh · no clinical/professional/rights approval -->

# 呼气酒精检测：认定值（巴西 Contran 第 432 号决议）

[条件、来源与许可](https://elucenia.org/zh/tools/etilometro-ctb)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 呼气酒精检测仪实测值（MR）

`mr`

mg/L 空气 · 范围: 0–5

## 方法版本

CONTRAN 432/2013附件I：误差0.032/8%/30%；截取2位小数；适用于巴西

## 已记录的公式

VC = MR − EM，保留两位小数，其余截去（不四舍五入）。

最大允许误差（EM）：MR低于0.40 mg/L = 0.032 mg/L；MR为0.40至2.00 mg/L = MR的8%；MR高于2.00 mg/L = MR的30%。

违法（第165条）：MR ≥ 0.05 mg/L（VC ≥ 0.01）。犯罪（第306条）：MR ≥ 0.34 mg/L（VC ≥ 0.30 mg/L，相当于血液6 dg/L）。

## 限制与适用人群

432/2013号决议区分实际测量值与扣除计量误差后的认定值，并要求仪器获批准且通过检定。法律认定还可采用其他证据，包括血液及一组精神运动体征。单独的呼气酒精检测计算不能构成临床评估、驾驶能力证明或法律决定；应结合个案核对《巴西交通法典》（CTB）及计量法规的效力。

## 参考文献

- [Brasil. Conselho Nacional de Trânsito. Resolução Contran nº 432, de 23 de janeiro de 2013 (procedimentos de fiscalização do consumo de álcool, Anexo I).](https://www.gov.br/transportes/pt-br/assuntos/transito/conteudo-contran/resolucao-no-432-de-23-de-janeiro-de-2013)

- [Brasil. Lei nº 9.503, de 23 de setembro de 1997: Código de Trânsito Brasileiro (arts. 165, 276 e 306), texto compilado.](https://www.planalto.gov.br/ccivil_03/leis/l9503compilado.htm)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 已记录的结果

以下信息保留该方法对合成示例的输出，不构成独立的临床验证。

### 1

CTB 第165条行政违法（测量值 ≥ 0,05 mg/L）

| 结果详情 | |
| --- | --- |
| 所进行的测量（MR） | 0.05 mg/L |
| 允许最大误差（EM） | 0.032 mg/L（固定，MR < 0,40） |
| 血液近似当量（VC × 2） | 0.02 g/L |


### 2

CTB 第165条行政违法（测量值 ≥ 0,05 mg/L）

| 结果详情 | |
| --- | --- |
| 所进行的测量（MR） | 0.33 mg/L |
| 允许最大误差（EM） | 0.032 mg/L（固定，MR < 0,40） |
| 血液近似当量（VC × 2） | 0.58 g/L |


### 3

CTB 第165条违法和第306条犯罪（采用值 ≥ 0,30 mg/L）

| 结果详情 | |
| --- | --- |
| 所进行的测量（MR） | 0.34 mg/L |
| 允许最大误差（EM） | 0.032 mg/L（固定，MR < 0,40） |
| 血液近似当量（VC × 2） | 0.60 g/L |


### 4

CTB 第165条违法和第306条犯罪（采用值 ≥ 0,30 mg/L）

| 结果详情 | |
| --- | --- |
| 所进行的测量（MR） | 0.64 mg/L |
| 允许最大误差（EM） | 0.051 mg/L（MR 的 8%） |
| 血液近似当量（VC × 2） | 1.16 g/L |


### 5

CTB 第165条违法和第306条犯罪（采用值 ≥ 0,30 mg/L）

| 结果详情 | |
| --- | --- |
| 所进行的测量（MR） | 1.00 mg/L |
| 允许最大误差（EM） | 0.080 mg/L（MR 的 8%） |
| 血液近似当量（VC × 2） | 1.84 g/L |


### 6

CTB 第165条违法和第306条犯罪（采用值 ≥ 0,30 mg/L）

| 结果详情 | |
| --- | --- |
| 所进行的测量（MR） | 2.50 mg/L |
| 允许最大误差（EM） | 0.750 mg/L（MR 的 30%） |
| 血液近似当量（VC × 2） | 3.50 g/L |


### 7

低于呼气酒精测试仪构成违法的数值（测量值 < 0,05 mg/L）

| 结果详情 | |
| --- | --- |
| 所进行的测量（MR） | 0.04 mg/L |
| 允许最大误差（EM） | 0.032 mg/L（固定，MR < 0,40） |
| 血液近似当量（VC × 2） | 0.00 g/L |

精神运动能力受损的迹象（第 432 号决议附件 II）也构成该违法行为，与呼气酒精测试仪无关。

