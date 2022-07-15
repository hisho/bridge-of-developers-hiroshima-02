---
theme: penguin


layout: intro
---
# 1週間でNestJS完全に理解した


---
layout: presenter
presenterImage: 'https://user-images.githubusercontent.com/56404715/179198206-455311de-d952-40bd-a652-1d603dfdfc7f.jpg'
---

# hisho

フリーランス フロントエンドエンジニア   
TypeScriptとReactが好き   
最近パーマかけました

```shell
$ npx @hisho/card
```

- ニート
- 職業訓練
- i社で2年アルバイト
- フリーランス

---
layout: intro
---
# NestJSはご存知ですか？

---
layout: intro
---


<div class="absolute inset-0 bg-black flex items-center justify-center">
<img style="width: 70%" src="/images/nextjs-logo.png">
</div>

---
layout: intro
---
<h1 class="relative z-20">🤔</h1>
<div class="absolute inset-0 bg-black flex items-center justify-center" />

---
layout: intro
---


<div class="absolute inset-0 bg-black flex items-center justify-center">
<img style="width: 70%" src="/images/nuxt-logo.png">
</div>

---
layout: intro
---
<h1 class="relative z-20">🤔</h1>
<div class="absolute inset-0 bg-black flex items-center justify-center" />

---
layout: intro
---
<div class="absolute inset-0 bg-black flex items-center justify-center" >
<img src="/images/nest-logo.png">
</div>

---
layout: intro
---
<div class="absolute inset-0 bg-black flex items-center justify-center" >
<img src="/images/nest-cat.png">
</div>

---
layout: intro
---

# Nest🤗

---
layout: intro
---
# NestJSとは

---
layout: intro
---
# Node.js(TypeScript)で<br />バックエンドが書ける


---
layout: intro
---
# なぜやったのか

---
layout: new-section
---

# なぜやったのか

<ul class="text-left text-3xl relative z-20 flex-1">
  <li>1 年間 React でフロントを書いたのでバックエンドも書きたい</li>
  <li>当時ジョインしていたプロジェクトでバックエンドができていなかったので自分が作れば早くねって思った</li>
  <li>なんとなく何をすればいいのか処理はわかるので自分で書けそうだと思った</li>
  <li>フルスタックかっこよくない？</li>
</ul>

---
layout: intro
---
# なにをやったか


---
layout: new-section
---

# 一週間でやった内容
<ul class="text-left text-3xl relative z-20 flex-1">
  <li>NestJS で graphql のバックエンドを構築した</li>
  <ul>
    <li>Query 作成</li>
    <li>Mutation 作成</li>
    <li>JWT の Auth 作成</li>
    <li>JWT の認証のガード実装</li>
  </ul>
</ul>

---
layout: intro
---
# Nestの話をしても・・・

<!--
NestJSの具体的な話をしても分からないので勉強した方法について語る
-->

---
layout: intro
---
# 自分が勉強した<br />具体的な内容を話します！

<!--
自分がした具体的な勉強法について語る
-->

---
layout: new-section
---
# 大まかな計画を建てる

<ol class="text-left text-3xl relative z-20 flex-1">
  <li>前提知識から情報を整理する</li>
  <li>技術選定</li>
  <li>ゴールを明確にする</li>
  <li>今回やらない範囲を決める</li>
  <li>進め方を決める</li>
  <li>手を動かす</li>
  <li>自分で考える</li>
</ol>

---
layout: new-section
---

# 1. 前提知識から情報を整理する

<ol class="text-left text-3xl relative z-20 flex-1">
  <li>今の自分が分かる、できること</li>
  <li>今の自分が分からない、できないこと</li>
</ol>

<!--
前提知識として自分が持っているものから今回やる範囲の必要な部分を洗い出す  
とは言ってもやったことないと何もわからない状態になるので、やりながら必要な部分だけ勉強していく感じになる
-->


---
layout: new-section
---

# 1.1 今の自分が分かる、できること

<ul class="text-left text-3xl relative z-20 flex-1">
  <li>TypeScript がわかる</li>
  <li>オブジェクト思考が分かる</li>
  <li>graphql が分かる</li>
  <li>query が何をするのか分かる</li>
  <li>mutation が何をするのか分かる</li>
  <li>バックエンドではNestJS を一瞬触ったことがある</li>
</ul>

---
layout: new-section
---

# 1.2 今の自分が分からない、できないこと

<ul class="text-left text-3xl relative z-20 flex-1">
  <li>db が分からない</li>
  <li>インフラが分からない</li>
  <li>バックエンドのデプロイが分からない</li>
  <li>docker が分からない</li>
  <li>セキュリティが分からない</li>
  <li>バックエンドの作り方が分からない</li>
</ul>

---
layout: new-section
---

# 2. 技術選定

<ul class="text-left text-3xl relative z-20 flex-1">
  <li>自分ができる技術を選定をする</li>
  <li>学ぶ範囲を広げすぎない</li>
</ul>

<!--
フロントでは技術選定をしているので、その感じでバックエンドも技術選定をする  
ポイントとしては何も分からない状態を勉強する場合は勉強する範囲が広すぎないほうが良い  
今回で言えばバックエンドの技術に Go や Rust を選択したいが、Go や Rust を選択した場合は言語仕様から勉強する必要があるので、とても大変  
そこで今回選択したのはバックエンドを TypeScript でかける NestJS である  
前提知識として、Node のエコシステムや TypeScript が書けるので言語という壁がなくなり今回一番勉強したいバックエンドに集中して勉強ができる
-->

---
layout: intro
---

# 選ばれたのはNestJSでした


---
layout: new-section
---

# 3. ゴールを明確にする

<ul class="text-left text-3xl relative z-20 flex-1">
  <li>1 週間後までに Query、Mutation ある程度自由に作成できるようになる(Must)</li>
  <li>JWT の認証ができるようになる(Want)</li>
</ul>

<!--
ゴールがないと方向性やモチベーションが定まらないので、必ずゴールを設定しよう
MustとWantがあればなおよし
-->

---
layout: new-section
---

# 4. 今回やらない範囲を決める

<ul class="text-left text-3xl relative z-20 flex-1">
  <li>勉強していると芋づる式に勉強しないといけない</li>
  <li>すべて勉強していると時間が無限に足りないので捨てる範囲を決める</li>
</ul>


<!--
一つ前のセクションで NestJS を選択したが、バックエンドには DB を使うので仮想で DB を作るかローカルの DB を使うかの選択が必要になってくる  
ローカルのでDBはよくわからないのでMySQLだけ動くdockerを用意する(ほぼコピペ)   
その他のデプロイ、開発、本番用の環境構築やセキュリティなども考慮する必要があるが、今回はバックエンドの構築が主題になるのでここは勉強しない範囲に設定する
-->

---
layout: new-section
---

# 今回やらないこと

<ul class="text-left text-3xl relative z-20 flex-1">
  <li>docker</li>
  <li>デプロイ</li>
  <li>セキュリティ</li>
</ul>


---
layout: new-section
---

# 5. 進め方を決める

<ul class="text-left text-3xl relative z-20 flex-1">
  <li>自分の得意な勉強の方法でいい</li>
  <li>いきなり公式を呼んでもいいけど概要を理解する必要がある</li>
  <li>今回だとハンズオンをしてその後自分で作ってみる</li>
</ul>


<!--
自分の勉強方法は辞書を呼んで単語を覚えてから必要な時に必要な単語を組み合わせて言葉を作る的な感じだが、基礎じゃない場合はそれだと覚えることが多すぎたり、バージョンによって書き方が違うので概要を理解するために一旦ハンズオンをやった後自分で考えたものを全部自分で調べながら実装するのが良さそう
全く分からない状態だと大海に放り出されたみたいな感じになるけど、まずは泳ぎ方を学ぼう
-->

---
layout: new-section
---

# 6. 手を動かす

<ul class="text-left text-3xl relative z-20 flex-1">
  <li>まずは動くものを作る</li>
  <li>経験上とりあえず動くものを作ったほうがいい</li>
  <li>細かい部分は後から</li>
</ul>

<!--
とりあえず何をやったらいいのかさっぱり分からないのでハンズオン系をやってみることにする。   
Nest公式は英語なので英語ができない人間にとってはつらいし、情報量が多すぎて理解できないので日本語のハンズオン系を探すことにす
-->

---
layout: text-image
media: 'https://user-images.githubusercontent.com/56404715/179198666-2b441e97-a7ff-46cd-b7aa-fbeb6a73052e.jpeg'
---
 
# 6.1 GraphQL スターターパックをやる
  Nestの事が書いてある部分(Chapter 04 ~ Chapter 08)あたりまでやった
- [実際に試したリポジトリ](https://github.com/hisho/nestjs-nextjs-blog)
- 🙆‍♂️NestJSで実際に動くものができた
  正直これだけでは到底理解できないので、環境構築やその他を適当なリポジトリで作りつつREADMEを書くことにする
- [構築手順を書いたREADME.md](https://github.com/hisho/nestjs-nextjs-blog/blob/main/backend/README.md)

---
layout: new-section
---

# 6.2 自分で開発環境を組んでみる

<ul class="text-left text-3xl relative z-20 flex-1">
  <li>動くものはできたが手順通りなので、自分で開発環境を作ってみる</li>
  <li>READMEを書きながらだと見返せるのでおすすめ</li>
  <li><a href="https://github.com/hisho/nestjs-nextjs-blog/blob/main/backend/README.md">構築手順を書いたREADME</a></li>
</ul>

<!--
READMEはまじで大事。
未来への自分や属人化を防ぐので実務ではなるべく書きたいね
gitには無いけどREADMEを書きながらもう一つ新しいNestのプロジェクトを作った
-->

---
layout: new-section
---

# 7. 自分で考える

<ul class="text-left text-3xl relative z-20 flex-1">
  <li>自分で考えてアプリを作ってみる</li>
  <li>簡単なものからやっていこう</li>
</ul>

<!--
ハンズオン系では指示に従っているだけでアプリができるので概要がつかめたら、自分で考えてアプリを作ってみることにする   
とりあえずTODOアプリ辺りが初心者にとって良さそうなので、TODOアプリを作ってみることにする
-->

---
layout: new-section
---

# 7.1 TODOアプリを作る

<ul class="text-left text-3xl relative z-20 flex-1">
  <li>前回のアプリから動く形を作成</li>
  <li>基本的なCRUDを実装(new)</li>
  <li>dto(バリデーション)の実装(new)</li>
  <li>prismaからentityの自動生成(new)</li>
  <li>e2eテスト(new)</li>
  <li><a href="https://github.com/hisho/nest-todo-api">実際に試したリポジトリ</a></li>
</ul>

<!--
TODOアプリは簡単ですが、自分で考えてすべて作らないといけないのでその辺がいい！！！   
基本的な環境構築は前回のREADME.mdを見ながら作成する   
普通にやっても面白くないので前回でやらなかった新しいことに挑戦する
-->

---
layout: intro
---

# 次は・・・

<!--
基本的なCRUDを含め<br />NestJSに対する解像度が上がってきたので<br />次は認証機能を実装してみる
-->

---
layout: new-section
---

# 7.2 認証機能の作成

<ul class="text-left text-3xl relative z-20 flex-1">
  <li>前回のアプリから動く形を作成</li>
  <li>JWTによる認証を実装(new)</li>
  <li>Auth Gradを実装(new)</li>
  <li><a href="https://github.com/hisho/nest-auth-playground">実際に試したリポジトリ</a></li>
</ul>

<!--
実際に動く認証機能を実装してみる   
認証機能は結構重たいので、前回のように認証以外に新しいことには挑戦しないようにする(環境構築はマニュアル)

これで一旦認証から基本的なCRUDまで自分で実装できるようになった   
まだまだ実装したことはあるが、これ以上は覚えきれないのでまた別の機会に挑戦する
-->

---
layout: intro
---

# まとめ


---
layout: new-section
---


<ul class="text-left text-3xl relative z-20 flex-1">
  <li>手順を立てて勉強しよう</li>
  <li>考えても分からないのでとりあえず動くまで手を動かしてみよう</li>
  <li>README.mdなどで自分がやったことを文書化するのは大事</li>
  <li>わからないことを勉強する時は何もわからいのでgithubで検索するとコードベースで会話ができるのでいいかも</li>
</ul>

---
layout: intro
---

# 結局


---
layout: intro
---

# 楽しもう

---
layout: intro
---

# おすすめの検索法

---
layout: intro
---

# GitHubで使っているパッケージを最新順にして検索する