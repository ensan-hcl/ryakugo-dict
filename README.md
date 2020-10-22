# ryakugo-dict

「とく＝ておく」のような略語の語彙で左文脈idと右文脈idが異なるように上書きするMeCab用ユーザ辞書です。

A user dictionary csv file for MeCab which contains ryakugo data with different left and right attribute id.

## Usage
下のリンクのドキュメントを読んで手順に従ってください。

read the following document and follow the steps.

https://taku910.github.io/mecab/dic.html


⚠️記載されているコマンドは正しくないことに注意してください。

⚠️Note that the command is incorrect. 

```
% /usr/local/libexec/mecab/mecab-dict-index -d/usr/local/lib/mecab/dic/ipadic \
-u foo.dic -f euc-jp -t euc-jp foo.csv
```
代わりにこちらを使ってください。

Please use this instead.

```
% /usr/local/libexec/mecab/mecab-dict-index -d/usr/local/lib/mecab/dic/ipadic \
-u foo.dic -f utf8 -t utf8 foo.csv
```
