# Junior / High School in Japan
日本の中高等学校

## 注意

- このデータはスクレイピングの結果であり、正確さは保証できません。
   - 学術研究のために使用せず、データ分析の練習用としてお使いください。
- 全国の中高が入っているわけではございません。
   - 2025年現在、日本国内の中学校は約10000校、高等学校は約5000校あるとされています。

## ファイル

- `jhs_list.csv`：中学リスト
- `hs_list.csv`：高校リスト
- `did_dataset.csv`：都道府県、市区町村別人口集中地区人口（比）

## 変数

**`jhs_list.csv`および`hs_list.csv`**

|変数名|説明|備考|
|:---|:---|:---|
|`id`|識別番号||
|`rank`|偏差値順位||
|`score`|偏差値||
|`name`|高校名||
|`course`|コース名|コース名がない場合、`NA`|
|`region`|地域8区分|北海道、東北、関東、中部、近畿、中国、四国、九州・沖縄|
|`jis_code`|全国地方公共団体コード||
|`pref`|都道府県||
|`city`|市区町村名||
|`ward`|行政区名|政令指定都市のみ|
|`station`|最寄りの駅名||
|`distance`|最寄りの駅からの徒歩距離（分）|中学データセットのみ|
|`type`|学校の種類|国立、公立、私立|
|`gender`|性別|共学、男子校、女子校、その他|
|`review`|口コミ評価|5点満点|
|`did_pref`|DID（人口集中地区）人口比|都道府県|
|`did_city`|DID（人口集中地区）人口比|市区町村|


**`did_dataset.csv`**

|変数名|説明|備考|
|:---|:---|:---|
|`code`|全国地方公共団体コード||
|`pref`|都道府県||
|`city`|市区町村||
|`pop`|人口||
|`did`|人口集中地区人口||
|`did_prop`|人口集中地区人口比||

## 出典

- 収集日時：2025年6月23日（高校）、2025年6月24日（中学）
- みんなの中学情報：<https://www.minkou.jp/junior/ranking/deviation/>
- みんなの高校情報：<https://www.minkou.jp/hischool/ranking/deviation/>
- 2020年国勢調査：<https://www.stat.go.jp/data/kokusei/2020/kekka.html>
