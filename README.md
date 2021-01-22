# 2020gsc_YunaHomma
本間友那 2020年度ゼミ論用レポジトリ

# Introduction
## 研究内容
世田谷区で地震が起きた時のドローンの撮影ルートをGoogle Earth Studioで想定する。

## 目的
地震大国である日本はいつどこで大きな地震が発生するか分からず、昨今懸念されている大地震の1つに首都直下型地震があり、政府の地震調査委員会によると今後30年以内に70%の確率でマグニチュード約7の地震が関東で予測されている。世界的に見ても過去4番目に大きな地震であった2011年3月の東日本大震災では、首都圏は人的被害、建築物等被害、停電、道路、ライフライン等で被害が生じ、さらに帰宅困難者などの課題も発見されている。また地震が起きてこれらの被害が生じたならば、早期情報収集をして迅速な対応が必要とされるだろう。最近では情報収集の課題解決策としてドローンの活用に注目する自治体が多い。ドローンを使うメリットとしては災害時の交通状況や被害により状況把握が難しい場合、被災状況を早期収集することが可能であることが挙げられる。映像から災害状況を把握することで、自治体は火災の被害が大きい地域に消防を派遣したり、駅周辺や主要道路の帰宅困難者対策を迅速に講じることできる。そして私はこの早期情報収集のためには、ドローンの効率的で計画的なルートも重要であると考え、ドローンの地震時のルートをGoogle Earth Studioでシミュレーションすることを研究目的にした。今回はDRONE BIRDが災害協定を結ぶ世田谷区を対象に作成する。
　
# Method
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

