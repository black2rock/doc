# tig使ってみた

gitクライアントツールでtigなるものがあると知り、使ってみました。
## 動作環境
macOS Mojave
(バージョン10.14.4)

## tigとは
ncursesベースのgitのテキストモードインターフェースツールです。（※ncursesとは、端末のテキストユーザインタフェース（TUI）を作成する際のライブラリのこと）

### インストール
homebrewを使用してインストールします。
```
$ brew install tig
$ tig --version
tig version 2.4.1
ncurses version 5.7.20081102
readline version 8.0
```

### 使い方
とりあえず、tigコマンドを叩きます。
```
tig
```

tigには、複数のビューが存在しており、
viライクなコマンドでビューを切り替えて操作します。

| コマンド | アクション | 
| --- | --- |
| m | mainビューへ切り替え | 
| d | diffビューへ切り替え | 
| l | logビューへ切り替え | 
| p | pagerビューへ切り替え | 
| t | (directory) treeビューへ切り替え | 
| f | file blobビューへ切り替え | 
| g | grepビューへ切り替え | 
| b | blameビューへ切り替え | 
| r | refsビューへ切り替え |
| y | stashビューへ切り替え |
| h | helpビューへ切り替え |
| s | statusビューへ切り替え |
| c | stageビューへ切り替え |

各ビューに置けるカーソルの操作は、まさにvi操作と同様、j,kやCtl+d,Ctl+uで上下操作します。
操作についての詳細は、マニュアルに詳しく記載されているためここでは割愛します。

## まとめ


## 参考
[tig公式サイト](https://github.com/jonas/tig)

[tigでgitをもっと便利に！ addやcommitも](https://qiita.com/suino/items/b0dae7e00bd7165f79ea)