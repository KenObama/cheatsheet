## 構文
grep [オプション] [単語] [ディレクトリ]

#### Ex1 ./srcディレクトリ以下のfooの出現を探す
```shell
grep -r foo src
```
-r == --recursive

#### Ex2 ./srcディレクトリ以下のfooの出現を探し、行番号も出力する
```shell
grep -rn foo src
```
-r == --recursive

-n == --line-number
#### Ex3 ./srcディレクトリ以下のfooの出現回数を調べる
```shell
grep -rc foo src
```
-r == --recursive

-c == --count

#### Ex4. 正規表現を使う
```shell
grep -r '^foo$' src #fooのみの行を探す
```
-r == --recursive

^ :行頭

$ :行末
