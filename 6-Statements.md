**このページおよび言語仕様は作成中です**
<hr>

# 文
Qsuのプログラムは、文によって構成されます。  
以下は、その種類と構文です。

## ローカル変数宣言文
- *\<type\> \<identifier\>* **;**
- *\<type\> \<identifier\>* **=** *\<expression\>* **;**
- **let** *\<identifier\>* **=** *\<expression\>* **;**

## 式文
- *\<expression\>* **;**

## 条件分岐文
- **if (** *\<expression\>* **) {** *\<statementList\>* **}**
- **if (** *\<expression\>* **) {** *\<statementList\>* **} else {** *\<statementList\>* **}**

## 繰り返し文
- **while (** *\<expression\>* **) {** *\<statementList\>* **}**
- for文の構文定義は保留

## ループ制御
- **break ;**
- **continue ;**

## 関数終了文
- **return ;**
- **return** *\<expression\>* **;**
