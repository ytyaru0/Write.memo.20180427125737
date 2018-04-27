# Licenseについての検討

創作物におけるライセンスはCCが有名かつ一般的である。

練習用の文章については誰でも閲覧、改変できるようにしたい。CCライセンスが妥当か。

商用の文章については対象外。CCライセンスは不適切。

## Creative Commons

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

付与する。同様のライセンスを強制する。

#### ND

付与しない。改変禁止はしない。改変許可する。

