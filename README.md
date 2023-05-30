# ゲーム のタイトル
エアホッケー
## 実行環境の必要条件
* python >= 3.10
* pygame >= 2.1

## ゲームの概要
１つのPCで2つのスマッシャーを動かし、２人で対戦ができるゲーム

## ゲームの実装
###参考元のゲーム内容
* エアホッケーの当たり判定やゴール、パック、マレットなどの基本的な内容はせていさてていた
* 左側のゴールの当たり判定がない
* 片方のマレットの動きを止めるともう片方のマレットの動きも止まる
* マレットの斜め方向への移動ができない
* ゴールの後はディスクが中央から右下に向かって発射
* マレットが片方しか動くことができない(二つ同時に動かすことができない)
###共通基本機能
* エアホッケーのフィールドに関するクラス
* エアホッケーのマレットに関するクラス
* エアホッケーのパックに関するクラス
###元のゲームを調整
* 斜め方向への移動を可能にさせた
* マレットを２つ同時に動かせるようにした
* ゴールの判定の調整


### 担当追加機能
* マレットに当たるごとに速度変化
* 10点先取で勝利画面の表示
* ５点差がついたとき、同点になるまで負けているほうのマレット　が大きくなる
* 合計得点が5点追加されるごと障害物追加
* お互いの得点差に合わせてゴールの大きさの変化
* ゴールの後ディスクの発射方向をランダムにする
### ToDo
### メモ
* クラス内の変数は，すべて，「get_変数名」という名前のメソッドを介してアクセスするように設計してある
* すべてのクラスに関係する関数は，クラスの外で定義してある
参考文献
https://github.com/mkfeuhrer/Air-hockey