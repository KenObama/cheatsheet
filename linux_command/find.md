## 構文
find [ディレクトリ] [オプション]
## 使用例
#### Ex1 ./以下の全てのディレクトリ・ファイルを表示する
```shell
find .
```
#### Ex2 ./以下にある全てのindex.htmlを探す(ディレクトリ、ファイル両方が表示される)
```shell
find . -name index.html
```
名前が空白を含むときは、' か ” で囲う

#### Ex3 ./以下のuserを含むファイルを探す
```shell
find . -name '*user*' -type f
```
userだけだと、完全に一致するものしか検索しないので、'\*user\*'とする。


''については下を参照。
https://unix.stackexchange.com/a/123441


-type f でfileのみを、

-type d でdirectoryのみを検索する
