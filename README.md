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
