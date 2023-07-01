# Japanese Argument Omission  Judgment

## Source Corpus
[The Balanced Corpus of Contemporary Written Japanese (BCCWJ)](https://clrd.ninjal.ac.jp/bccwj/en/index.html) 
- We used documents from the book Domain.
- `00002_A_PB43_00001` ~ `00036_B_PB42_00014`
（excluding `00003_A_PB59_00001`, `00004_A_PB22_00002`, `00010_A_PB50_00003`）


## BCCWJ-DepParaPAS
In this study, we created a corpus by overlaying information on ellipsis judgments on BCCWJ-DepParaPAS, a widely-used Japanese corpus with predicate-argument structure annotation. The version of BCCWJ-DepParaPAS we used is  3.3.0_1.2.0_20160301. The annotation procedure is explained in detail in the paper.


## Attributes of annotated information
| | Attribute | Details |
|:---|:---|:---|
|1 |`type` |Whether the argument is  or omitted (present: "dep", omitted: "zero") | 
|2 |`dep_arg_span` |Word span when the annotated argument is expressed |
|3 |`filler` |Expression of the embedded filler when the annotated argument is omitted |
|4 |`insert_position` |Insertion position of the embedded filler ([the number of the sentence from the beginning, the number of the syntactic chunk that should follow the insertion point]) | 
|5 |`pred_span` |Span of a target predicate|
|6 |`casemk`|Case marker (NOM: "ga", ACC: "o", DAT: "ni") |
|7 |`answers` |Annotators' answers (Displaying the answers of each annotator in the order of their IDs, and the alphabets represent the terminals in the decision tree. The details are explained in the paper. ) |

Note that the word spans for attributes 2 and 5 represent [the number of the sentence from the beginning of the text, the position of the start of the argument or predicate in words from the beginning of the sentence, the position of the end of the argument or predicate in words from the beginning of the sentence].

## License
</a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.

## Related work
Use the following citation if you use the data set:
BibTeX
```
% Syntactic Dependency and Coordination Structure
@Article{浅原正幸2018,
 title={『現代日本語書き言葉均衡コーパス』に対する係り受け・並列構造アノテーション},
 author={浅原 正幸 and 松本 裕治},
 journal = {自然言語処理},
 volume = {25},
 number = {4},
 pages = 	 {331--356},
 year = 	 {2018}
}

% Sentence Segmentation
@inProceedings{小西光2013bccwj,
  title={BCCWJ 係り受け関係アノテーション付与のための文境界再認定},
  author={小西光 and 小山田由紀 and 浅原正幸 and 柏野 和佳子 and 前川喜久雄},
  booktitle = {第3回コーパス日本語学ワークショップ予稿集},
  pages = 	 {135--142},
  year = 	 {2013},
  organization = {国立国語研究所}
}

% BCCWJ Original Data
@article{maekawa2014balanced,
  title={Balanced corpus of contemporary written Japanese},
  author={MAEKAWA, Kikuo and YAMAZAKI, Makoto and OGISO, Toshinobu and MARUYAMA, Takehiko and OGURA, Hideki and KASHINO, Wakako and KOISO, Hanae and YAMAGUCHI, Masaya and TANAKA, Makiro and DEN, Yasuharu},
  journal={Language resources and evaluation},
  volume={48},
  number={2},
  pages={345--371},
  year={2014},
  publisher={Springer}
}

% Semantic Dependency and Coreference Information
@inProceedings{植田禎子2015bccwj,
  title={『現代日本語書き言葉均衡コーパス』に対する述語項構造・共参照情報アノテーション},
  author={植田禎子 and 飯田龍 and 浅原正幸 and 松本裕治 and 徳永健伸},
  booktitle = {第8回コーパス日本語学ワークショップ予稿集},
  pages = 	 {205--214},
  year = 	 {2015},
  organization = {国立国語研究所}
}

% the Resource
@inProceedings{浅原正幸2016bccwj,
  title={BCCWJ-DepParaPAS:『現代日本語書き言葉均衡コーパス』係り受け・並列構造と述語項構造・共参照アノテーションの重ね合わせと可視化},
  author={浅原 正幸 and 大村 舞},
  booktitle = {言語処理学会第22回年次大会発表論文集},
  pages = 	 {489--492},
  year = 	 {2016}
}
```
