# About

### test and prototype code memos

- testコードや、プロトタイプのコード群の置き場所
- gitのテストとかもしてるためcommit履歴は汚い(かもしれない)
- ライセンスについて( 念のため...こんな自由帳みたいなソースを利用する人は居ないと思うけど )
  - 特に定めてないです。考えてるのは`CC0`か`Boost Software License 1.0`
  - 今のところ煮るなり焼くなり好きにしてください。特に許可など要らないです
  - `bode.md`のみ許可ください。恥ずかしいのでｗ
- マサカリ
  - Pull Request、issue諸々大歓迎です。遠慮なくマサカリを投げて知見を僕にください（ぇ

### top

- bode.md
  - ただの自己紹介

### cpp
- dispatcher.cpp
  - win32系で使おうと思っているスロット形式のイベント管理prototype

- dispatcher2.cpp
  - dispatcherで使ってる`has_mouse_event`の引数型指定を抽象化しようとしてみたもの

- conditional_helpers.cpp
  - `if`を楽して書きたいという試行錯誤

- numeric_cast.cpp
  - 文字列型を数値型に変換するだけ `boost::lexical_cast`を参考にえらくシンプルにしようとあがいたもの
  - `optional`を使ってるので環境に応じて`boost::optional`使うなりしなければならない

- chrono_time_get.cpp
  - `#include <chrono>`だけで現在時刻を取得することは出来るだろうか。という試み

- multi_vector.cpp
  - `std::vector`を多次元に拡張する時、`vector<vector<vector<...`などと書くのは冗長である
  - それを無くそうとした試み

- tuple_extract_practice.cpp
  - `std::tuple`を逐次展開してみたかった練習
  - 最終的に某先生に助けてもらった

- operator_overalod_prac.cpp
  - operator overloadの練習も兼ねている
  - if文における`(value == 2) || (value == 3)...`みたいなcaseの出来損ないをスマートに書けるように努力したもの
  - scoped enum使った時にerror constantになってしまう

- windows_restart.cpp
  - Windowsで再起動をかけるときに使うコード

- variable_template_bug.cpp
  - Visual Studio 2017のインテリセンスは変数テンプレートに弱い（確信）

### perl
- unused_comment_outer.pl
  - Visual Studio 2017で大量に`C4100`のwarningが出てきた時用に一気にコメントアウトする自分用ツール

- automatic_issue_creator.pl
  - github APIを使用してissueを作成するサンプル
