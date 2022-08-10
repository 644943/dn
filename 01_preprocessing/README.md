#RoBERTaモデルの頑健性の検証の際の事前準備用のデータについて

このフォルダには、GLUE,CommonsenseQAの元となるデータが入っています。
このデータをRoBERTaに入れて正解したデータと不正解したデータに分ける。

## 概要
trainが学習用データ、devが開発用データ、testがテスト用データとなっています。
実験に使う際はdevを使用して下さい。

## 内容物<a name="content"></a>[](#content)
- [dataフォルダ](#data)

### dataフォルダ<a name="data"></a>について[[一覧へ戻る](#content)]
GLUE,CommonsenseQAの学習、開発、テストデータがフォルダごとに入っています。
