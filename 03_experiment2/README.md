# 実験用のデータについて

このフォルダには、RoBERTaの頑健性の研究における、実験の手順を実行するために必要なデータが格納されています。

## 概要
事前準備でGLUEのデータを正解と不正解のデータに分けた後、各データの傾向を元に25件ずつ抽出します。
各25件をルールに従って変更したものがdataの中に入っています。  
下記のURLのEvaluateで再び評価  

(参照URL)  
https://github.com/facebookresearch/fairseq/blob/main/examples/roberta/README.glue.md

## 内容物<a name="content"></a>[](#content)

- [dataフォルダ](#data)
### dataフォルダ<a name="data"></a>について[[一覧へ戻る](#content)]

MRPCの場合  
sample_MRPC_right_easy ... 正解したデータの名詞1単語のみを変更した。  
sample_MRPC_right__hard ... 正解データのeasyで変更した以外の部分を変更した。  
sample_MRPC_wrong_easy ... 不正解したデータの名詞1単語のみを変更した。  
sample_MRPC_wrong_hard ... 不正解データのeasyで変更した以外の部分を変更した。  

## 使い方<a name="howtouse"></a>[](#howtouse)

1 pythonコードのopenの中身を実行したいtsvファイルに変更してください。  
2 ターミナルで  
python Evaluate_Sample/Evaluate_MRPC.py と実行してください。(MRPCの場合)

- [注意点](#remarks)

### 注意点<a name="remarks"></a>[[一覧へ戻る](#howtouse)]
研究室のサーバファイル(cafeaulait)につなげた状態で実行してください。
