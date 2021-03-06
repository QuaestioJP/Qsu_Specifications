# 字句構造
## 行終端子
行は、ASCII文字のCR、LF、CRLFによって終端します。CRLFは2つではなく1つの行終端子としてカウントされます。

## 空白
空白は、行終端子だけではなく、ASCIIのスペース及び水平タブも含みます。

## コメント
Qsuは、2種類のコメントを定義します。
- `/*` から `*/` までのすべてのテキストを無視します。
- `//` から行末までのすべてのテキストを無視します。

## 入力要素文字
行終端子でもなく、コメントでもないものを、入力要素文字とします。

## 識別子
識別子は、大小英数字及びアンダーバーによって交際されるの長さ制限のない列であって、先頭の文字は大小英文字またはアンダーバーでなければなりません。  
識別子は、キーワード、bool型リテラル又はnullリテラルと同じ文字の並びにすることはできません。

## キーワード
ASCII文字列から形成される次の文字列は、キーワードとして予約されており、識別子として使用することはできません。
- `if`
- `else`
- `return`
- `for`
- `while`
- `do`
- `break`
- `continue`
- `let`
- `float`
- `char`
- `int`
- `bool`
- `object`
- `long`
- `double`
- `fn`
- `void`
- `this`
- `new`
- `class`

## リテラル
リテラルは、int型、float型、char型、bool型、string型、null型の値のソースコード表現とします。

### 整数リテラル
整数リテラルは、10進数又は16進数で表現可能とします。  
以下の2つを10進数整数リテラルとします。
- 0
- 1から9までの数字に続く0から9までの数字の繰り返し。(正規表現: `[1-9]\d*`)

以下の1つを16進数整数リテラルとします。
- 文字列`0x`に続く0から9までの数字とaからfまでの文字の繰り返し。(正規表現: `0x[\da-fA-F]+`)

### 浮動小数点数リテラル
浮動小数点数リテラルは、整数部、ピリオド文字、小数部、指数部及び型接尾語、文字`f`の部分をもちます。  
指数部が存在する場合には、e又はE及びそれに続く負符号付き又は符号なしの整数によって示されます。  
以下の2つの正規表現のどちらかに一致する文字列を浮動小数点数リテラルとします。
- `\d+\.\d+(e-?\d+)?f`
- `\d+e-?\d+f`

### bool型リテラル
以下の2つをbool型リテラルとします。
- `true`
- `false`

### 文字リテラル
文字リテラルは、一重引用符で囲まれた入力要素文字またはエスケープシーケンスです。

### 文字列リテラル
文字列リテラルは、二重引用符で囲まれた0個以上の入力要素文字から構成されます。  
各文字は、エスケープシーケンスで表現することも可能です。

### エスケープシーケンス
- `\b` Backspace
- `\t` Horizontal Tab
- `\n` Line Feed
- `\f` Form Feed
- `\r` Carriage Return
- `\"` Double Quote
- `\'` Single Quote
- `\\` Backslash

### nullリテラル
`null`の4文字で構成される文字列を、nullリテラルとします。

## 分離子
以下の文字を分離子とします。
- `,`
- `;`
- `:`
- `(`
- `)`
- `[`
- `]`
- `{`
- `}`

## 演算子
以下のトークンを演算子とします。
- `.`
- `++`
- `--`
- `+`
- `-`
- `!`
- `*`
- `/`
- `%`
- `<`
- `>`
- `<=`
- `>=`
- `==`
- `!=`
- `&`
- `|`
- `^`
- `&&`
- `||`
- `=`
