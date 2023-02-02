# JAOJ
Japanese argument omission  judgment

## 1.対象ドキュメント
[「現代日本語書き言葉均衡コーパス」(BCCWJ)](https://clrd.ninjal.ac.jp/bccwj/) の書籍ドメインのドキュメント`00002_A_PB43_00001` ~ `00036_B_PB42_00014`
（`00003_A_PB59_00001`, `00004_A_PB22_00002`, `00010_A_PB50_00003`を除く）


## 2.BCCWJ-DepParaPasとの差分データ
Example [annotated_data/00002_A_PB43_00001-jaoj.tsv](https://github.com/tohoku-edunlp/JAOJ/blob/main/annotated_data/00002_A_PB43_00001-jaoj.tsv)

## 3.付与されている情報の属性
| |属性名 |内容 |
|:---|:---|:---|
|1 |`type` |アノテーション対象項が元コーパスで表出か省略か（表出:"dep", 省略:"zero") | 
|2 |`dep_arg_span` |アノテーション対象項が表出している場合の単語スパン |
|3 |`filler` |アノテーション対象項が省略されている場合に埋め込まれた項の表出系 |
|4 |`insert_position` |埋め込まれた項の挿入位置（[挿入箇所が先頭から何文目か, 挿入箇所の次にくるべきの文節の番号]） | 
|5 |`pred_span` |アノテーション対象述語の単語スパン|
|6 |`casemk`|格属性（"ga", "ni", "o"） |
|7 |`answers` |作業者の回答（作業者に紐付いたid順に各作業者の回答を表示しており、アルファベットは[フローチャート](https://github.com/tohoku-edunlp/JAOJ/blob/main/decision_tree.pdf) の終端を示す。） |

なお、2および5の単語スパンは`[先頭から何文目の単語か, 項または述語の開始位置が文の先頭から短単位で何単語目か, 項または述語の終了位置が文の先頭から短単位で何単語目か]`を表している。

## 4.License
</a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.

## 　5.関連研究
- 浅原正幸, 松本裕治. 『現代日本語書き言葉均衡コーパス』に対する係り受け・並列構造アノテーション. 自然言語処理, Vol. 25, No. 4, pp. 331–356, 2018.
- 小西光, 小山田由紀, 浅原正幸, 柏野和佳子, 前川喜久雄. Bccwj 係り受け関係アノテーション付与のための文境界再認定. 第 3 回コーパス日本語学ワークショップ予稿集, pp. 135–142.国立国語研究所, 2013.
- Kikuo MAEKAWA, Makoto YAMAZAKI, Toshinobu OGISO, Takehiko MARUYAMA,Hideki OGURA, Wakako KASHINO, Hanae KOISO, Masaya YAMAGUCHI, Makiro TANAKA, and Yasuharu DEN. Balanced corpus of contemporary written japanese.Language resources and evaluation, Vol. 48, No. 2, pp. 345–371, 2014.
- 植田禎子, 飯田龍, 浅原正幸, 松本裕治, 徳永健伸. 『現代日本語書き言葉均衡コーパス』に対する述語項構造・共参照情報アノテーション. 第 8 回コーパス日本語学ワークショップ予稿集, pp. 205–214. 国立国語研究所, 2015.
- 浅原正幸, 大村舞. Bccwj-DepParaPas:『現代日本語書き言葉均衡コーパス』係り受け・並列構造と述語項構造・共参照アノテーションの重ね合わせと可視化. 言語処理学会第 22 回年次大会発表論文集, pp. 489–492, 2016.10
- 石月由紀子, 栗林 樹生, 松林 優一郎, 笹野 遼平, 乾 健太郎. 日本語話者の項省略判断に関するアノテーションとモデリング. 言語処理学会第 29 回年次大会発表論文集, , 2023.
