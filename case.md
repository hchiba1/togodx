## Case 3: 特定の疾患に関連する遺伝子を絞り込んだうえで、それらのタンパク質と相互作用する可能性のある化合物を取得する

### 目的
網膜色素変症に関わるヒト遺伝子について、ゼブラフィッシュでも保存されているものに絞ったうえで、それらのタンパク質と相互作用する可能性のある化合物を取得する。

### 背景
網膜色素変症は指定難病の一つで治療方法も確立していないが、研究アプローチとしてモデル生物を用いた薬剤候補スクリーニング実験が考えられる([参考文献](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8425951/))。ここでは、網膜色素変性症およびそれに関連する表現型に着目して、TogoDXを用いた検索を行ってみる。

### 検索方法の組み合わせ

#### Add filters
* `Protein` / `Disease-related proteins`
  * Retinitis pigmentosa（網膜色素変性症）
  * Congenital stationary night blindness（先天停止性夜盲）
  * Cone-rod dystrophy（錐体桿体ジストロフィー）
  * Leber congenital amaurosis（レーバー先天黒内障）
* `Gene` / `Tissue-specific high expression (HPA)`
  * Retina（網膜）
* `Gene` / `Ortholog existence`
  * Zebrafish (Danio rerio)

#### Map attributes
* `Compound` / `Max drug development phase`

[検索の再現](https://togodx.dbcls.jp/human/?dataset=ensembl_gene&annotations=%5B%7B%22attributeId%22%3A%22compound_drug_development_phase_chembl%22%7D%5D&filters=%5B%7B%22attributeId%22%3A%22protein_disease_related_proteins_uniprot%22%2C%22nodes%22%3A%5B%7B%22node%22%3A%22682%22%7D%2C%7B%22node%22%3A%221014%22%7D%2C%7B%22node%22%3A%22510%22%7D%2C%7B%22node%22%3A%22901%22%7D%2C%7B%22node%22%3A%22182%22%7D%5D%7D%2C%7B%22attributeId%22%3A%22gene_specific_expression_in_tissues_hpa%22%2C%22nodes%22%3A%5B%7B%22node%22%3A%22Retina%22%7D%5D%7D%2C%7B%22attributeId%22%3A%22gene_ortholog_existence_homologene%22%2C%22nodes%22%3A%5B%7B%22node%22%3A%22organism_10%22%7D%5D%7D%5D)

### 結果
* 指定した疾患に関連するヒト遺伝子で、ゼブラフィッシュにもオーソログが存在する42の遺伝子が得られる。
* さらに、それらのタンパク質と相互作用する可能性のある化合物が得られる。このうち、第IV相試験(製造販売後臨床試験)に達している化合物は46件である。
* 関連する遺伝子が多くまた表現型も多様なため、得られた化合物が疾患に対して有効かはどうかを判定することは難しいが、少なくともCHEMBL91 (Miconazole) については、上記参考文献の実験でも網膜色素変性症に対し神経保護剤として有効であるという結果が出ている。
![](https://i.imgur.com/QjvBiZG.png)


## Case 3: 特定の疾患に関連する遺伝子を絞り込んだうえで、それらのタンパク質と相互作用する可能性のある化合物を取得する

### 目的
網膜色素変症に関わるヒト遺伝子について、ゼブラフィッシュでも保存されているものに絞ったうえで、それらのタンパク質と相互作用する可能性のある化合物を取得する。

### 背景
網膜色素変症は指定難病の一つで治療方法も確立していないが、研究アプローチとしてモデル生物を用いた薬剤候補スクリーニング実験が考えられる([参考文献](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8425951/))。ここでは、網膜色素変性症およびそれに関連する表現型に着目して、TogoDXを用いた検索を行ってみる。

### 検索方法の組み合わせ

#### Add filters
* `Protein` / `Disease-related proteins`
  * Retinitis pigmentosa（網膜色素変性症）
  * Congenital stationary night blindness（先天停止性夜盲）
  * Cone-rod dystrophy（錐体桿体ジストロフィー）
  * Leber congenital amaurosis（レーバー先天黒内障）
* `Gene` / `Ortholog existence`
  * Zebrafish (Danio rerio)

#### Map attributes
* `Compound` / `Max drug development phase`

[検索の再現](https://togodx.dbcls.jp/human/?dataset=ncbigene&annotations=%5B%7B%22attributeId%22%3A%22compound_drug_development_phase_chembl%22%7D%5D&filters=%5B%7B%22attributeId%22%3A%22gene_ortholog_existence_homologene%22%2C%22nodes%22%3A%5B%7B%22node%22%3A%22organism_10%22%7D%5D%7D%2C%7B%22attributeId%22%3A%22protein_disease_related_proteins_uniprot%22%2C%22nodes%22%3A%5B%7B%22node%22%3A%22682%22%7D%2C%7B%22node%22%3A%221014%22%7D%2C%7B%22node%22%3A%22901%22%7D%2C%7B%22node%22%3A%22182%22%7D%5D%7D%5D)

### 結果
* 指定した疾患に関連するヒト遺伝子で、ゼブラフィッシュにもオーソログが存在する132の遺伝子が得られる。
* さらに、それらのタンパク質と相互作用する可能性のある化合物が得られる。このうち、第IV相試験(製造販売後臨床試験)に達している化合物は193件である。
* 関連する遺伝子が多くまた表現型も多様なため、得られた化合物が疾患に対して有効かはどうかを判定することは難しいが、少なくともCHEMBL91 (Miconazole) については、上記参考文献の実験でも網膜色素変性症に対し神経保護剤として有効であるという結果が出ている。
![](https://i.imgur.com/HWpMYRG.png)


## Case 3: 特定の疾患に関連する遺伝子を絞り込んだうえで、それらのタンパク質と相互作用する可能性のある化合物を取得する

### 目的
網膜色素変症に関わる遺伝子について、ゼブラフィッシュにおいてオーソログがあるものに絞ったうえで、それらのタンパク質と相互作用する可能性のある化合物を取得する。

### 背景
網膜色素変症は指定難病の一つで治療方法も確立していないが、研究アプローチとしてはモデル生物を用いた薬剤候補のスクリーニング実験が考えられる([参考文献](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8425951/))。ここでは、網膜色素変性症およびそれに関連する表現型に着目して、TogoDXを用いた検索を行ってみる。

### 検索方法の組み合わせ
#### Add filters
* `Protein` / `Disease-related proteins`
  * Retinitis pigmentosa（網膜色素変性症）
  * Congenital stationary night blindness（先天停止性夜盲）
  * Cone-rod dystrophy（錐体桿体ジストロフィー）
  * Leber congenital amaurosis（レーバー先天黒内障）
* `Gene` / `Ortholog existence`
  * Zebrafish (Danio rerio)

#### Map attributes
* `Compound` / `Max drug development phase`

[この検索条件の再現](https://togodx.dbcls.jp/human/?dataset=ncbigene&annotations=%5B%7B%22attributeId%22%3A%22compound_drug_development_phase_chembl%22%7D%5D&filters=%5B%7B%22attributeId%22%3A%22gene_ortholog_existence_homologene%22%2C%22nodes%22%3A%5B%7B%22node%22%3A%22organism_10%22%7D%5D%7D%2C%7B%22attributeId%22%3A%22protein_disease_related_proteins_uniprot%22%2C%22nodes%22%3A%5B%7B%22node%22%3A%22682%22%7D%2C%7B%22node%22%3A%221014%22%7D%2C%7B%22node%22%3A%22901%22%7D%2C%7B%22node%22%3A%22182%22%7D%5D%7D%5D)

### 結果
* 指定した疾患に関連するヒト遺伝子のうち、ゼブラフィッシュでも保存されている132遺伝子が得られる。
* さらに、それらのタンパク質と相互作用する可能性のある化合物が得られる。このうち、第IV相試験(製造販売後臨床試験)に達している化合物は193件である。
* これらは単一遺伝子疾患ではなくまた表現型も多様で複雑なため、得られた化合物が疾患に対して有効かはどうかを判定することは難しいが、少なくともCHEMBL91 (Miconazole) については、上記参考文献の実験でも網膜色素変性症に対し神経保護剤として有効であるという結果が示されている。
![](https://i.imgur.com/HWpMYRG.png)

## Case 3
難病の原因遺伝子について、疾患のバーと遺伝子のバーを組み合わせた検索を行い、モデル生物へとつなげてみる。
* Add filtersでDiseases in NANDOバーのトップのカテゴリ2つと、ChromosomeバーのXと、Ortholog existenceのBudding yeastおよびFission yeastにチェックを入れる。
![](https://i.imgur.com/jnIeAVs.png)
* View resultsで結果を見ると、遺伝子7つが出る。たとえばGLA (galactosidase alpha, α‐ガラクトシダーゼ) という遺伝子が出ている。
![](https://i.imgur.com/zza2QBf.png)
* これに対応する難病オントロジーNANDOのID`1200158`をクリックすると、ファブリー病に関連していることが確認できる。
![](https://i.imgur.com/IgAscPa.png)
* α‐ガラクトシダーゼはファブリー病の治療に重要であり、かつ酵母のような微生物を用いた研究アプローチも有効であると期待される。([Ref.](https://www.tandfonline.com/doi/abs/10.3109/07388551.2013.794124?cookieSet=1))

## Case 4
疾患 - 遺伝子 - タンパク質 - 化合物 という関係と、遺伝子 - モデル生物 という関係、遺伝子発現データを利用してみる。
* 目の異常に関連し、網膜特異的グリア細胞（Muller glial cell）で発現が認められるタンパク質に対して、相互作用する可能性のある化合物とそのDrug developmen phaseを挙げるとともに、それらの遺伝子がどのようなモデル生物に存在するかを見る。
* Add filtersでCell Geneのtype-specific high expression (HPA)というバーのMuller glial cell、DiseaseのPhenotypic abnormalityというバーのAbnormality of the eyeを選択し、さらにMap attributesでCompoundのDrug development phaseというバーと、GeneのOrtholog existenceというバーを選択する。
![](https://i.imgur.com/29kiZ8H.png)
* 結果を見ると、3つの遺伝子が出ている。テーブルの4カラム目を見ると、各遺伝子がコードするタンパク質に対して、相互作用する可能性のある化合物が出ている。よく調べられている遺伝子や化合物もあるが、そうでないものもある。PAX6は眼の発生におけるマスター制御因子である。KCNJ13や対応する化合物についてはまだ分かっていないこともあるが、ゼブラフィッシュをモデル生物とした研究アプローチも有効であると期待される。

## Case 4-2
疾患 - 遺伝子 - タンパク質 - 化合物 という関係と、オーソログ遺伝子 - 生物の関係を利用する。特定の目の病気(夜盲症)に関係する遺伝子と、その遺伝子がコードするタンパク質に対し相互作用する可能性のある化合物を上げるとともに、それらの遺伝子のオーソログが存在する生物を表示する。
![](https://i.imgur.com/UxyvS8a.png)
Add filtersで以下の条件を選択する
* ProteinのDisease-related proteinsのバーでCongenital stationary night blindnessを選択
* GeneのOrtholog existenceのバーでZebrafish (Danio rerio)を選択

Map attributesで以下の条件を選択する
* Drug development phaseのバーを選択

結果
* 13の遺伝子が出てくる。これらの遺伝子がコードするタンパク質に対して、相互作用する可能性のある化合物が出ている。
* GRM6に対疾患応する化合物の、一番下にCHMBL91 (Miconazole) が出ている。

考察
* 網膜色素変性症に対して有効な化合物をスクリーニングした実験の[論文](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8425951/)において、Miconazoleは有効なリード化合物の一つに挙げられている。

### 2022-03-03 修正版
網膜色素変症に関わるタンパク質について、ゼブラフィッシュにおいて相同遺伝子があるものに絞ったうえで、それらのタンパク質と相互作用する可能性のある化合物を列挙する。

Add filtersで以下の条件を選択する
* `Protein` / `Disease-related proteins`
  * Retinitis pigmentosa
  * Congenital stationary night blindness
* `Gene` / `Ortholog existence`
  * Zebrafish (Danio rerio)

Map attributesで以下の条件を選択する
* `Compound` / `Drug development phase`

結果
* 101の疾患関連遺伝子がリストアップされて出てくる。
* GRM6に対応する化合物として、CHMBL91 (Miconazole) が出ている。これは実験によって得られた網膜色素変性症に対するリード化合物の一つである。
![](https://i.imgur.com/HWpMYRG.png)
