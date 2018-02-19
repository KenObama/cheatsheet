## 導入(Mac)
brew install tree
## 説明
フォルダ構成を表示してくれる便利コマンド。パイプしてgrepすると更に便利。デフォルトだと深さ制限がなしなので注意。自分は下のaliasをしている。
## alias例
t を 'tree -a -d -L 3'にしている。(適当に決めた)
## 便利なオプション
#### Ex1 ディクレクトリだけを表示
```shell
tree -d
```
-d means directory

#### Ex2 深さ制限を2にする	
```shell
tree -L 2
```
-L means LIMIT
#### Ex3 相対パスも表示する(grepするときには便利)
```shell
tree -f
```
-f means ??

#### Ex4. 隠しファイル、フォルダも表示する
```shell
tree -a
```
-a means all
