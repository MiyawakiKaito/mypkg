![test](https://github.com/MiyawakiKaito/mypkg/actions/workflows/test.yml/badge.svg)

# mypkg

このリポジトリは2022年度のロボットシステム学の講義で扱ったROS2のパッケージである。

## パッケージの説明
### ノード
* talker
  * パブリッシャを持ち、数字をカウントするノード
* listener
  * サブスクライバ―を持ち、トピックを通じて受け取ったメッセージを表示するノード

### トピック
* /countup
  * talkerから受け取ったメッセージをlistenerに渡す。メッセージの型は16ビットの符号つき整数である。

## 実行方法
```
$ ros2 launch mypkg talk_listen.launch.py
```
### 実行結果
```
[listener-2] [INFO] [1672796251.072674100] [listener]: Listen: 0
[listener-2] [INFO] [1672796251.559227600] [listener]: Listen: 1
[listener-2] [INFO] [1672796252.059344800] [listener]: Listen: 2

・・・
```

## 必要なソフトウェア
* ROS2
  * バージョン : foxy

## 動作確認済み環境
* Ubuntu20.04 LTS

## ライセンス
* このソフトウェアパッケージは，3条項BSDライセンスの下，再頒布および使用が許可されます．
* このパッケージのコードは，下記のスライド（CC-BY-SA 4.0 by Ryuichi Ueda）のものを，本人の許可を得て自身の著作としたものです．
  * [ryuichiueda/my_slides robosys_2022](https://github.com/ryuichiueda/my_slides/tree/master/robosys_2022)

* © 2022 Miyawaki Kaito


