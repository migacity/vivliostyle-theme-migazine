---
title: Vivliostyleのここが好き
class: text_01
---

<div class="text-header">
    <div class="text-title">Vivliostyleのここが好き</div>
    <div class="text-author">idomshi</div>
</div>
<div class="text-main">

## はじめに

今回（No. 2）、MIGAZINEの制作にVivliostyleという組版プログラムが使われることになったので、なにそれ、どこが良いの？ という話をしたいと思います。これは私の主観でVivliostyleを紹介する記事です。

Vivliostyleは組版プログラムです。組版プログラムは「本を作る際の原稿データを、印刷物として良い感じの見栄えにする」ためのプログラムです。この場合の原稿とは基本的には文章が主体の小説や（プログラミングとかの）技術所であることが多いと思います。ほぼイラストしかないMIGAZINEに使っているのは若干尖った用途であるとも言えそうです。

私は本業で図や表が多く入った文書を作ることが多い。そのため、見た目がスッキリきれいな文書をできるだけ楽に作りたいと思ってきました。そのなかで出会ったのがVivliostyleです。

印刷用の文章を作るプログラム（ワープロソフトなどの組版プログラムとは呼ばないものも含む）の種類は多く、私が触ったことのあるものだけでもMicrosoft Word、LaTeX、Adobe InDesign、Vivliostyle、Pandoc、Asciidoctor、Sphinxなどがあります。Vivliostyleはこの中でもかなり気に入っているプログラムでして、今回はどういうところが好きなのかを語ります。

## 無料で使える

無料だから使っているというわけではありませんが、使い始めるときに有料だと二の足を踏んでしまいます。そういう意味で、無料だからお試しで使ってみようと思ったのは大きなきっかけでした。

他人に薦めるときもどうせタダだから使ってみるだけ使ってみなよと言いやすいです。

## 文書の内容とThemeのデータが別れている

文書の内容を書いたテキストファイルと、紙面上での見た目を定義したThemeファイルが分かれています。

## プロジェクトの管理方法が今風

## Markdownで書ける

Markdownを知っていますか？ Markdownはフォントや文字サイズなどの書式を使わずに、文字だけで見出しや箇条書きを表現する記法です。そのままでも文書構造が一目で分かるほか、書式を設定した文書にコンバートするツールがたくさんあります。Vivliostyleもその一つです。

同じような記法はいくつもありますが昨今ではデファクトスタンダードの地位を築いており、いますので、見たことのある人もいるかもしれません。

ではMarkdownの何が良いのでしょうか。MS Wordではいけないのでしょうか。答えとしては文書構造に集中できることとバージョン管理システムと相性がいいことが挙げられます。

例えばMS Wordではどうしても見た目が気になってしまい、「この大見出しから始まるのが1つの節、節の中にそれぞれ小見出しから始まる小節が3つあって……」といった文書の構造（アウトライン）とは異なった書式を設定してしまうことがあります。もちろんWordにもアウトラインエディタがありますので、構造を崩さずに文章を書くこともできるのですが、おせっかいが過ぎるため文章が長くなるほど書式設定が乱れやすいという問題は残ります。A4用紙1枚にぴったり収めたいなどの用途では、グラフィカルにかつアドホックに書式を設定できるのがWordの強みです。

またLaTeXでは構造を意識した書きかたができますが、見出しや箇条書きの命令がやや長く、気軽に書くのに向かないと感じます。ただし、LaTeXはその長い歴史（LaTeXのベースであるTeXの初版は1978年）の中で培われた組版精度の高さのために使いたくなるタイミングがあります。

その点MarkdownではWindowsのメモ帳で気軽に書き始められて文書構造に集中でき、長大な文章になるときはファイルを分割することもでき、Visual Studio Codeなどを使うと書式を設定した結果も見ながら執筆できるなど、書くことへの心理的負担が低くなっています。あ、でも何をもって負担とするかは人に依るかもしれません。

それから、書式を設定せずにテキストだけで原稿が成り立っているため、バージョン管理システムで管理することができるというのも強みです。バージョン管理システムはもともとプログラムのソースコードを管理するために生まれたプログラムなので、テキスト形式のファイルの扱いに長けています。具体的に言うと、「ファイルのxx行目が変更された」「xx行目の後ろにnn行追加された」というような差分を見やすいのです。そもそも執筆にバージョン管理システムを使うメリットを説明するのは難しいのですが、使った後ならわかる安心感があるので、使えるなら使いたいものだと思ってください。

## コマンドラインで使う

MarkdownやHTMLの文書をPDFに変換する操作は、基本的にはコマンド操作です。WindowsならPowerShellなどで次のように入力します。

```powershell
vivliostyle input.md
```

黒い画面にキーボード入力！ うひゃぁ！ と感じるひともいるでしょうが、これ、自動化しやすいのです。「xxのボタンを探してマウスでクリック」よりも「このコマンドを実行」の方がコンピュータには理解しやすい、だから確実に自動化できる。ほかのプロセスにも組み込みやすい。

技術文書でも小説でもイラスト集でも、本を作る作業は工程が多いため、自動化できて毎回同じ作業を確実に実行できるようにしておくのは重要なことです。プログラマは手を抜くためなら全力でめんどくさいことをするのです。

## Vivliostyleの良いとは言えないところ

ここまでVivliostyleの好きなところを書いてきました。しかし好きにはなれないところも少なからずあります。いくつか紹介しましょう。

### Themeファイルを作りこむのが面倒

文書の内容（Markdown）と見た目（Theme）が明確に分かれているのがVivliostyleのいいところではあるのですが、どんな文書にでも使える万能のThemeを作るのは本当に難しいです。見出しの文字サイズは何ptがいいのか、見出しの上下はどのくらい開けたほうがいいのか、あの文書ではちょうどよかったがこちらでは行数が微妙……など、調整を始めたらキリがないものですし、個々の文書ごとにThemeを作るのはちょっと違います。

このように、最大の利点にして最大の欠点であるThemeを、いくつもの文書を作りながらいかに地道に育てるかというのは気長な戦いになります。残念ながら公式のThemeを使ってもすべての痒いところには手が届きません。この戦いを続けられるか、途中であきらめるか試されるのは欠点といえるでしょう。

### 一般人にMarkdownはわかりづらい

最終的な見た目通りに書けないMarkdownは気軽に他人にお勧めできない記法です。普段からプログラムを書くような人には受け入れやすいのですが、そうでない人にとっては分かりづらいと思います。

インターネット上のサービスではMarkdownを使える場面が増えている（GitHub、Notion、いくつかのWikiやBlogなど）ので、覚えてみてはいかがですか。

### 細かい調整が難しい

あと一行分詰めると1ページに納まるんだけどなぁ！ というときは行送りをちょっとだけ小さくしたくなりますよね。しかしVivliostyleではThemeを文書全体、ほかの文書でも共有していますので、基本的には特定の文書向けの微調整を行いません。1行詰めたいときは文の言い回しを修正する方がいいでしょう。

文書ごとの微調整が重要な場合は最初からWordなどのワープロソフトを使う方が幸せになれます。

Vivliostyleで細かい調整や特殊なレイアウトが必要なときは、MarkdownのなかにHTMLをべた書きすることができます。これは裏技とかではなく一般的なテクニックです。ただし、文書全体の統一感が無くなるとThemeを使っている意味が薄れる（し、そもそもHTMLを書きたくないからMarkdownを使っている）ので使いどころが限られます。

### 複雑な表を表現するのが苦手

Markdownの仕様のせいでセルの結合ができません。複雑な表を作るならSphinx（reStructuredText）が強いです。Asciidoctor（Asciidoc）でも、Sphinxよりちょっと分かりづらい記法ですが、セル結合が表現できます。

Vivliostyleで複雑な表を作る時はHTMLで書くか、別のソフトで作った表を図として読み込むのが正攻法だと思います。Markdownの手軽さが失われてしまうので惜しいところだと思います。

### おわりに

内なる自分が「Vivliostyleの好きなところ10個言って」という（めんどくさい彼女みたいな）お題を出してくれたので文字数が埋まりました、という話をしたいのではなくて。10個も挙げてないし。

先にも書いた通り、様々な文書作成プログラム・組版プログラムをかじってきた中で思うことは、痒いところ全てに手が届くツールはなかなか無いということです。私の主観では。

たとえば、ホビーユースのLaTeX人口がもうちょっと多かったらそもそもほかのツールは探してなかったかもしれないし、AsciidoctorやPandocのデフォルトスタイルに少ページ文書向けのものがあったら十分満足できていたでしょう（Vivliostyleの前にスタイルを作りこんでいたPandocもまだ使っていますしね）。逆に、今後Markdownで表を書くのに疲れてほかのツールに移っていってしまう可能性も大いにあります。しかし今はVivliostyleがとても良く私の要求に応えてくれていて、むこう数年は使いこんでいきたいと感じています。

文章を書くことや本をつくることが楽しくなるツールがあることはとてもうれしいことです。幸運にもVivliostyleというちょうどいいツールがあって、文章主体の本だけでなくイラスト集にも使えることを今回、MIGAZINEが見せてくれました。

本記事を通してVivliostyleをはじめとした組版プログラムに興味を持つ人が1人でもいたらいいなと思います。

</div>