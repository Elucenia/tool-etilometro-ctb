<!-- ELUCENIA technical documentation · etilometro-ctb · ja · no clinical/professional/rights approval -->

# 呼気アルコール検査：採用値（ブラジルContran決議432）

[条件・出典・許諾](https://elucenia.org/ja/tools/etilometro-ctb)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 呼気アルコール測定器による測定値（MR）

`mr`

mg/L 空気 · 範囲: 0–5

## 方法の版

CONTRAN 432/2013付属書I：誤差0.032/8%/30%；2桁で切捨て；ブラジル適用

## 記載された計算式

VC = MR − EM。小数点以下2桁を残し，それ以降を切り捨てる（四捨五入なし）。

最大許容誤差（EM）：MRが0.40 mg/L未満 = 0.032 mg/L；MRが0.40〜2.00 mg/L = MRの8%；MRが2.00 mg/L超 = MRの30%。

違反（第165条）：MR ≥ 0.05 mg/L（VC ≥ 0.01）。犯罪（第306条）：MR ≥ 0.34 mg/L（VC ≥ 0.30 mg/L，血液6 dg/L相当）。

## 限界・対象集団

決議432/2013は、測定値と計量誤差を差し引いた後の認定値を区別し、承認・検定済みの機器を要求します。法的な該当判断には、血液や精神運動徴候の組合せなど、他の手段も認められています。呼気アルコール計算だけでは、臨床評価、運転適性の証明、法的判断にはなりません。個別の事例において、ブラジル道路交通法（CTB）と計量法令の効力を確認する必要があります。

## 参考文献

- [Brasil. Conselho Nacional de Trânsito. Resolução Contran nº 432, de 23 de janeiro de 2013 (procedimentos de fiscalização do consumo de álcool, Anexo I).](https://www.gov.br/transportes/pt-br/assuntos/transito/conteudo-contran/resolucao-no-432-de-23-de-janeiro-de-2013)

- [Brasil. Lei nº 9.503, de 23 de setembro de 1997: Código de Trânsito Brasileiro (arts. 165, 276 e 306), texto compilado.](https://www.planalto.gov.br/ccivil_03/leis/l9503compilado.htm)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026
