#shell-script-practice

## 初めてのシェルスクリプト
- シェルとはOSと対話するためにインターフェースであり, それのスクリプトがシェルスクリプト.
```bash
# まず, bashがどこにあるか調べる
which bash
> /bin/bash
```
- #!のことを「シェバン」もしくは「シバン」という.
- shell scriptファイルの頭に`#! /bin/bash`と書いてあげる.

```bash
vim hello
i
#i /bin/bash
echo hello
Esc
:wq

ls -l
> -rw-rw-r--. 1 solareenlo solareenlo 24 日付 hello
chmod +x hello
ls -l
> -rwxrwxr-x. 1 solareenlo solareenlo 24 日付 hello
./hello
> hello
```
## 文字列を表示する
```bash
vim hello
i
#!/bin/bash
# コメントは#を使うと文末までコメントアウトしてくれる

echo "hello world"
echo 'hello world'

echo "foo"; echo "bar";
ESC
:wq

./hello
> hello world
> hello world
> foo
> bar
```
