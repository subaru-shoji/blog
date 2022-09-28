# debtapを使ってArch LinuxでdebianパッケージをインストールしてArch Linuxを最強にする

Arch LinuxはArchの公式リポジトリに加えて、AURまであるのでほとんどの場合ツールのインストールに困りません。

さらにUbuntu等でよく使われるSnapをインストールすると、たいていのGUIアプリもインストールできます。（snapだと日本語入力できないとかありましたけど）

ただし、まれに上記のどれでもなく、ツールがdebian用パッケージでだけ配布されている場合があります。

そんな時は、`debtap`を使いましょう。
`debtap`を使うと、debianパッケージをArch用のパッケージに変換してインストールができます。

https://github.com/helixarch/debtap



## 使い方

GithubのREADMEを読むのが一番正しいので、概要だけ説明します。

debtapはAURに登録されているので、AURヘルパーを使ってインストールします。

```shell
yay -S debtap
```



インストールしたら、最初にdebtap自体のセットアップのためのコマンドをroot権限で実行する必要があります。

```shell
sudo debtap -u
```

ここから実際にdebianファイルをArch用のパッケージファイルに変換してインストールする作業に入ります。

```shell
# ここはroot権限は不要
# 完了すると、xxx.zstファイルができる
debtap xxx.debian

# できあがったパッケージをpacmanでインストール
sudo pacman -U xxx.zst
```



## 感想

最強じゃん！！！