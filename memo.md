# Description

最近触った新しい技術の LP を書くにあたって考えたことを簡単にメモする

## 概要

- NestJS で graphql のバックエンドを構築したのを書く
- 勉強期間は期間 1 週間
- 仕事をやめたのでやる時間ができた

## なにをやったのか

今回の勉強でやった具体的なこと

- NestJS で graphql のバックエンドを構築した
- - Query 作成
- - Mutation 作成
- - JWT の Auth 作成
- - JWT の認証のガード実装

## なにをやらなかったのか

今回勉強するのにあたって本質ではないが必要な部分まで勉強していると時間が足りないため、あえてやらなかった

- 実際にデプロイ
- docker の詳しい使い方
- セキュリティ
- データベースの設計
- 詳細なエラーハンドリング
- test

## なぜやったのか

- 1 年間 React でフロントを書いたのでバックエンドも書きたい
- 当時やっていたプロジェクトでバックエンドができていなかったので自分が作ればいいと思った
- プログラミング経験でなんとなく何をすればいいのか処理はわかるので自分でかけそうだと思った
- フルスタックだと給与がいい 🤑
- 実務で rest の経験は無いので経験がある graphql の方が構築できそうだなと思った

## どのようにやったのか

- 前提知識から必要な知識を探す
- 今回のやる範囲を決める
- 今回やる期間を決める
- 今回やらない範囲を決める

## 流れ

勉強するにあたっての流れを書く

### 1.前提知識から情報を整理する

前提知識として自分が持っているものから今回やる範囲の必要な部分を洗い出す  
とは言ってもやったことないと何もわからない状態になるので、やりながら必要な部分だけ勉強していく感じになる

#### 分かる、できること

- TypeScript がわかる
- オブジェクト思考が分かる
- graphql が分かる
- query が何をするのか分かる
- mutation が何をするのか分かる
- NestJS を一瞬触ったことがある

#### 分からない、できないこと

- db が分からない
- インフラが分からない
- バックエンドのデプロイが分からない
- docker が分からない
- セキュリティが分からない
- バックエンドの作り方が分からない

### 2.技術選定

自分ができる技術選定をする  
フロントでは技術選定をしているので、その感じでバックエンドも技術選定をする  
ポイントとしては何も分からない状態を勉強する場合は勉強する範囲が広すぎないほうが良い  
今回で言えばバックエンドの技術に Go や Rust を選択したいが、Go や Rust を選択した場合は言語仕様から勉強する必要があるので、とても大変  
そこで今回選択したのはバックエンドを TypeScript でかける NestJS である  
前提知識として、Node のエコシステムや TypeScript が書けるので言語という壁がなくなり今回一番勉強したいバックエンドに集中して勉強ができる

### 3.ゴールを明確にする

- 1 週間後までに Query、Mutation ある程度自由に作成できるようになる(Must)
- JWT の認証ができるようになる(Want)

### 4.今回やらない範囲を決める(本来(実務)であれば必要だが今回の勉強では不要なものを決める)

一つ前のセクションで NestJS を選択したが、バックエンドには DB を使うので仮想で DB を作るかローカルの DB を使うかの選択が必要になってくる  
ローカルのでDBはよくわからないのでMySQLだけ動くdockerを用意する(ほぼコピペ)   
その他のデプロイ、開発、本番用の環境構築やセキュリティなども考慮する必要があるが、今回はバックエンドの構築が主題になるのでここは勉強しない範囲に設定する

### 5.進め方
自分の勉強方法は辞書を呼んで単語を覚えてから必要な時に必要な単語を組み合わせて言葉を作る的な感じだが、基礎じゃない場合はそれだと覚えることが多すぎたり、バージョンによって書き方が違うので概要を理解するために一旦ハンズオンをやった後自分で考えたものを全部自分で調べながら実装するのが良さそう

### 6.ハンズオン系をやってみる(手を動かす)
とりあえず何をやったらいいのかさっぱり分からないのでハンズオン系をやってみることにする。   
Nest公式は英語なので英語ができない人間にとってはつらいし、情報量が多すぎて理解できないので日本語のハンズオン系を探すことにす   

#### 6.1[GraphQL スターターパック | Prisma + NestJS + Next.JS 製 個人ブログサイトを Cloud Run で運用しよう](https://zenn.dev/waddy/books/graphql-nestjs-nextjs-bootcamp)をやる(概要を理解する)
とりあえず、Classmethodの方が書いているこの本を買ってやった
- [実際に試したリポジトリ](https://github.com/hisho/nestjs-nextjs-blog)   
Nestの事が書いてある部分(Chapter 04 ~ Chapter 08)あたりまでやった
- 🙆‍♂️postgresqlをmysqlに変更した
- 🙆‍♂️NestJSで実際に動くものができた
正直これだけでは到底理解できないので、環境構築やその他を適当なリポジトリで作りつつREADMEを書くことにする
- [構築手順を書いたREADME.md](https://github.com/hisho/nestjs-nextjs-blog/blob/main/backend/README.md)

### 7.自分でアプリを作ってみる(自分で考える)
ハンズオン系では指示に従っているだけでアプリができるので概要がつかめたら、自分で考えてアプリを作ってみることにする   
とりあえずTODOアプリ辺りが初心者にとって良さそうなので、TODOアプリを作ってみることにする

### 7.1TODOアプリを作る
- [実際に試したリポジトリ](https://github.com/hisho/nest-todo-api)
TODOアプリは簡単ですが、自分で考えてすべて作らないといけないのでその辺がいい！！！   
基本的な環境構築は前回のREADME.mdを見ながら作成する   
普通にやっても面白くないので前回でやらなかった新しいことに挑戦する
- 基本的なCRUDを実装
- dto(バリデーション)の実装
- prismaからentityの自動生成
- e2eテスト
これで基本的なCRUDを含めNestJSに対する解像度が上がってきたので次は認証機能を実装してみる

### 7.2認証機能の作成
- [実際に試したリポジトリ](https://github.com/hisho/nest-auth-playground)
実際に動く認証機能を実装してみる   
認証機能は結構重たいので、前回のように認証以外に新しいことには挑戦しないようにする(環境構築はマニュアル)
- JWTによる認証を実装
- Auth Gradを実装
これで一旦認証から基本的なCRUDまで自分で実装できるようになった   
まだまだ実装したことはあるが、これ以上は覚えきれないのでまた別の機会に挑戦する


## 勉強するのに使ったもの

Github で使っているパッケージの OOS をの最新のリポジトリを調べる

- https://github.com/search?o=desc&q=nestjs%2Fgraphql&s=updated&type=Repositories

### 参考文献

- https://docs.nestjs.com/
- https://qiita.com/marumaru0113/items/9bc72335439ed135b030
- https://qiita.com/naoki-haba/items/ed004a4235a660dd706a
- https://zenn.dev/waddy/books/graphql-nestjs-nextjs-bootcamp
- https://qiita.com/kikikikimorimori/items/5d1098f6a51324ddaab4
- https://qiita.com/TakedaTakumi/items/329c6798f984814d4ae1
- https://zenn.dev/uttk/articles/9095a28be1bf5d
- https://zenn.dev/mseto/articles/nest-graphql-prisma
- https://zenn.dev/nori_k/articles/2834ca2f339a71
- https://zenn.dev/mano_r/articles/8d25be4b4452dd
- https://github.com/unlight/prisma-nestjs-graphql#readme
- https://zenn.dev/tkcel/articles/d5b7ec71ceacf6
- https://zenn.dev/nori_k/articles/45399999ff39f2
- https://zenn.dev/hakushun/articles/7daac74ae9af25
- https://circleci.com/blog/testing-nestjs-graphql/
