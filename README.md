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
[01_hello](https://github.com/solareenlo/shellscript-practice/blob/master/01_hello)の中身を見てください.

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
[02_variable](https://github.com/solareenlo/shellscript-practice/blob/master/02_variable)の中身を見てください.

## 特殊変数を使う
[03_variable](https://github.com/solareenlo/shellscript-practice/blob/master/03_variable)の中身を見てください.
```bash
$1 = 第1引数
$2 = 第2引数
$0 = コマンド名
$# = 引数の個数
$@ = 全部の引数
```

## ユーザーに入力してもらう
[04_read](https://github.com/solareenlo/shellscript-practice/blob/master/04_read)の中身を見てください.

## 配列を使う
[05_array](https://github.com/solareenlo/shellscript-practice/blob/master/05_array)の中身を見てください.

## 数値演算を行う
[06_num_cal](https://github.com/solareenlo/shellscript-practice/blob/master/06_num_cal)の中身を見てください.

## if分を使う
[07_if](https://github.com/solareenlo/shellscript-practice/blob/master/07_if)の中身をご覧ください.

## 文字列の比較を行う
[08_compare_strings](https://github.com/solareenlo/shellscript-practice/blob/master/08_compare_strings)の中身をご覧ください.

## ファイルや数値の比較を行う
[09_compare](https://github.com/solareenlo/shellscript-practice/blob/master/09_compare)の中身をご覧ください.

## forでループ処理を行う
[10_for](https://github.com/solareenlo/shellscript-practice/blob/master/10_for)をご覧ください.

## whileでループ処理を行う
[11_while](https://github.com/solareenlo/shellscript-practice/blob/master/11_while)をご覧ください.

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
[12_read_line](https://github.com/solareenlo/shellscript-practice/blob/master/12_read_line)をご覧ください.

## catとwhileを使って, catで表示するものに行番号を付ける
```bash
cat colors.txt | ./13_add_number
# 1 red
# 2 green
# 3 blue
# と表示される
```
[13_add_number](https://github.com/solareenlo/shellscript-practice/blob/master/13_add_number)をご覧ください.

## caseを使って条件分岐を行う
[14_case](https://github.com/solareenlo/shellscript-practice/blob/master/14_case)をご覧ください.

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
[15_select](https://github.com/solareenlo/shellscript-practice/blob/master/15_select)をご覧ください.

## 関数を使う
[16_funciton](https://github.com/solareenlo/shellscript-practice/blob/master/16_function)をご覧ください

## 変数スコープについて
[17_scope](https://github.com/solareenlo/shellscript-practice/blob/master/17_scope)をご覧ください.
