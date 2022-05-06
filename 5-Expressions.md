# 式
式は、演算子とオペランドにより構成されます。  

## 演算子
### 結合優先順位
<table>
  <tr>
    <th>結合度</th>
    <th>種類</th>
    <th>結合方向</th>
    <th>演算子</th>
  </tr>
  <tr>
    <td>1</td>
    <td>グループ化</td>
    <td>なし</td>
    <td><code>(</code> ... <code>)</code></td>
  </tr>
  <tr>
    <td rowspan="3">2</td>
    <td>メンバーアクセス</td>
    <td rowspan="3">左から右</td>
    <td>... <code>.</code> ...</td>
  </tr>
  <tr>
    <td>インデックスアクセス</td>
    <td>... <code>[</code> ... <code>]</code></td>
  </tr>
  <tr>
    <td>メソッド呼び出し</td>
    <td>... <code>(</code> ... <code>)</code></td>
  </tr>
  <tr>
    <td rowspan="2">3</td>
    <td>後置インクリメント</td>
    <td rowspan="2">なし</td>
    <td>... <code>++</code></td>
  </tr>
  <tr>
    <td>後置デクリメント</td>
    <td>... <code>--</code></td>
  </tr>
  <tr>
    <td rowspan="5">4</td>
    <td>単項＋</td>
    <td rowspan="5">右から左</td>
    <td><code>+</code> ...</td>
  </tr>
  <tr>
    <td>単項－</td>
    <td><code>-</code> ...</td>
  </tr>
  <tr>
    <td>前置インクリメント</td>
    <td><code>++</code> ...</td>
  </tr>
  <tr>
    <td>前置デクリメント</td>
    <td><code>--</code> ...</td>
  </tr>
  <tr>
    <td>論理否定</td>
    <td><code>!</code> ...</td>
  </tr>
  <tr>
    <td rowspan="3">5</td>
    <td rowspan="3">乗除</td>
    <td rowspan="14">左から右</td>
    <td>... <code>*</code> ...</td>
  </tr>
  <tr>
    <td>... <code>/</code> ...</td>
  </tr>
  <tr>
    <td>... <code>%</code> ...</td>
  </tr>
  <tr>
    <td rowspan="2">6</td>
    <td rowspan="2">加減</td>
    <td>... <code>+</code> ...</td>
  </tr>
  <tr>
    <td>... <code>-</code> ...</td>
  </tr>
  <tr>
    <td rowspan="4">7</td>
    <td rowspan="4">大小比較</td>
    <td>... <code><</code> ...</td>
  </tr>
  <tr>
    <td>... <code>></code> ...</td>
  </tr>
  <tr>
    <td>... <code><=</code> ...</td>
  </tr>
  <tr>
    <td>... <code>>=</code> ...</td>
  </tr>
  <tr>
    <td>8</td>
    <td>ビット論理積</td>
    <td>... <code>&</code> ...</td>
  </tr>
  <tr>
    <td>9</td>
    <td>ビット論理和</td>
    <td>... <code>|</code> ...</td>
  </tr>
  <tr>
    <td>10</td>
    <td>ビット排他的論理和</td>
    <td>... <code>^</code> ...</td>
  </tr>
  <tr>
    <td>11</td>
    <td>論理積</td>
    <td>... <code>&&</code> ...</td>
  </tr>
  <tr>
    <td>12</td>
    <td>論理和</td>
    <td>... <code>||</code> ...</td>
  </tr>
  <tr>
    <td>13</td>
    <td>代入</td>
    <td>右から左</td>
    <td>... <code>=</code> ...</td>
  </tr>
</table>
