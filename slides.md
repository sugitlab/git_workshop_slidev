---
theme: bricks # https://github.com/slidevjs/themes/tree/main/packages/theme-bricks
# background: https://source.unsplash.com/collection/94734566/1920x1080
class: "text-center"
highlighter: shiki
layout: intro
info: |
  ## Get along with Git

  Presented by [@sugitlab](https://twitter.com/sugitlab).
  Arranged by [@yuki82511988](https://twitter.com/yuki82511988).
---
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Kosugi+Maru&display=swap" rel="stylesheet">
<link href="./override.css" rel="stylesheet">

<!-- This slide uses following fonts.
font-family: 'Kosugi Maru', 'Sigmar One', 'Signika Negative', sans-serif; -->

# Get along with <span style="font-size:96px;">Git</span>

<div class="pt-12">
  <p @click="$slidev.nav.next" class="px-2 p-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Gitとなかよくなろう ...>
  </p>
</div>

---

# Who is Sugit?!

<div class="blend" style="display:flex" >
  <img style="vertical-align:middle" src="https://pbs.twimg.com/profile_images/1261278455842271232/4TQJWEPG_400x400.jpg" height="80" width="80" />
  <p> <a href="https://twitter.com/sugitlab">@sugitlab</a>: 自称フルペラットエンジニア </p>
</div>

<br>
<br>

- 🍵 **Kyoto** - 京都にある会社で研究寄りのエンジニアやってます
  - 化学 + 数学 + プログラミング がお仕事です
  - 最近は PdM なお仕事が多くて、あまりコードを書く機会がなく寂しいです🙄
- 🧑‍💻 **Flutter** - プライベートの時間は（最近は）大体 Flutter やってます
- 🗞 **[Zenn](https://zenn.dev/sugitlab)** - Flutter のことばかり書いている Zenn アカウントです
- 🚃 **[TechTrain](https://techbowl.co.jp/techtrain/mentors/116)** - 副業でU30向けのメンターやってます


---
layout: fact
---

# Thanks
<div style="
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 48px;">
  <span style="font-size: 48px; vertical-align:middle;">
  事前アンケートへのご協力 <br>
  ありがとうございました
  </span>
</div>

---

# Questionnaire Results

- "git-flow という運用パターンとそのPros, Cons" : 11
- "git のちょっと踏み込んだ使い方" : 10
- "git でやらかさないためにすること" : 10
- "そもそも VCS (Version Control System) のことについて知っていますか？" : 10
- "git が管理している .git フォルダの中身を見たことがありますか？" : 10
- "git におけるマージは2種類ある" : 9
- "GitHubのIssueでやってほしくないこと" : 9
- "OSS コントリビューションマナー" : 7

---

# Others

- "git やらかしと対処法" : 6
- "VSC と VCS Hosting Service のことについて知っていますか？" : 6
- "Git Client (GUI, TUI, CLI tool) のおすすめたち" : 5
- "ローカルとリモートをちゃんと理解する" : 5
- "GitHubにおける Markdown 文化とお作法" : 5
- "git の四方山話 (歴史など)" : 2
- "git の基本的な使い方" : 1

---
layout: section
---

# Outline

::right::

## 1. VCSって何?
## 2. .gitの中身
## 3. ちょっと踏み込んだ git
## 4. gitのマージは2種類
## 5. git-flow の Pros/Cons
## 6. gitでやらかさないためにすること
## 7. GitHubのIssueで気をつけること
## 8. OSSコントリビューションマナー

<style>
h2, h3, body {
  font-family: 'Kosugi Maru', 'Signika Negative', sans-serif
}
</style>

---
layout: statement
---
# ① VCSって何?

<style>
h1 {
  font-family: 'Kosugi Maru', 'Signika Negative', sans-serif
}
</style>

---

# What's <span style="font-size:48px;">VCS</span> ?

## Version Control System

電子的なファイルの変更履歴を残しておき、<br>
過去の状態に戻したり、変更内容を確認できるようにするソフトウェアの総称

<br>
<br>
<br>

- ソースコードを管理するためのものではなく<span style="color:red;">電子的な記録全て</span>が対象
- 音楽・写真・テキスト・書類全て

数ある VCS ソフトウェアのうちの１つがみんな大好き <span style="font-size:32px">Git</span> です

---

# "VCS" Software

<br>

Git以外にも有名なバージョン管理システムがいくつかあります。

いまでも選択肢に上がる現役バリバリなものは以下の通りです

## - Git
## - Subversion
## - Mercurial

---
layout: fact
---

# Why Git?

<br>
<span style="font-size:32px">
いろいろな選択肢があるのに <br><br>
どうしてみんな Git を使うんだろう??
</span>

---
layout: fact
---

# Git is Champion?

<br>

## 🙅 NO 🙅

---
layout: fact
---

# Git + GitHub is Champion !!

<br>

## 🙆‍♂️ YES 🙆‍♂️
### I'm not sure

---

# Git + GitHub is Champion

<br>

Git が流行る前は Subversion が最強でした

昭和からある企業ではまだ Subversion が現役のところもたくさんあります (弊社でも現役です)

そんな Subversion から VCS 王座を奪ったのは

<br>

<span style="font-size:42px">Git ではなく GitHub</span> です（と思っています）


---

# History

<br>

もともと Git は Linux 開発者の Linus Tovalds が

「俺の オープンソースプロジェクトを支える VCS が無い！！ （全部気に入らない）」

と言い出してサクサク作ったものです。（二週間で作ったという話です… 🙈）

<v-click>

そう、

<span style="font-size:42px;">オープンソースのために作った</span>

のです。

</v-click>

---
layout: items
cols: 2
---

# Why Git is good for OpenSource ?

::items::

<div>
  Subversion は 中央集中型 と呼ばれます。<br><br><br>
  <img src="/resources/centralized.png" width=200 />
</div>
<div>
  一方、Git は 分散型 と呼ばれます。<br><br><br>
  <img src="/resources/distributed.png" width=200 />
</div>

---

# Subversion

<br>

- リポジトリはサーバー側にのみ作ります
- クライアント側（実装者）は特定の<span style="color:red;">歴史の１ページのみ</span>を引き出します
- 変更の記録・履歴の閲覧など全ての操作はサーバーへの接続が必須です
- バカでかい歴史やバカでかい単一ファイルを扱うのは Subversion が得意です
  - Gitで動画を扱ったらすぐに死にます🧟‍♂️
- Subversionの歴史は絶対です

<div style="
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top:42px;
">
  <img src="/resources/centralized.png" width=200 />
</div>

---

# Git

<br>

- サーバー・クライアント関係なく、<span style="color:red;">すべての環境がリポジトリを持ちます</span>
- 変更の記録・履歴の閲覧など全ての操作はオフラインでもOKです
- 変更の共有（歴史の共有）をリポジトリの同期によって実現します
- 軽いファイルを扱うことを基本とします（GitHubはデフォルトで Max 50MB です）
- Gitの歴史は簡単に書き換えることができます（権限があれば）

<div style="
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top:42px;
">
  <img src="/resources/distributed.png" width=200 />
</div>

---

# Git v.s. Subversion

<br>
単純な特長だけを比較しても、甲乙つけがたい…。

<br>
<br>

でも、オープンソースなら？

みんなで作るのに、１箇所のサーバーに集中アクセスするの？

<span style="color:red;">
サーバー死んじゃう！！
</span>

---

# GitHub makes Git Champion

<br>

GitHubの登場によって、 **オープンソース** 活動が世の中に急速に拡大しました。

その結果、 「Git 最強じゃね？」 となったのです。

Git だけの力では「Git 良さそうだけど Subversion で別にいいわ」となっていたことでしょう。

---
layout: statement
---
# ② .git の中身を見てみよう

<style>
h1 {
  font-family: 'Kosugi Maru', 'Signika Negative', sans-serif
}
</style>

---

# DOING

あとで書く

---
layout: statement
---

# ③ ちょっと踏み込んだ git

<style>
h1 {
  font-family: 'Kosugi Maru', 'Signika Negative', sans-serif
}
</style>

---
layout: statement
---

# ④ gitのマージは2種類

<style>
h1 {
  font-family: 'Kosugi Maru', 'Signika Negative', sans-serif
}
</style>

---
layout: statement
---

# ⑤ git-flow の Pros/Cons

<style>
h1 {
  font-family: 'Kosugi Maru', 'Signika Negative', sans-serif
}
</style>

---
layout: statement
---

# ⑥ gitでやらかさないためにすること

<style>
h1 {
  font-family: 'Kosugi Maru', 'Signika Negative', sans-serif
}
</style>

---
layout: statement
---

# ⑦ GitHubのIssueで気をつけること

<style>
h1 {
  font-family: 'Kosugi Maru', 'Signika Negative', sans-serif;
}
</style>

---
layout: statement
---

# ⑧ OSSコントリビューションマナー

<style>
h1 {
  font-family: 'Kosugi Maru', 'Signika Negative', sans-serif
}
</style>

---
layout: statement
---

# THANKS