# ArchLinuxでトラックパッドのタップ操作を無効にした

タッチ操作ではなくタップ操作の話  

* タッチ -> 押し込む
* タップ -> 触れる

カーソルが良く分からないタイミングで急に移動したりしていたけど、うっかりトラックパッドに触れてタップしていたせいだった


* 修正方法

以下のURLを参考に、xwindowの設定で`Option "Tapping" "Off"`にした

https://gist.github.com/miguelmota/c35999dbf9c15154d0aec8dace29d481
