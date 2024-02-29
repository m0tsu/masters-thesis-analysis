# 概要
このリポジトリには、私の修士論文で使用したコードに類似した内容が含まれています。元のコードは共同研究の一環として開発されたため、守秘義務により公開できません。そのため、ChatGPTを利用して、守秘義務に違反しない範囲で同様の機能を持つコードを再作成しました。

# 処理内容の概要
* データ前処理: データ形式の乱れを整理し、異常値の切り捨てを行いました。
* データ分析: データを可視化し、分析を繰り返し行いました。
* 時系列データ処理: 時系列データの欠損補完や、データの正規分布への変換（対数変換やYeo-Johnson変換）を試み、Shapiro-WilkテストとKolmogorov-Smirnovテストで正規性を確認しました。
* 特徴量選択: 相関が高い特徴量を除外し、XGBoostを使用して予測モデルを作成、特徴量の重要度を評価しました。
* 最適な特徴量の選定: AUCを最大化する特徴量の組み合わせを求めました。
* 追加の機械学習手法の試行: PyCaretを使用して様々な機械学習手法を比較し、LSTMを用いた時系列予測も行いました。

# 研究の背景
この研究では、患者データの計測間隔が1日1回であったため、XGBoostのような非時系列手法を選択しました。計測忘れによる欠損データへの対応も重要な課題でした。

# 備考
* このリポジトリのコードは、元の修士論文のコードを基にしていますが、守秘義務の範囲内で変更が加えられています。
* コードは各セルごとに変換されており、一部冗長なコードが含まれている可能性がありますが、研究の全体的なアプローチを理解するための参考としてご覧ください。
