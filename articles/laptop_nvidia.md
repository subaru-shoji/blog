# nvidiaのグラボ付きノートパソコンにUbuntuをインストールしてnvidiaのドライバーを動かした忘備録

* とりあえずgnomeを使う。事故りづらい。
* 公式ドライバとprime-selectを使う
* 最初は`prime-select intel`を使う。`prime-select nvidia`を最初から使うと大体事故る。
* `prime-select nvidia`を使う前にxserverなしで起動できるようにしておく。事故ってからだと遅い。
* xrandrの設定ファイルはいじらない。`prime-select`がファイルを書き換えるので、わけわからんことになる。
* virtual screenは全然動かないと考える。
