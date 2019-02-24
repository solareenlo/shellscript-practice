# shellscript-practice

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
01_helloの中身を見てください.

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

## 変数を使う
02_variableの中身を見てください.

## 特殊変数を使う
03_variableの中身を見てください.
```bash
$1 = 第1引数
$2 = 第2引数
$0 = コマンド名
$# = 引数の個数
$@ = 全部の引数
```

## ユーザーに入力してもらう
04_readの中身を見てください.

## 配列を使う
05_arrayの中身を見てください.

## 数値演算を行う
06_num_calの中身を見てください.

## if分を使う
07_ifの中身をご覧ください.

## 文字列の比較を行う
08_compare_stringsの中身をご覧ください.

## ファイルや数値の比較を行う
09_compareの中身をご覧ください.

## forでループ処理を行う
10_forをご覧ください.

## whileでループ処理を行う
11_whileをご覧ください.

## catでテキストファイルの中身に文字を保存する
```bash
cat > colors.txt
red
green
blue
# CTL + d
# で保存
```

## whileを使って, テキストファイルの中身を1行ずつ読み込む
12_read_lineをご覧ください.

## catとwhileを使って, catで表示するものに行番号を付ける
```bash
cat colors.txt | ./13_add_number
# 1 red
# 2 green
# 3 blue
# と表示される
```

## caseを使って条件分岐を行う
14_caseをご覧ください.

## selectを使ってメニューを作る
```bash
./15_select
> 1) red
> 2) blue
> 3) green
> 4)yello
> #?
1
> stop
2
> go
3
> go
4
> caution
5
> wrong signal
```
15_selectをご覧ください.

## 関数を使う
16_funcitonをご覧ください

## 変数スコープについて
17_scopeをご覧ください.
