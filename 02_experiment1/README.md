# 実験用のデータについて

このフォルダには、RoBERTaの頑健性の研究における、実験の手順を実行するために必要なデータが格納されています。

## 概要
事前準備でCommonsenseQAのデータを正解と不正解のデータに分けた後、各データの傾向を元に25件ずつ抽出します。
各25件をルールに従って変更したものがdataの中に入っています。  
下記のURLのEvaluateで再び評価  

(参照URL)  
https://github.com/facebookresearch/fairseq/blob/main/examples/roberta/commonsense_qa/README.md

## 内容物<a name="content"></a>[](#content)

- [dataフォルダ](#data)
### dataフォルダ<a name="data"></a>について[[一覧へ戻る](#content)]
sample_common_right_answer ... 正解したデータの選択肢の部分を変更した。
sample_common_right_question ... 正解したデータの質問の部分を変更した。
sample_common_wrong_answer ... 不正解したデータの選択肢の部分を変更した。
sample_common_wrong_question ... 不正解したデータの質問の部分を変更した。

## 使い方<a name="howtouse"></a>[](#howtouse)

1 pythonコードのopenの中身を実行したいjsonlファイルに変更してください。
2 ターミナルで
python Evaluate_Sample/Evaluate_Commonsense.py と実行してください。

- [注意点](#remarks)

### 注意点<a name="remarks"></a>[[一覧へ戻る](#howtouse)]
研究室のサーバファイル(cafeaulait)につなげた状態で実行してください。
