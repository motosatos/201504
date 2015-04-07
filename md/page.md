## 第3章　コンポーネント設計のアイデア

---

1. CSSにおけるコンポーネント設計
2. OOCSS
3. BEM

---

### 3-1 CSSにおけるコンポーネント設計 

--

+ コンポーネントとは
 - 部品だ。目的は部品化することで機能や振る舞いなどを明確に分離する

--

+ カプセル化
 - コンポーネントの構造やデータを隠し、外部からは許可された操作のみを受付、また内部の仕様変更が外部に影響しないようにするといったこと 
  - 分離が成立
  - メンテアップ、再利用性アップ
 - しかし、、

--

+ CSSにはカプセル化の概念がない
 - 容易に他への影響が出る
+ コンポーネント設計が難しいCSSだが、アイデアがある
 - OOCSS 

---

### 3-2. OOCSS(Object Oriented CSS)

--

+ OOCSSの原則
 - 構造と見た目の分離
 - コンテナーとコンテンツを分離

--


---

Markdownだけ別ファイルにしておけば<br>
index.htmlは使いまわせる！

```html
<section data-markdown="./md/firstpage.md"
data-separator="\n---\n$"
data-vertical="\n--\n">
<script type="text/template">
< / script>
</section>
```

---
