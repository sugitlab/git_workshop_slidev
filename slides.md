---
title: git workshop
theme: light-icons # https://github.com/lightvue/slidev-theme-light-icons
image: "https://source.unsplash.com/collection/94734566/1920x1080"
layout: intro
info: |
  ## Get along with Git

  Presented by [@sugitlab](https://twitter.com/sugitlab). <br>
  Arranged by [@yuki82511988](https://twitter.com/yuki82511988).
---

<div class="mb-4 absolute bottom-4 left-12">
  <span class="text-6xl text-primary-lighter text-opacity-80" style="font-weight:500;" >
    Get Along With
  </span>
  <div class="text-9xl text-white text-opacity-60" style="font-weight:600;" >
    Git  <light-icon icon="git-branch"/>
  </div> 
</div>

---
layout: image-right
equal: false
---

<div class="text-5xl font-bold text-primary pb-4">Who is Sugit?!</div>


<div class="blend" style="display:flex" >
  <img style="vertical-align:middle" src="https://pbs.twimg.com/profile_images/1261278455842271232/4TQJWEPG_400x400.jpg" height="80" width="80" />
  <p> <a href="https://twitter.com/sugitlab">@sugitlab</a>: 自称フルペラットエンジニア </p>
</div>

<br>
<br>

- 🍵 **Kyoto** - 京都にある会社で研究寄りのエンジニアやってます
  - 化学 + 数学 + プログラミング がお仕事です
  - 最近は PdM なお仕事が多め (´・ω・｀)
- 🧑‍💻 **Flutter** - プライベートの時間は大体 Flutter やってます
- 🗞 **[Zenn](https://zenn.dev/sugitlab)** - Flutter のことばかり書いている Zenn アカウントです
- 🚃 **[TechTrain](https://techbowl.co.jp/techtrain/mentors/116)** - 副業で U30 向けのメンターやってます。
  - U30なら無料なので興味あればぜひ

<style>
.blend {
  display: grid;
  place-items: center;
}

.blend img {
  mix-blend-mode: multiply;
  max-width: 300px;
  height: auto;
}

ul {
  list-style-type: circle;
}
</style>

---
layout: image-right
---

<div class="text-5xl font-bold text-primary pb-4">Thanks <light-icon icon="color-picker" /> </div>

<div class="text-xl">
  事前アンケートへのご協力ありがとうございました
</div>

---
layout: center-image
---

<div class="text-5xl font-bold text-primary pb-4">Questionnaire Results</div>

- "git-flow という運用パターンとその Pros, Cons" : 11
- "git のちょっと踏み込んだ使い方" : 10
- "git でやらかさないためにすること" : 10
- "そもそも VCS (Version Control System) のことについて知っていますか？" : 10
- "git が管理している .git フォルダの中身を見たことがありますか？" : 10
- "git におけるマージは 2 種類ある" : 9
- "GitHub の Issue でやってほしくないこと" : 9
- "OSS コントリビューションマナー" : 7

<style>
ul {
  text-align: left;
  list-style-type: circle;
  font-size: 1.3rem;
}
</style>

---
layout: center-image
---

- "git やらかしと対処法" : 6
- "VSC と VCS Hosting Service のことについて知っていますか？" : 6
- "Git Client (GUI, TUI, CLI tool) のおすすめたち" : 5
- "ローカルとリモートをちゃんと理解する" : 5
- "GitHub における Markdown 文化とお作法" : 5
- "git の四方山話 (歴史など)" : 2
- "git の基本的な使い方" : 1

<style>
ul {
  text-align: left;
  list-style-type: circle;
  font-size: 1.3rem;
}
</style>

---
layout: center-image
---

<div class="text-3xl">早速ですが質問です</div>

---
layout: center-image
---

<div class="text-5xl">どうして Git を使っているのですか??</div>


---
layout: center-image
---

<div class="text-5xl">Git以外...選択肢あるの? 🤔</div>

<br>

<v-click>
  <div class="text-4xl">安心してください。Git でOKです 💁🏻‍♂️</div>
</v-click>

---
layout: center-image
---

<div class="text-3xl leading-relaxed">
  ソースコードを管理するなら<br>
  現時点での最善はGitだと思います <br><br>
  しかし、まだまだ Git ではない現場というのもあるのです… 
</div>

---
layout: center-image
---

<div class="text-3xl leading-relaxed">
  これに対して<br>
  「なんだ、時代遅れの会社か 🤷🏼‍♂️」<br>
  と言う人は、大体何もわかってない人です。<br>
  無視しましょう🙆‍♂️
</div>

---
layout: center-image
---

<div class="text-3xl leading-relaxed">
  どうして Git が使われているのか <br>
  Git以外の選択肢は何があるのか <br>
  余談ですが少〜しお付き合いください
</div>

---
layout: center-image
---

<div class="text-5xl font-bold text-primary pb-4">What's VCS</div>

<div class="text-3xl"> Version Control System </div>

<div class="rounded-2xl border-4 border-green-200 p-4 m-8">
  電子的なファイルの変更履歴を残しておき、<br>
  過去の状態に戻したり変更内容を確認できるようにするソフトウェアの総称
</div>

音楽・写真・テキスト・書類 など<span style="color:red;">電子的な記録全て</span>が対象

数ある VCS ソフトウェアのうちの１つがみんな大好き <span style="font-size:32px">Git</span> です

---
layout: center-image
---

<div class="text-2xl m-8">
Git 以外にも有名なバージョン管理システムがいくつかあります<br>
いまでも選択肢に上がる現役バリバリなものは以下の3つです
</div>

<div class="text-3xl font-bold text-primary pb-4">
Git / Subversion / Mercurial
</div>

といっても、Mercurial を使っている人をみたことがないので<br>

実質 Git vs Subversion です。

---
layout: center-image
image: 'https://i.gyazo.com/a6663519f17bc80a6af38dbc4e10a96c.jpg'
---

<div class="text-4xl text-primary font-bold m-4">
Google Trends
</div>

---
layout: center-image
---

<div class="text-2xl mb-8 leading-relaxed">
  ご覧の通り Git が流行る前は Subversion が最強でした🏋️‍♀️
</div>

<div class="text-2xl mb-8 leading-relaxed">
  まだ Subversion が現役の組織もたくさんあります (弊社でも現役です)<br>
</div>

<div class="text-2xl mb-8 leading-relaxed">
  では、なぜここまで Git が普及したのでしょう
</div>

---
layout: image-right
image: 'https://upload.wikimedia.org/wikipedia/commons/thumb/0/01/LinuxCon_Europe_Linus_Torvalds_03_%28cropped%29.jpg/440px-LinuxCon_Europe_Linus_Torvalds_03_%28cropped%29.jpg'
equal: false
---


<div class="text-2xl mb-8 leading-relaxed">
もともと Git は Linux 開発者の Linus Tovalds が

<br><br>
「オープンソースでLinux作りたいんだけど

　良いVCSないわ〜、作るわ〜」
<br><br>


と言い出してサクサク作ったものだそうです

（二週間で作ったという話です… 🙈）
</div>


<v-click>

<div class="text-3xl mb-8 leading-relaxed">
  そう、オープンソースのために作ったのです。
</div>

</v-click>

---
layout: center-image
---

<div class="text-4xl font-bold">
  どうしてオープンソースにはGitが良いの？
</div>

---
layout: image-left
image: 'https://i.gyazo.com/58bdb692e3d248913103fc25f04fbec7.jpg'
equal: false
---

<div class="text-3xl font-bold">
  Git は分散型だからです
</div>

---
layout: image-right
image: 'https://i.gyazo.com/1572c8c55c60bb28cad1a238864b1d70.jpg'
equal: false
---

<div class="text-3xl font-bold">
  Subversion は中央集中型です
</div>

---
layout: image-left
image: 'https://i.gyazo.com/8b356b1ffedb364f4bd0fa8dd9280daf.jpg'
---

<div class="text-4xl text-primary font-bold m-4">
Git
</div>

参加者全員がリポジトリをもちます

```shell
$ git clone ...
```

っていうアレです

---
layout: image-left
image: 'https://i.gyazo.com/f9a64a8692ba0996b6441c0a930ba94b.jpg'
---
<div class="text-4xl text-primary font-bold m-4">
Subversion
</div>

<br>

参加者はリポジトリをもちません

ファイルをもらって、変更して、登録します


---
layout: center-image
---

<div class="text-2xl font-bold">
オープンソースで Subversionを使うと<br><br>

みんなで１箇所のサーバーに集中アクセスすることになります<br><br>

ログを見るだけでもサーバーにアクセスです <br><br>

サーバー死んじゃう！！😨
</div>

---
layout: center-image
---

<div class="text-3xl font-bold leading-relaxed">
　じゃあ Git 最強やん
</div>

---
layout: center-image
---


<div class="text-5xl font-bold pb-4 mb-8">
  Git is Champion?
</div>

<div class="text-5xl font-bold pb-4">
  🙅 NO 🙅
</div>

---
layout: center-image
---


<div class="text-5xl font-bold pb-4 mb-8">
  ”Git + GitHub” is Champion!!
</div>

<div class="text-5xl font-bold pb-4">
  🙆‍♂️ YES 🙆‍♂️
</div>

<br><br>
知らんけど 🤪


---
layout: center-image
---

<div class="text-5xl font-bold text-primary pb-4 mb-8">
  GitHub <light-icon icon="brand-github" /> makes Git <light-icon icon="git-merge" />  Champion
</div>


<div class="text-xl">
GitHub の登場によってオープンソース活動が世の中に急速に拡大しました。

その結果「Git 最強じゃね？」となったのです。
</div>

---
layout: center-image
image: 'https://i.gyazo.com/a6663519f17bc80a6af38dbc4e10a96c.jpg'
---

<div class="text-2xl mb-8">
GitHubのサービススタートが2010年です

Gitの大逆転が始まっていますね
</div>

---
layout: center-image
---

<div class="text-3xl font-bold">長くなりましたが四方山話はこれでおしまいです</div>

---
layout: center-image
---

<div class="text-3xl font-bold">実用的な話をしましょう</div>

---
layout: center-image
---

<div class="text-3xl font-bold">実用的な話をしましょう</div>

---
layout: center-image
---

<div class="text-2xl">
  適当なフォルダで git log とたたくと
</div>

```shell
fatal: not a git repository (or any of the parent directories): .git
```
<div class="text-2xl">
  と怒られます
</div>

---
layout: center-image
---
<div class="text-5xl">
  not a git repository 
</div>

---
layout: center-image
---
<div class="text-4xl">
  gitリポジトリって何か説明できますか?
</div>


---
layout: center-image
---
<div class="text-4xl">
  git commit って何か分かりますか?
</div>

---
layout: center-image
---
<div class="text-4xl">
  分からなくなってきませんか? 😵‍💫
</div>

---
layout: center-image
---
<div class="text-4xl">
  実際 分からなくてもコードはかけます 🤫
</div>


---
layout: center-image
---
<div class="text-4xl mb-8">
  Gitの仕組みがわかると...🤔
</div>

<v-click>
  <div class="text-4xl">
    Gitの操作に自信が出る 😎
  </div>
</v-click>

---
layout: center-image
---

<div class="text-4xl font-bold text-primary mb-8">
.git の中身を見てみよう
</div>

.git ?? 🤔

---
layout: center-image
image: 'https://gyazo.com/239107de6b5d59a372531fc380c080d2.png'
---

<div class="text-3xl font-bold mb-8">
Gitリポジトリであるかどうか...
</div>
<div class="text-3xl font-bold mb-8">
それは .git があるかどうかです!
</div>

---
layout: center-image
---

<div class="text-2xl">
.git は Git リポジトリの情報をすべて保持している隠しフォルダです
</div>

---
layout: image-right
---

<div class="text-5xl text-primary font-bold mb-8">
  Unpack the .git
</div>

<br>

`git init` から見ていきましょう

---
layout: center-image
---

```shell
~/.git $ tree -L 1
├── HEAD
├── config
├── description
├── hooks
├── info
├── objects
└── refs
8 directories, 17 files
```
<div class="text-xl">
git init で作った git リポジトリです

さっそく README.md をつくってコミットしてみましょう
</div>


---
layout: center-image
---

```shell {all|4}
~/gitdir $ echo test > README.md  <-- README.mdを作って
~/gitdir $ git add README.md  <-- ステージングにして
~/gitdir $ git commit -m "initialize repository"  <-- コミット
[main (root-commit) d041e09] initialize repository
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
```

<v-click>
  <div class="text-2xl">
  最初のコミットができましたね
  </div>
</v-click>

---
layout: center-image
---

```shell {all}
~/.git $ tree
// ~~~省略~~~
├── logs
│   ├── HEAD
│   └── refs
│       └── heads
│           └── main
├── objects
│   ├── 9d
│   │   └── aeafb9864cf43055ae93beb0afd6c7d144bfa4
│   ├── c1
│   │   └── 2d7c0ed49ad9c7aa938743ba6fdee54b6b7fe1
│   ├── d0
│   │   └── 41e090b548f4ab7c11848384f9e171e728fc3d
│   ├── info
│   └── pack
└── refs
    ├── heads
    │   └── main
    └── tags
```

<div class="text-2xl">
  .gitにいろいろ増えました
</div>

---
layout: image-right
---

<div class="text-xl text-primary">
  Commit
</div>

```shell {all|1}
[main (root-commit) d041e09] initialize repository
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
```

<div class="text-xl text-primary">
  .git/objects
</div>

```shell {all|6-7}
├── objects
│   ├── 9d
│   │   └── aeafb9864cf43055ae93beb0afd6c7d144bfa4
│   ├── c1
│   │   └── 2d7c0ed49ad9c7aa938743ba6fdee54b6b7fe1
│   ├── d0
│   │   └── 41e090b548f4ab7c11848384f9e171e728fc3d
│   ├── info
│   └── pack
```

<v-click>
  <div class="text-xl">
    おや、一致した ID が見つかりましたね
  </div>
</v-click>

---
layout: center-image
---

<div class="text-3xl">
  解析してみましょう 🥳
</div>

```shell
├── d0
    └── 41e090b548f4ab7c11848384f9e171e728fc3d
```

---
layout: center-image
---

<div class="text-2xl mb-4">
  git cat-file で解析できます
</div>

```shell {all|2}
$ git cat-file -p d041 <-- 最初4文字くらいでOK
tree c12d7c0ed49ad9c7aa938743ba6fdee54b6b7fe1
author SuGit <sgmt.snj@gmail.com> 1626708424 +0900
committer SuGit <sgmt.snj@gmail.com> 1626708424 +0900
```

<v-click>

```shell {4-5}
├── objects
│   ├── 9d
│   │   └── aeafb9864cf43055ae93beb0afd6c7d144bfa4
│   ├── c1
│   │   └── 2d7c0ed49ad9c7aa938743ba6fdee54b6b7fe1
│   ├── d0
│   │   └── 41e090b548f4ab7c11848384f9e171e728fc3d
│   ├── info
│   └── pack
```

こちらも .git/object に同じIDのものがありますね。

</v-click>

---
layout: center-image
---

<div class="text-2xl mb-4">
  これも cat-file しましょう
</div>

```shell {all|2}
$ git cat-file -p c12d
100644 blob 9daeafb9864cf43055ae93beb0afd6c7d144bfa4    README.md
```

<v-click>

```shell {2-3}
├── objects
│   ├── 9d
│   │   └── aeafb9864cf43055ae93beb0afd6c7d144bfa4
│   ├── c1
│   │   └── 2d7c0ed49ad9c7aa938743ba6fdee54b6b7fe1
│   ├── d0
│   │   └── 41e090b548f4ab7c11848384f9e171e728fc3d
│   ├── info
│   └── pack
```

ほう...　次は君ですね

</v-click>

---
layout: center-image
---

<div class="text-2xl mb-4">
  これも cat-file しましょう
</div>

```shell
$ git cat-file -p 9dae
test
```

<br><br>
<div class="text-2xl">
  これは・・・、README.md の中身だ!!
</div>

---
layout: center-image
---

<div class="text-2xl mb-4">
  まとめると
</div>

```shell
├── 9d
│   └── aeafb9864cf43055ae93beb0afd6c7d144bfa4
├── c1
│   └── 2d7c0ed49ad9c7aa938743ba6fdee54b6b7fe1
├── d0
│   └── 41e090b548f4ab7c11848384f9e171e728fc3d
```

```shell
$ git cat-file -p 9dae
test
$ git cat-file -p c12d
100644 blob 9daeafb9864cf43055ae93beb0afd6c7d144bfa4    README.md
$ git cat-file -p d041
tree c12d7c0ed49ad9c7aa938743ba6fdee54b6b7fe1
author SuGit <sgmt.snj@gmail.com> 1626708424 +0900
committer SuGit <sgmt.snj@gmail.com> 1626708424 +0900
```

<div class="text-2xl mb-4">
  3種類の情報が記録されている、と言うことのようですね。
</div>

---
layout: center-image
---


<div class="text-3xl font-bold text-primary mb-4">
  type: commit
</div>

<div class="text-xl rounded-2xl border-4 border-green-200 p-4 m-8 text-left">
  <div class="text-xl font-bold">$ git cat-file -p d041</div>
  tree <span class="text-red-500">c12d</span>7c0ed49ad9c7aa938743ba6fdee54b6b7fe1<br>
  <div class="text-sm">// c12d のツリーにコミットをつんだよ</div>
  <span class="text-green-500">author</span> SuGit &lt;sgmt.snj@gmail.com&gt; 1626708424 +0900<br>
   <div class="text-sm">// コミットの著者は SuGit だよ</div>
   <div class="text-sm">// 時刻は 1626708424 +0900 = 2021/7/20 00:27:04 だよ (UNIX時間)</div>
  <span class="text-green-500">committer</span> SuGit &lt;sgmt.snj@gmail.com&gt; 1626708424 +0900
   <div class="text-sm">// コミッターは... 以下同文</div>
</div>

---
layout: center-image
---


<div class="text-3xl font-bold text-primary mb-4">
  type: tree
</div>

<div class="text-xl rounded-2xl border-4 border-green-200 p-4 m-8 text-left">
  <div class="text-xl font-bold">$ git cat-file -p c12d</div>
  100644 blob <span class="text-red-500">9dae</span>afb9864cf43055ae93beb0afd6c7d144bfa4    README.md
  <div class="text-sm">// README.md を圧縮して 9dae に保存したよ</div>
</div>

---
layout: center-image
---


<div class="text-3xl font-bold text-primary mb-4">
  type: blob
</div>

<div class="text-xl rounded-2xl border-4 border-green-200 p-4 m-8 text-left">
  <div class="text-xl font-bold">$ git cat-file -p 9dae</div>
  <span class="text-red-500">test</span>
  <div class="text-sm">// README.md の中身だよ</div>
</div>

---
layout: center-image
---

<div class="text-3xl font-bold text-primary mb-4">
  つまり
</div>

- commit: コミットの情報
- tree: コミット履歴の情報
- blob: ファイルのバックアップ

<br><br>
が、特定のコミットに対して記録されていると言うことがわかりました。
<style>
ul {
  text-align: left;
  list-style-type: circle;
  font-size: 1.3rem;
}
</style>


---
layout: center-image
---

<div class="text-xl font-bold mb-4">
  次はログをみましょう
</div>

```shell {4-7}
~/.git $ tree
// ~~~省略~~~
├── logs
│   ├── HEAD
│   └── refs
│       └── heads
│           └── main
├── objects
│   ├── 9d
│   │   └── aeafb9864cf43055ae93beb0afd6c7d144bfa4
│   ├── c1
│   │   └── 2d7c0ed49ad9c7aa938743ba6fdee54b6b7fe1
│   ├── d0
│   │   └── 41e090b548f4ab7c11848384f9e171e728fc3d
│   ├── info
│   └── pack
└── refs
    ├── heads
    │   └── main
    └── tags
```

---
layout: center-image
---

<div class="text-2xl font-bold mb-4">
log が1つでは寂しいので、コミットをもう一度追加しておきましょう
</div>

📄 README.md

```md
- test
+ # Abs.
+  This repository is just for testing the git behaviour
```

<v-click>

せっせとコミット

```shell
~/gitdir $ git add README.md
~/gitdir $ git commit -m "update README.md"
[main dd96c8f] update README.md
1 file changed, 3 insertions(+), 1 deletion(-)
```

</v-click>

---
layout: center-image
---

```shell {all|2-6}
~/gitdir$ git log
commit dd96c8f8bbcff86922b3db1f94aa38c4c6f3d633 (HEAD -> main)
Author: Sugit <sgmt.snj@gmail.com>
Date:   Tue Jul 20 01:09:32 2021 +0900

    update README.md

commit d041e090b548f4ab7c11848384f9e171e728fc3d
Author: SuGit <sgmt.snj@gmail.com>
Date:   Tue Jul 20 00:27:04 2021 +0900

    initialize repository
```

<div class="text-xl font-bold mb-4">
新しいコミットが増えました
</div>
 
---
layout: center-image
---

<div class="text-xl font-bold mb-4">
このときのログファイルは...
</div>

```shell {all|8-12}
~/.git/logs $ tree
├── HEAD
└── refs
    └── heads
        └── main

~/.git/logs $ cat HEAD
0000000000000000000000000000000000000000
d041e090b548f4ab7c11848384f9e171e728fc3d
SuGit <sgmt.snj@gmail.com> 1626708424 +0900
commit (initial): initialize repository

d041e090b548f4ab7c11848384f9e171e728fc3d
dd96c8f8bbcff86922b3db1f94aa38c4c6f3d633
Sugit <sgmt.snj@gmail.com> 1626710972 +0900
commit: update README.md
```

---
layout: center-image
---

<div class="text-xl font-bold mb-4">
分解すると
</div>

```shell
0000000000000000000000000000000000000000 ## <- 1つ前のコミットハッシュ
d041e090b548f4ab7c11848384f9e171e728fc3d ## <- 自身のコミットハッシュ
SuGit <sgmt.snj@gmail.com> 1626708424 +0900 ## <- コミット情報
commit (initial): initialize repository with ## <- メッセージ
```

---
layout: center-image
---

<div class="text-5xl text-primary font-bold mb-4">
1つ前のコミットハッシュ
</div>

---
layout: center-image
---

```mermaid
graph LR
  c01((0000))
  c02((d041))
  style c01 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
  c01 --> c02
```

```shell
0000000000000000000000000000000000000000 ## <- 1つ前のコミットハッシュ
d041e090b548f4ab7c11848384f9e171e728fc3d ## <- 自身のコミットハッシュ
SuGit <sgmt.snj@gmail.com> 1626708424 +0900 ## <- コミット情報
commit (initial): initialize repository  ## <- メッセージ
```

```mermaid
graph LR
  c02((d041))
  c03((dd96))
  style c02 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
  c02 --> c03
```

```shell
d041e090b548f4ab7c11848384f9e171e728fc3d
dd96c8f8bbcff86922b3db1f94aa38c4c6f3d633
Sugit <sgmt.snj@gmail.com> 1626710972 +0900
commit: update README.md
```

---
layout: center-image
---

<div class="text-2xl font-bold mb-8">
  コミットは「自身のハッシュ値」と「ひとつ前のハッシュ値」を持ちます
</div>

<div class="text-2xl font-bold mb-4">
git graph はこの連結によって作られます
</div>

```mermaid
graph LR
  c01((0000))
  c02((d041))
  c03((dd96))
  c04((........))
  style c01 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
  c01 --> c02 --> c03
  c03 --> c04
```

---
layout: center-image
---

<div class="text-3xl font-bold mb-4">
これを踏まえて、いろいろなコマンドをみていきましょう
</div>

---
layout: center-image
---

<div class="text-3xl text-primary font-bold mb-4">
git branch test
</div>

<div class="text-xl">
test ブランチの作成<br>
実態は・・・
</div>

---
layout: center-image
---

<div class="text-3xl text-primary font-bold mb-4">
コミットハッシュに名前をつけて保存しただけ
</div>

<div class="text-xl rounded-2xl border-4 border-green-200 p-4 m-8 text-left">
~/.git/refs/heads $ cat test <br>
dd96c8f8bbcff86922b3db1f94aa38c4c6f3d633
</div>

```mermaid
graph LR
  c01((0000))
  c02((d041))
  c03((dd96))
  c04((........))
  style c01 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
  c01 --> c02 --> c03
  c03 --> c04
```

<arrow x1="480" y1="430" x2="450" y2="390" color="#99f" width="2" arrowSize="1" />
test

---
layout: center-image
---

<div class="text-3xl text-primary font-bold mb-4">
git commit --amend -m "hogehoge"
</div>

<div class="text-xl">
コミットの修正は...
</div>


---
layout: center-image
---

<div class="text-3xl text-primary font-bold mb-4">
  単に log を書き換えているだけ
</div>

```shell {3-4}
0000000000000000000000000000000000000000 ## <- 1つ前のコミットハッシュ
d041e090b548f4ab7c11848384f9e171e728fc3d ## <- 自身のコミットハッシュ
SuGit <sgmt.snj@gmail.com> 1626708424 +0900 <-- ここを書き換える
commit (initial): initialize repository <-- ここを書き換える
```

---
layout: center-image
---

<div class="text-3xl text-primary font-bold mb-4">
git merge test
</div>

test ブランチのマージは...?

<br><br>

<v-click>
  2パターンに分かれます
</v-click>

---
layout: center-image
---

<div class="text-lg m-8">
それぞれが独自に進化している場合
</div>

main
<arrow x1="520" y1="220" x2="630" y2="260" color="#f99" width="2" arrowSize="1" />
```mermaid
graph LR
  c01((0000))
  c02((d041))
  c03((dd96))
  c04((9437))
  c05((a79b))
  style c01 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
  c01 --> c02 --> c03 --> c04
  c03 --> c05
```
test
<arrow x1="520" y1="420" x2="630" y2="380" color="#99f" width="2" arrowSize="1" />

---
layout: center-image
---

<div class="text-lg m-8">
マージコミットが増えて main の位置が変わります
</div>

main
<arrow x1="520" y1="220" x2="700" y2="300" color="#f99" width="2" arrowSize="1" />
```mermaid
graph LR
  c01((0000))
  c02((d041))
  c03((dd96))
  c04((9437))
  c05((a79b))
  c06((88a0))
  style c01 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
  c01 --> c02 --> c03 --> c04
  c03 --> c05
  c04 --> c06
  c05 --> c06
```
test
<arrow x1="520" y1="420" x2="580" y2="390" color="#99f" width="2" arrowSize="1" />

---
layout: center-image
---

<div class="text-lg m-8">
testだけが進化している場合
</div>

main
<arrow x1="480" y1="280" x2="520" y2="300" color="#f99" width="2" arrowSize="1" />
```mermaid
graph LR
  c01((0000))
  c02((d041))
  c03((dd96))
  c05((a79b))
  style c01 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
  c01 --> c02 --> c03
  c03 --> c05
```
test
<arrow x1="510" y1="370" x2="630" y2="340" color="#99f" width="2" arrowSize="1" />
---
layout: center-image
---

<div class="text-lg m-8">
git merge しても mainの位置が変わるだけです
</div>

main
<arrow x1="520" y1="270" x2="600" y2="300" color="#f99" width="2" arrowSize="1" />
```mermaid
graph LR
  c01((0000))
  c02((d041))
  c03((dd96))
  c05((a79b))
  style c01 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
  c01 --> c02 --> c03 --> c05
```
test
<arrow x1="510" y1="370" x2="600" y2="350" color="#99f" width="2" arrowSize="1" />


---
layout: center-image
---

<div class="text-3xl text-primary font-bold m-8">
Git のマージが 2 種類ありますね
</div>

アンケートの内容をやっと回収 🤫

---
layout: center-image
---

<div class="text-2xl text-primary font-bold m-8">
  ① マージコミットが作られる git merge
</div>

<div class="text-2xl text-primary font-bold m-8">
  ② main の位置だけズラす git merge
</div>

---
layout: center-image
---

<div class="text-3xl font-bold m-8">
  どっちが良いんだろう🤨 ??
</div>

---
layout: center-image
---

<div class="text-3xl font-bold m-8">
  ケースバイケース 🤓
</div>

<v-click>

ですが、
<div class="text-3xl font-bold m-8">
  どちらかと言えば ① の方が良い
</div>

</v-click>

---
layout: center-image
---

<div class="text-3xl text-primary font-bold m-8">
  ① non-first-forward
</div>
<div class="text-3xl text-primary font-bold m-8">
  ② first-forward
</div>

といいます

---
layout: center-image
---

<div class="text-3xl font-bold m-8">
  何が違うの？
</div>

---
layout: center-image
---

<div class="text-3xl text-primary font-bold m-8">
  ① non-first-forward
</div>

```mermaid
graph LR
  c01((0000))
  c02((d041))
  c03((dd96))
  c04((9437))
  c05((a79b))
  c06((88a0))
  style c01 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
  c01 --> c02 --> c03 --> c04
  c03 --> c05
  c04 --> c06
  c05 --> c06
```

<div class="text-3xl text-primary font-bold m-8">
  ② first-forward
</div>

```mermaid
graph LR
  c01((0000))
  c02((d041))
  c03((dd96))
  c05((a79b))
  style c01 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
  c01 --> c02 --> c03 --> c05
```

---
layout: center-image
---

<div class="text-3xl text-primary font-bold m-8">
  ① non-first-forward
</div>

```mermaid
graph LR
  c01((0000))
  c02((d041))
  c03((dd96))
  c04((9437))
  c05((a79b))
  c06((88a0))
  style c01 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
  style c05 fill:#afa,stroke:#dfd,stroke-width:1px
  style c06 fill:#afa,stroke:#dfd,stroke-width:1px
  c01 --> c02 --> c03 --> c04
  c03 --> c05
  c04 --> c06
  c05 --> c06
```

<div class="text-3xl text-primary font-bold m-8">
  ② first-forward
</div>

```mermaid
graph LR
  c01((0000))
  c02((d041))
  c03((dd96))
  c04((a79b))
  style c01 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
  c01 --> c02 --> c03 --> c04
```

---
layout: center-image
---

<div class="text-3xl font-bold m-8">
  マージコミットが無い = マージしたぞという "歴史が無い"
</div>

<div class="text-2xl font-bold m-8">
  歴史は大事にしようぜ 😎
</div>


---
layout: center-image
---

<div class="text-4xl font-bold m-8">
  ② は ① にできる 🤗
</div>

---
layout: center-image
---

<div class="text-3xl font-bold m-8">
  --no-ff オプション
</div>

```shell
$ git merge branch-name --no-ff
```

<div class="text-lg m-8">
  これで強制的にマージコミットを積むことができます
</div>

---
layout: center-image
---

<div class="text-3xl font-bold m-8">
  マージコミットは残しておいた方がベターです
</div>

<v-click>

<div class="text-2xl m-8">
  <img style="margin: auto" src="https://pbs.twimg.com/profile_images/1070038810111565824/1omCvDAZ.jpg" />
  それってあなたの感想ですよね？
</div>

</v-click>

---
layout: center-image
---

<div class="text-3xl font-bold m-8">
  はい、残念ながら私の感想です 😥
</div>

---
layout: center-image
---

<div class="text-2xl font-bold m-8">
  残念ですが、世の中には一定数いるのです。
</div>

<div class="text-2xl font-bold m-8">
　正しい歴史 &lt;&lt; 美しいコミットグラフ 派が... 😰
</div>

---
layout: center-image
---

<div class="text-3xl font-bold m-4">
  コミットグラフの美しさを意識するのは<br>
  OSSにPRを出すときだけで良い!!
</div>
<div class="text-2xl font-bold m-4">
  派です
</div>

OSSコントリビューションのお作法については後ほど 🙌

---
layout: center-image
---

<div class="text-3xl text-primary font-bold mb-4">
	git reset
</div>

こいつは歴史を書き換える危険なコマンドです ☠️

---
layout: center-image
---

<div class="text-2xl font-bold mb-4">
  👽👽ローカルのコミットを取り消すくらいならOKです👽👽
</div>

<v-click>

<div class="text-3xl font-bold mb-4">
  OKじゃない！！<br>
  めっちゃ注意して！！
</div>

</v-click>

---
layout: center-image
---

<div class="text-2xl font-bold mb-4">
git reset は "まだリモートに入れていない" <br> ローカルのコミットに対してだけ安全です
</div>

コミットはハッシュの連鎖でしたね。

push済みのコミットに対して git reset をするということは、

リモートで既に構築された **コミットの連鎖を破壊する** ってことですね。

---
layout: center-image
---

<div class="text-2xl font-bold">
  あ、"dd96" のコミット、ミスってるわ〜
</div>
<div class="text-2xl font-bold mb-8">
  git reset しよ
</div>

<div class="text-xl text-primary font-bold">
  REMOTE
</div>
```mermaid
graph LR
  c01((0000))
  c02((d041))
  c03((dd96))
  style c01 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
  c01 --> c02 --> c03
```

<div class="text-xl text-primary font-bold mt-8">
  LOCAL
</div>
```mermaid
graph LR
  c01((0000))
  c02((d041))
  c03((dd96))
  c04[staging]
  style c01 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
  c01 --> c02 --> c03 --> c04
```

---
layout: center-image
---

<div class="text-2xl font-bold mb-8">
  git reset したったぜ
</div>

<div class="text-xl text-primary font-bold">
  REMOTE
</div>
```mermaid
graph LR
  d01((0000))
  d02((d041))
  d03((dd96))
  style d01 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
  d01 --> d02 --> d03
```

<div class="text-xl text-primary font-bold mt-8">
  LOCAL
</div>
```mermaid
graph LR
  c01((0000))
  c02((d041))
  c03[staging]
  style c01 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
  c01 --> c02 --> c03
```

---
layout: center-image
---

<div class="text-2xl font-bold mb-8">
  新しい変更をコミットだ!!
</div>

<div class="text-xl text-primary font-bold">
  REMOTE
</div>
```mermaid
graph LR
  e01((0000))
  e02((d041))
  e03((dd96))
  style e01 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
  e01 --> e02 --> e03
```

<div class="text-xl text-primary font-bold mt-8">
  LOCAL
</div>
```mermaid
graph LR
  f01((0000))
  f02((d041))
  f03((e292))
  style f01 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
  style f03 fill:#dfd,stroke:#333,stroke-width:1px
  f01 --> f02 --> f03
```

---
layout: center-image
---

<div class="text-2xl font-bold mb-8">
  リモートにプッシュだ.... あれ?!
</div>

<div class="text-xl text-primary font-bold">
  REMOTE
</div>
```mermaid
graph LR
  c01((0000))
  c02((d041))
  c03((dd96))
  style c01 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
  c01 --> c02 --> c03
```

<div class="text-xl text-primary font-bold mt-8">
  LOCAL
</div>
```mermaid
graph LR
  d01((0000))
  d02((d041))
  d03((e292))
  style d01 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
  style d03 fill:#dfd,stroke:#333,stroke-width:1px
  d01 --> d02 --> d03
```

---
layout: center-image
---

<div class="text-2xl font-bold mb-8">
  コミット = 自身のハッシュ + 直前のハッシュ
</div>

```mermaid
graph LR
  d01((d041))
  d03((e292))
  style d01 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
  style d03 fill:#dfd,stroke:#333,stroke-width:1px
  d01 --> d03
```

---
layout: center-image
---

<div class="text-2xl font-bold m-4">
  ハッシュでつなぐと…
</div>

<div class="text-xl text-primary font-bold">
  REMOTE
</div>
```mermaid
graph LR
  c01((0000))
  c02((d041))
  c03((dd96))
  style c01 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
  c01 --> c02 --> c03
```

<div class="text-xl text-primary font-bold">
  COMMIT
</div>
```mermaid
graph LR
  d01((d041))
  d03((e292))
  style d01 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
  style d03 fill:#dfd,stroke:#333,stroke-width:1px
  d01 --> d03
```

---
layout: center-image
---

<div class="text-2xl font-bold m-4">
  mainブランチが2つに分離してしまう… = push error
</div>

<div class="text-xl text-primary font-bold">
  REMOTE
</div>

```mermaid
graph LR
  c01((0000))
  c02((d041))
  c03((dd96))
  d03((e292))
  style c01 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
  style d03 fill:#dfd,stroke:#333,stroke-width:1px
  c01 --> c02 --> c03
  c02 --> d03
```

---
layout: center-image
---

<div class="text-2xl font-bold m-4">
  「push errro 対応」 ググる
</div>
<br>
<div class="text-2xl font-bold m-4">
  git push -f でできるんだって!!
</div>

<v-click>
  <div class="text-2xl font-bold m-4">
    ↑ 犯罪です
  </div>
</v-click>

---
layout: center-image
---

<div class="text-3xl font-bold mb-4">
git reset は明らかに push してないことを事前に確認
</div>

<div class="text-2xl font-bold mb-4">
よくわからないなら使わない！
</div>

---
layout: center-image
---

<div class="text-3xl text-primary font-bold md-4">
	git cherry-pick
</div>

つまみ食いコマンド

---
layout: center-image
---

<div class="text-xl text-primary font-bold">
  BRANCH-A
</div>
```mermaid
graph LR
  c01((a901))
  c02((d041))
  c03((dd96))
  style c03 fill:#dfd,stroke:#333,stroke-width:1px
  c01 --> c02 --> c03
```

<div class="text-xl text-primary font-bold">
  BRANCH-B
</div>
```mermaid
graph LR
  d01((a901))
  d02((d041))
  d03((e292))
  d04((41d2))
  style d03 fill:#aef,stroke:#333,stroke-width:1px
  style d04 fill:#aef,stroke:#333,stroke-width:1px
  d01 --> d02 --> d03 --> d04
```

<div class="text-xl font-bold m-8">
  A に B から e292 だけ取り込みたい
</div>

---
layout: center-image
---

<div class="text-xl font-bold m-8">
  git cherry-pick e292...
</div>

<div class="text-xl">
  cherry-pick は 競合しやすいので、我慢して手作業で修正しましょう。
</div>

---
layout: center-image
---

別のブランチで作業したコミットにおける **変更**を 

<span class="text-2xl font-bold">
"別のコミットとして"
</span>
取り込みます。

<v-click>

```mermaid
graph LR
  d03((e292))
  d04{{patch}}
  style d03 fill:#aef,stroke:#333,stroke-width:1px
  style d04 fill:#aef,stroke:#333,stroke-width:1px
  d03 -- パッチを作る --> d04
```

</v-click>

<v-click>

<div class="text-xl text-primary font-bold">
  BRANCH-A
</div>
```mermaid
graph LR
  c01((a901))
  c02((d041))
  c03((dd96))
  c04((ae22))
  style c03 fill:#dfd,stroke:#333,stroke-width:1px
  style c04 fill:#aef,stroke:#333,stroke-width:1px
  c01 --> c02 --> c03 -- パッチからコミットを作る --> c04
```
</v-click>

---
layout: center-image
---

<br><br>
<div class="text-2xl font-bold">
コミットハッシュが異なるところがポイントです
</div>
<div class="text-2xl font-bold">
e292 != ae22
</div>

<br><br>

<v-click>
  <div class="text-2xl font-bold">
    もしハッシュが一緒だったら??<br>
    何がやばいか考えてみてください 🤔
  </div>
</v-click>

---
layout: center-image
---

<div class="text-xl font-bold">

このコマンドは歴史を書き換えないので安心です
<br>
<br>
リリースコントロールのために使ったり
<br>
<br>
別ブランチで誰かがやった神対応が欲しかったり
<br>
<br>

そんなときにつかいます
</div>

---
layout: center-image
---

<div class="text-3xl text-primary font-bold md-4">
	git stash
</div>

これはめっちゃ使います。

---
layout: center-image
---

新機能の作業用ブランチで作業中...
<br><br>

<div class="text-xl font-bold">
🥸「急で悪いけど、このバグ直して欲しいんや」
</div>

<br>
とか言われた時に
<br><br>

<div class="text-xl font-bold">
🥺「うぅぅぅ・・・まだコミットしたくないんだよなぁ・・」
</div>

<br>ということがあります。

そんなときに git stash です。

---
layout: center-image
---

- git stash save
- git stash list
- git stash apply
- git stash drop
- git stash pop (apply して drop する)

<style>
ul {
  text-align: left;
  list-style-type: circle;
  font-size: 1.3rem;
}
</style>

---
layout: center-image
---

<div class="text-3xl text-primary font-bold md-8">
	git rebase
</div>

ちょっと危険なヤツ

ちゃんと理解しておこう

---
layout: center-image
---

rebase はあるブランチのコミットを
別のブランチの歴史につなげます

topic で rebase してみましょう

```mermaid
graph LR
  d01((a311))
  d02((92fb))
  d03((e21b))
  d04((52b1))
  e01((31c2))
  e02((8a24))
  d01 --> d02 --> d03 --> d04
  d03 --> e01 --> e02
  subgraph main
    d04
  end
  subgraph topic
    e02
  end
```

---
layout: center-image
---

同じ変更を別のコミットに変換して、繋げます（ハッシュが異なる）

```mermaid
graph LR
  d01((a311))
  d02((92fb))
  d03((e21b))
  d04((52b1))
  d05((8ab2))
  d06((c1be))
  e01((31c2))
  e02((8a24))
  d01 --> d02 --> d03 --> d04 --> d05 --> d06
  d03 --> e01 --> e02
  e01 -.-> d05
  e02 -.-> d06
  subgraph main
    d04
  end
  subgraph topic
    d06
  end
  style e01 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
  style e02 fill:#fff,stroke:#333,stroke-width:1px,stroke-dasharray: 5 5
```

---
layout: center-image
---

rebase 後は一直線になります

```mermaid
graph LR
  d01((a311))
  d02((92fb))
  d03((e21b))
  d04((52b1))
  d05((8ab2))
  d06((c1be))
  d01 --> d02 --> d03 --> d04 --> d05 --> d06
  subgraph main
    d04
  end
  subgraph topic
    d06
  end
```

---
layout: center-image
---

<br><br>
平行線の歴史を一直線にすることができます

つまり、**「歴史を書き換えます」**

リモートへの影響は常に意識しましょう（何度でも言います）

---
layout: center-image
---

<div class="text-3xl font-bold">
git rebase はいつ使うのか？
</div>

---
layout: center-image
---

<div class="text-3xl font-bold mb-16">
OSS への Pull Requestのときです
</div>

<div class="text-2xl">
main へのマージ前にするケースもあるようです。
<br>
これは組織の方針に合わせてください。
<br>
なお、私はしません。
</div>

---
layout: center-image
---


<div class="text-3xl font-bold mb-8">
レビュワーの気持ちになろう
</div>

<div class="text-xl">
PRを受け取ったら、そのPRはちょっと昔のコミットから生えていた。

おいおい、マージすんの俺かよ・・・

PR 断ろ www
</div>

<br><br>
というのが割とあります。

事前にリベースして、コンフリクトのないPRを作りましょう。

---
layout: center-image
---
<div class="text-xl font-bold mb-8">
  綺麗な歴史は大事
  <br><br>
  でも、OSSの場合は、

  歴史の持ち主は自分ではありません

  いくらコントリビューターと言えども、配慮が必要です。
</div>

---
layout: center-image
---

<div class="text-3xl text-primary font-bold md-4">
	git commit --squash
</div>

複数のコミットを1つにまとめる

---
layout: center-image
---

<div class="text-2xl font-bold md-4">
  コミットが細かくバラバラと切られたPRはなかなかレビューが大変です。
</div>
<br><br>
<div class="text-xl md-4">
  レビュアーの気持ちになって、 1 Issue - 1 Commit を心がけましょう。<br>
  でも、作業中は細かくコミットしておきたい。<br>
  そんな時に squash です。
</div>

---
layout: center-image
---

<div class="text-3xl font-bold">
せっかく OSS へ PR を投げる話になったので、

コントリビューションマナーについて紹介します
</div>


---
layout: image-left
image: 'https://i.gyazo.com/0d53da503208419287de5a8f2cd03b13.png'
---

<div class="text-3xl font-bold">
まずこれを読む
</div>

https://github.com/github/opensource.guide

https://opensource.guide/how-to-contribute/


---
layout: center-image
image: 'https://qvault.io/wp-content/uploads/2020/10/6-Things-to-Avoid-When-Contributing-to-Open-Source-Projects-1536x864.jpg'
---

<div class="text-3xl font-bold">
  この記事がとてもよかったので引用して紹介します
</div>

https://qvault.io/open-source/contributing-to-open-source/

---
layout: center-image
---

<div class="text-3xl font-bold">
  👕 Tシャツ事件をご存知だろうか...
</div>

---
layout: center-image
---

<div class="text-3xl font-bold mb-8">
  👕 Tシャツ事件
</div>

Hacktoberfest という団体がやったイベントで

"なんでもいいから OSS に PR を 4 つ作ったらTシャツあげます!!"

が事件を起こしました

---
layout: center-image
---

<div class="text-7xl font-bold mb-8">
  クソ PR の大量発生
</div>

---
layout: center-image
---

<div class="text-6xl font-bold mb-8">
  憤怒するOSSメンテナー
</div>

---
layout: center-image
image: 'https://qvault.io/wp-content/uploads/2020/10/6-Things-to-Avoid-When-Contributing-to-Open-Source-Projects-1536x864.jpg'
---

<div class="text-3xl font-bold">
  ちなみにこの記事はこの事件がきっかけで生まれました
</div>

---
layout: center-image
---

<div class="text-3xl font-bold">
  6 Things to Avoid When Contributing to OSS
</div>

- Pull Requests Should Handle ONE Thing
- Don't Break Consistency
- Don't Start Work Without Approval
- Don't Re-Open Known Problems/Solutions
- Squash Those Commits
- Be Meaningful

<style>
ul {
  text-align: left;
  list-style-type: circle;
  font-size: 1.3rem;
}
</style>

---
layout: center-image
---

<div class="text-3xl text-primary font-bold mb-4">
  Pull Requests Should Handle ONE Thing
</div>

<div class="text-2xl">
  PRでは1つのトピックに関するもののみ
</div>

<br><br>
<div class="text-xl">
<v-click>

  バグAを修正したよ

  ついでに xxx の書き方が非効率だったから直してやったぜ

</v-click>

<v-click>

<br><br>
<div class="text-3xl">
  はぁぁぁぁああ!??!?!?!?
</div>

</v-click>

</div>

---
layout: center-image
---

<div class="text-3xl text-primary font-bold mb-4">
  Don't Break Consistency
</div>

<div class="text-2xl">
  一貫性を守ること （空気を読んでくれ…）
</div>

<br><br>
<div class="text-xl">
  コーディングスタイルを守って欲しい、ということです。
</div>

---
layout: center-image
---

<div class="text-3xl text-primary font-bold mb-4">
  Don't Start Work Without Approval
</div>

<div class="text-2xl">
  急にPR送ってこないで…

  まずは Issue たてて、コミュニケーションとってからやで…
</div>


---
layout: center-image
---

<div class="text-3xl text-primary font-bold mb-4">
  Don't Re-Open Known Problems/Solutions
</div>

<div class="text-2xl">
  Issue立てる前に似たIssueが既に無いか確認しておいてや…
</div>


---
layout: center-image
---

<div class="text-3xl text-primary font-bold mb-4">
  Squash Those Commits
</div>

<div class="text-2xl">
  PR内のコミットは squash でまとめておいて欲しい…
</div>

---
layout: center-image
---

<div class="text-3xl text-primary font-bold mb-4">
  Be Meaningful
</div>

<div class="text-2xl">
  なるべく意義のある提案をして欲しい
</div>

<div class="text-xl">
  そんなんどうでもええねん！！って言わさないで欲しいということ。
</div>

---
layout: center-image
---

<div class="text-3xl text-primary font-bold mb-4">
  いいコントリビューションはいいIssueから
</div>


<div class="text-xl">
  コントリビューションマナーを見ると、Issueの大切さがよくわかると思います

  いいIssueを目指しましょう
</div>


---
layout: center-image
---

<div class="text-3xl text-primary font-bold mb-4">
  Issue を立てる時に気をつけること
</div>

- Issue の重複はなるべくやめて…
- 感想？観測？どっち？
- テンプレート使ってよ… 🥺
- 情報が少なすぎる
- タイトルから中身が分からない

<style>
ul {
  text-align: left;
  list-style-type: circle;
  font-size: 1.3rem;
}
</style>
