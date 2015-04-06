## MarkdownとReveal.js
###で簡単スライド作成
by [@yshimizu0617](https://twitter.com/yshimizu0617)

---

## スライド作り…

--

##めんどくさい！

--

##Office2013…？
<br>
###なんかUI全然違うよ…？

--

##Keynote…？
###会社はWinだって＼(^o^)／

--

#ということで。。。
###スライドもMarkdownで作りたい！

---

#Markdown
#&
#Reveal.js

---

#やり方

---

* GitHubから[reveal.js](https://github.com/hakimel/reveal.js/)のzipをGET
* index.htmlをテキストエディタで開く。
* `<div class="slides">`タグ内の`<section>`内容を削除
* 次のページのオプション付き`<section>`を記載する
* `<section>`内にMarkdownでゴリゴリ書く

<br>
###これだけ！！

---

###Markdown用のsection定義。
`---`を入れることで右に次のページを作成。<br>
`--`を入れることで下に次のページを作成。

```html
<section data-markdown
	data-separator="\n---\n$"
	data-vertical="\n--\n">
	<script type="text/template">
	< / script>
</section>
```



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


`<iframe>`で埋め込みしたいときなどは

おとなしくHTML使ってね！

その他詳細な使い方はGitHubの[README.md](https://github.com/hakimel/reveal.js/)を参照
