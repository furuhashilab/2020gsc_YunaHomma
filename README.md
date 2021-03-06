# 2020gsc_YunaHomma
本間友那 2020年度ゼミ論用レポジトリ

# 概要
世田谷区で地震が起きた時のドローンの撮影ルートをGoogle Earth Studioで想定する.

# 序論
地震大国である日本はいつどこで大きな地震が発生するか分からず、昨今懸念されている大地震の1つに首都直下型地震があり、政府の地震調査委員会によると今後30年以内に70%の確率でマグニチュード約7の地震が関東で予測されている。世界的に見ても過去4番目に大きな地震であった2011年3月の東日本大震災では、首都圏は人的被害、建築物等被害、停電、道路、ライフライン等で被害が生じ、さらに帰宅困難者などの課題も発見されている。また地震が起きてこれらの被害が生じたならば、早期情報収集をして迅速な対応が必要とされるだろう。最近では情報収集の課題解決策としてドローンの活用に注目する自治体が多い。ドローンを使うメリットとしては災害時の交通状況や被害により状況把握が難しい場合、被災状況を早期収集することが可能であることが挙げられる。映像から災害状況を把握することで、自治体は火災の被害が大きい地域に消防を派遣したり、駅周辺や主要道路の帰宅困難者対策を迅速に講じることできる。そして私はこの早期情報収集のためには、ドローンの効率的で計画的なルートも重要であると考え、ドローンの地震時のルートをGoogle Earth Studioでシミュレーションすることを研究目的にした。今回はDRONE BIRDが災害協定を結ぶ世田谷区を対象に作成する。
　
# 研究方法
## 1.geojson.ioで徒歩帰宅支援対象道路、主要駅、火災危険度の高レベルの地域の地図とルートを作成
世田谷区役所を起点として対象の場所の効率的なルートを作成し、場所の名前、ルート名、色分け、ポップアップのシンボル、動画のリンク先をgeojson.ioで分かりやすく一元化する。

### ①徒歩帰宅支援対象道路
<img width="427" alt="帰宅支援対象道路　ズ" src="https://user-images.githubusercontent.com/40257255/105440259-9b51f480-5ca9-11eb-8550-22839d5d92f0.PNG">

東京都が指定する徒歩帰宅支援対象道路のうち世田谷区が指定されている「玉川通り」、「甲州街道」、「井の頭通り」、「環状７号線」、「環状８号線」の５路線のルートを作成する。


**ルート１**　世田谷区役所→環状７号線→井の頭通り→世田谷区役所

**ルート２**　世田谷区役所→環状８号線→世田谷区役所

**ルート３**　世田谷区役所→井の頭通り→甲州街道→世田谷区役所



### ②主要駅
2012年に世田谷区が帰宅困難者対策訓練が実施された、乗客数の多い二子玉川駅、三軒茶屋駅、下北沢駅、成城学園前駅、千歳烏山駅に加え、世田谷区が指定する帰宅困難者支援施設の周辺駅を主要駅とした。

<img width="392" alt="帰宅困難者施設　ず" src="https://user-images.githubusercontent.com/40257255/105441630-51b6d900-5cac-11eb-976e-d00202707039.PNG">

**ルート４**世田谷区役所→新代田駅→下北沢駅→三軒茶屋駅→駒沢大学駅→世田谷区役所

**ルート５**世田谷区役所→桜新町駅→二子玉川駅→成城学園前駅→千歳烏山駅→上北沢駅→経堂駅→世田谷区役所



### ③火災危険度の高レベルの地域
東京都のオープンデータ『地震に関する地域危険度測定調査　地域危険度一覧表（区市町村別）』の世田谷区の中で、地震の時の火災危険度がレベル４の地域を対象にした。

**ルート６**世田谷区役所→上馬一丁目→野沢一丁目→太子堂五丁目→若林二丁目→世田谷区役所

**ルート７**世田谷区役所→松原四丁目→松原一丁目→羽根木二丁目→大原一丁目→北沢五丁目→北沢四丁目→世田谷区役所

**ルート８**世田谷区所→経堂二丁目→船橋一丁目→上祖師谷４丁目→世田谷区役所

## 2.KML形式でgeojson.ioをGoogle Earth Studioにインポート

## 3.Google Earth Studioでシミュレーション動画の作成
geojson.ioで作成した地図を基にGoogle Earth Studioでドローンルートを映像にする。


# 研究結果
## 徒歩帰宅支援対象道路geojson.io
<img width="520" alt="帰宅困難者　主要道路　ルート　geojsonio" src="https://user-images.githubusercontent.com/40257255/105443974-5087ab00-5cb0-11eb-9b9d-356d2659a7a4.PNG">



## 主要駅のgeojson.io
<img width="571" alt="帰宅困難者　主要駅　帰宅困難者支援施設　geojson" src="https://user-images.githubusercontent.com/40257255/105444386-136fe880-5cb1-11eb-82d5-db882338e3ab.PNG">


## 火災危険度の高レベルの地域のgeojson.io
<img width="471" alt="木蜜地域　ルートgeojson" src="https://user-images.githubusercontent.com/40257255/105444637-8d07d680-5cb1-11eb-8a49-5ea463105523.PNG">

## ポップアップ
<img width="186" alt="ポップアップ表示" src="https://user-images.githubusercontent.com/40257255/105444879-09021e80-5cb2-11eb-81b2-af2f5eb93e5d.PNG">

## 動画
ルート７　movie①世田谷区役所→松原四丁目→松原一丁目→羽根木二丁目
(https://drive.google.com/file/d/1nCBB5Yrjn0LrCHM2Sp_oYHN8S_n6t_cs/view?usp=sharing)

ルート７　movie②大原一丁目→北沢五丁目→北沢四丁目→世田谷区役所
(https://drive.google.com/file/d/1WGhAZ0wKJ-v_LMu6VjtnitIpJviP9yyc/view?usp=sharing)
 
上記はGoogle Earth Studioで作成したシミュレーション動画だ。その他の動画はkmlファイルにGoogle Driveのリンクが添付されている。

# 考察・まとめ
ルートを動画や地図にして視覚化することで、地震時にドローンをどう飛ばすべきか事前に把握することができ、迷いなく飛ばせるので迅速な情報収集が出来ることが分かる。さらにgeojson.io上で効率的なルートを作成することでより素早い対応になることも期待できる。また、Google Earth Studioで高度150ｍの高さで飛ばそうとした場合、ビルに衝突する可能性も確認できたので、事故の防止にも繋がる。これらのことからシミュレーション動画を作成するこの研究を通して、実際の地震時同様の動きを明確にでき、対策を練ることが可能と分かった。
次に引き継ぐべき課題とは、その土地をよく知らないと、どの場所を飛ばしているのか上空から見ただけでは場所の見分けがつかないので、緯度経度などの具体的な数値を取り入れた地図の作成をすべきだと考える。

# 謝辞
本研究を進めるにあたり、青山学院大学地球社会共生学部教授の古橋大地氏をはじめ多くの方々より多大な助言を賜りました。厚く感謝申し上げます。

# プレゼン
(https://docs.google.com/presentation/d/e/2PACX-1vS0Jg-aZhjzIH_41sYIKM0PvMqZVeTaXOcZFtvrJEKomjT9ZFMqriJhOugOprtvMTutizOH3D_gYc_6/pub?start=false&loop=false&delayms=3000)

# 進捗管理用プロジェクト
(https://github.com/furuhashilab/sotsuron2020/projects/20)

# 参考文献
(https://docs.google.com/document/d/1UymaFtxnBopRSOId5nLjGKuH9JRI8Oudf48EBCe9cLU/edit)










