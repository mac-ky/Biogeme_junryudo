# 多項ロジットモデルの推定コード
交通手段選択を扱う多項ロジットモデルの推定方法をまとめました．

使用するデータは[第6回全国旅客純流動調査](https://www.mlit.go.jp/sogoseisaku/soukou/sogoseisaku_soukou_fr_000016.html)で，[e-Stat](https://www.e-stat.go.jp/stat-search/files?page=1&toukei=00600465&tstat=000001218540)で公開されています．

今回はモデル推定に際して，[都道府県間流動表の出発地から目的地のデータ](https://www.e-stat.go.jp/stat-search/files?page=1&layout=datalist&toukei=00600465&tstat=000001218540&cycle=0&tclass1=000001218541&tclass2=000001218542&tclass3=000001218543&tclass4val=0)を使用します．

また，[OD別交通サービス水準](https://www.e-stat.go.jp/stat-search/files?page=1&layout=datalist&toukei=00600465&tstat=000001218540&cycle=0&tclass1=000001218541&tclass2=000001219583&tclass3val=0)の，OD別所要時間のexcelとOD別費用のexcelを加工して使用します．


## データの出典
全国幹線旅客純流動調査(国土交通省)を加工して作成