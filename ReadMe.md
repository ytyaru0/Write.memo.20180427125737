# このソフトウェアについて

文章における成果物について考える。

## 目的

文章を書く練習が目的。公開することで指摘をもらったり、二次創作してもらって参考にすることが狙い。公開しないと気合も入らない。公開はアウトプットする意識づくりの口実にもなる。

## Licenseについての検討

創作物におけるライセンスはCCが有名かつ一般的である。

練習用の文章については誰でも閲覧、改変できるようにしたい。CCライセンスが妥当か。

商用の文章についてはCCライセンスは不適切。

### Creative Commons

* https://creativecommons.org/choose/
* https://creativecommons.jp/licenses/

CC|表示|継承|改変禁止|非営利
--|----|----|--------|------
CC0     | | | | |
CC-BY   |o| | | |
CC-BY-SA|o|o| | |
CC-BY-ND|o| |o| |
CC-BY-NC|o| | |o|
CC-BY-NC-SA|o|o| |o|
CC-BY-NC-ND|o| |o|o|

### GitHub

* https://help.github.com/articles/licensing-a-repository/

GitHubにあるCCライセンスは以下3つ。おそらくオープンソースにできるライセンスと思われる。

CC|表示|継承|改変禁止|非営利|GitHubiでの名
--|----|----|--------|------|-------------
CC0     | | | | |`cc0-1.0`
CC-BY   |o| | | |`cc-by-4.0`
CC-BY-SA|o|o| | |`cc-by-sa-4.0`

[CC0]: https://creativecommons.org/publicdomain/zero/1.0/deed.ja
[CC-BY 4.0]: https://creativecommons.org/licenses/by/4.0/deed.ja
[CC-BY-SA 4.0]: https://creativecommons.org/licenses/by-sa/4.0/legalcode.ja
[CC-BY-NC-SA 4.0]: https://creativecommons.org/licenses/by-nc-sa/4.0/deed.ja

### CC-BY-NC-SA 4.0

創作物（練習を含む作品）には CC-BY-NC-SA 4.0 を採用する

理由は、文章作品を作ることを目的にしたいから。営利目的の道具にされたくないから。

#### BY

付与する。

* 著者を明示して作品のライセンスを明確にしたい
* 著者、作品へのリンクから閲覧者を増やしたい
* 派生作品ができた場合、原作者を示すものとして利用したい
    * (原作者が派生作品の発生を瞬時に知れると面白そう。閲覧者の増加にもなる)

表記例は以下。

* `(C) *1 *2 *3`

位置|内容
----|----
`*1`|公開年
`*2`|著者名
`*3`|作品名

* `(C) 2018 ytwrite`
* `(C) 2018 ytwrite 作品名`
* `(C) 2018 ytwrite 作品名`

#### NC

付与する。営利目的を禁止する。


文章の練習が目的。たとえば例文を作り、それを元に誰かに改変をさせるようなお題を出したとき、出題者と回答者の双方がどちらも勝手に営利目的に利用されないことを意図する。

作品を勝手に有料サイトにアップロードして小遣い稼ぎに使われていた、という話を聞いたことがある。このようなことを防ぐため。

#### SA

#### BY

公開することで誰かが改変することを許容する。

#### ND
#### NC

CC-BY-SA|

## 前回まで

* [Gulp.Install.20180425070000](https://github.com/ytyaru/Gulp.Install.20180425070000)
* [Node.Gulp.Markdownit.20180425123432](https://github.com/ytyaru/Node.Gulp.Markdownit.20180425123432)

# 使い方

## node_modules インストール

```sh
$ cd (このディレクトリ)
$ npm i
```

* package.json
* node_modules/
* dst/

[※](memo/install.md)

## 起動

```sh
$ cd (このディレクトリ)
$ gulp
```

* ビルド（ファイル結合, トランスパイル）
* ブラウザ起動

なお、`./dst/`配下のpug,stylus,jsのソースコードが変更されるたびに自動でビルド＆ブラウザ更新される。詳細は[gulpfile.js](gulpfile.js)参照。

### 起動

ローカルサーバ、ブラウザ、が起動し、./index.htmlが表示される。

ローカルサーバはターミナルで`Ctrl+C`キー入力すれば停止できる。(Ctrl+Zで強制終了してしまうとプロセスが残ってしまう模様)[※](run.md)

# 開発環境

2018-04-24時点。[※](memo/install.md)

* [Raspberry Pi](https://ja.wikipedia.org/wiki/Raspberry_Pi) 3 Model B
    * [Raspbian](https://www.raspberrypi.org/downloads/raspbian/) GNU/Linux 8.0 (jessie)
        * vim 7.4
        * Chromium 56.0.2924.84
        * Node.js 9.4.0
            * npm 5.6.0
                * n 2.1.7
                * Gulp 3.9.1
                    * 他
                        * gulp-plumber 1.2.0
                        * gulp-notify 3.2.0
                        * browser-sync 2.23.7
                    * HTML
                        * gulp-pug 4.0.1
                    * CSS
                        * gulp-stylus 2.7.0
                    * JS
                        * webpack 4.6.0
                        * webpack-stream 4.0.3
                        * gulp-babel 7.0.1
                        * babel 6.23.0
                        * babel-env 2.4.1
                        * babel-polyfill 6.26.0
                        * babel-preset-env 1.6.1
                    * Markdown
                        * highlightjs 9.10.0
                        * markdown-it 8.4.1
                        * markdown-it-anchor 4.0.0
                        * markdown-it-deflist 2.0.3
                        * markdown-it-kbd 1.1.1
                        * markdown-it-multimd-table 3.1.2
                        * markdown-it-ruby 0.1.1

# ライセンス

このソフトウェアはCC0ライセンスである。

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png "CC0")](http://creativecommons.org/publicdomain/zero/1.0/deed.ja)

