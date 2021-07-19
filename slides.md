---
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

<div class="text-5xl font-bold text-primary pb-4">Thanks</div>

<div class="text-2xl">
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
layout: image-right
---


# Others

- "git やらかしと対処法" : 6
- "VSC と VCS Hosting Service のことについて知っていますか？" : 6
- "Git Client (GUI, TUI, CLI tool) のおすすめたち" : 5
- "ローカルとリモートをちゃんと理解する" : 5
- "GitHub における Markdown 文化とお作法" : 5
- "git の四方山話 (歴史など)" : 2
- "git の基本的な使い方" : 1

---
layout: image-right
---


# Outline

## 1. VCS って何?

## 2. .git の中身

## 3. ちょっと踏み込んだ git

## 4. git のマージは 2 種類

## 5. git-flow の Pros/Cons

## 6. git でやらかさないためにすること

## 7. GitHub の Issue で気をつけること

## 8. OSS コントリビューションマナー

<style>
h2, h3, body {
  font-family: 'Kosugi Maru', 'Signika Negative', sans-serif
}
</style>

---
layout: image-right
---

# ① VCS って何?

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
layout: image-right
---


# "VCS" Software

<br>

Git 以外にも有名なバージョン管理システムがいくつかあります。

いまでも選択肢に上がる現役バリバリなものは以下の通りです

## - Git

## - Subversion

## - Mercurial

---
layout: image-right
---


# Why Git?

<br>
<span style="font-size:32px">
いろいろな選択肢があるのに <br><br>
どうしてみんな Git を使うんだろう??
</span>

---
layout: image-right
---

# Git is Champion?

<br>

## 🙅 NO 🙅

---
layout: image-right
---


# Git + GitHub is Champion !!

<br>

## 🙆‍♂️ YES 🙆‍♂️

### I'm not sure

---
layout: image-right
---


# Git + GitHub is Champion

<br>

Git が流行る前は Subversion が最強でした

昭和からある企業ではまだ Subversion が現役のところもたくさんあります (弊社でも現役です)

そんな Subversion から VCS 王座を奪ったのは

<br>

<span style="font-size:42px">Git ではなく GitHub</span> です（と思っています）

---
layout: image-right
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
layout: image-right
---

# Why Git is good for OpenSource ?

<div>
  Subversion は 中央集中型 と呼ばれます。<br><br><br>
  <img src="/assets/centralized.png" width=200 />
</div>
<div>
  一方、Git は 分散型 と呼ばれます。<br><br><br>
  <img src="/assets/distributed.png" width=200 />
</div>

---
layout: image-right
---


# Subversion

<br>

- リポジトリはサーバー側にのみ作ります
- クライアント側（実装者）は特定の<span style="color:red;">歴史の１ページのみ</span>を引き出します
- 変更の記録・履歴の閲覧など全ての操作はサーバーへの接続が必須です
- バカでかい歴史やバカでかい単一ファイルを扱うのは Subversion が得意です
  - Git で動画を扱ったらすぐに死にます 🧟‍♂️
- Subversion の歴史は絶対です

<div style="
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top:42px;
">
  <img src="/assets/centralized.png" width=200 />
</div>

---
layout: image-right
---

# Git

<br>

- サーバー・クライアント関係なく、<span style="color:red;">すべての環境がリポジトリを持ちます</span>
- 変更の記録・履歴の閲覧など全ての操作はオフラインでも OK です
- 変更の共有（歴史の共有）をリポジトリの同期によって実現します
- 軽いファイルを扱うことを基本とします（GitHub はデフォルトで Max 50MB です）
- Git の歴史は簡単に書き換えることができます（権限があれば）

<div style="
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top:42px;
">
  <img src="/assets/distributed.png" width=200 />
</div>

---
layout: image-right
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
layout: image-right
---

# GitHub makes Git Champion

<br>

GitHub の登場によって、 **オープンソース** 活動が世の中に急速に拡大しました。

その結果、 「Git 最強じゃね？」 となったのです。

Git だけの力では「Git 良さそうだけど Subversion で別にいいわ」となっていたことでしょう。

---
layout: image-right
---

# ② .git の中身を見てみよう

<style>
h1 {
  font-family: 'Kosugi Maru', 'Signika Negative', sans-serif
}
</style>

---
layout: image-right
---

# What's .git ?

<br>
.git は Git <span style="color:red;">リポジトリの情報をすべて保持している</span> 隠しフォルダです

<br><br>
そもそも、PC の特定のフォルダが Git リポジトリになっているということを

各種エディタやターミナルはどうやって知るのか？

.git があるかどうかです

```shell {all|5}
 ~/W/t/gitdir $ la
total 0
drwxr-xr-x  3 sugit  staff    96B  7 16 08:03 .
drwxr-xr-x  4 sugit  staff   128B  7 16 08:03 ..
drwxr-xr-x  9 sugit  staff   288B  7 16 08:03 .git
```

---
layout: image-right
---

# Unpack the .git

<br>

`git init` から見ていきましょう

---
layout: image-right
---

# Unpack the .git

```shell
~/W/t/g/.git $ tree -L 1
├── HEAD
├── config
├── description
├── hooks
├── info
├── objects
└── refs
8 directories, 17 files
```

できたてほやほやの git リポジトリなので、フォルダはありますが中身はありません。

README.md をつくってコミットしてみましょう

---
layout: image-right
---

# Unpack the .git

```shell {all|6}
~/W/t/gitdir $ echo test > README.md
~/W/t/gitdir $ cat README.md
test
~/W/t/gitdir $ git add README.md
~/W/t/gitdir $ git commit -m "initialize repository with README.md"
[master (root-commit) e0167f0] initialize repository with README.md
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
```

コミットが積まれました。

.git をみてみましょう。

---
layout: image-right
---


# Unpack the .git

```shell {all|4}
~/W/t/.git $ tree
// ~~~省略~~~
├── logs
│   ├── HEAD
│   └── refs
│       └── heads
│           └── master
├── objects
│   ├── 9d
│   │   └── aeafb9864cf43055ae93beb0afd6c7d144bfa4
│   ├── c1
│   │   └── 2d7c0ed49ad9c7aa938743ba6fdee54b6b7fe1
│   ├── e0
│   │   └── 167f03015fa0ea463267610d1b16e82c91a4c9
│   ├── info
│   └── pack
```

なんか増えてますねぇ。

---
layout: image-right
---


# Unpack the .git

```shell {all|1}
[master (root-commit) e0167f0] initialize repository with README.md
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
```

```shell {all|6-7}
├── objects
│   ├── 9d
│   │   └── aeafb9864cf43055ae93beb0afd6c7d144bfa4
│   ├── c1
│   │   └── 2d7c0ed49ad9c7aa938743ba6fdee54b6b7fe1
│   ├── e0
│   │   └── 167f03015fa0ea463267610d1b16e82c91a4c9
│   ├── info
│   └── pack
```

<v-click>

おや、一致した ID が見つかりましたね

</v-click>

---
layout: image-right
---


# Unpack the .git

<br>
実は objects には README.md を圧縮したものが入っています

これがあるから、`git reset` ができるのです。

---
layout: image-right
---

# Unpack the .git

- HEAD
  > 0000000000000000000000000000000000000000 e0167f03015fa0ea463267610d1b16e82c91a4c9 SuGit <sgmt.snj@gmail.com> 1626391666 +0900 commit (initial): initialize repository with README.md

分解すると

```shell
0000000000000000000000000000000000000000 ## <- 1つ前のコミットハッシュ
e0167f03015fa0ea463267610d1b16e82c91a4c9 ## <- 自身のコミットハッシュ
SuGit <sgmt.snj@gmail.com> ## <- コミッター
1626391666 +0900 ## <- コミット時刻
commit (initial): initialize repository with ## <- メッセージ
```

となっています

---
layout: image-right
---


# ③ ちょっと踏み込んだ git

<style>
h1 {
  font-family: 'Kosugi Maru', 'Signika Negative', sans-serif
}
</style>

---
layout: image-right
---

# ④ git のマージは 2 種類

<style>
h1 {
  font-family: 'Kosugi Maru', 'Signika Negative', sans-serif
}
</style>

---
layout: image-right
---


# ⑤ git-flow の Pros/Cons

<style>
h1 {
  font-family: 'Kosugi Maru', 'Signika Negative', sans-serif
}
</style>

---
layout: image-right
---

# ⑥ git でやらかさないためにすること

<style>
h1 {
  font-family: 'Kosugi Maru', 'Signika Negative', sans-serif
}
</style>

---
layout: image-right
---


# ⑦ GitHub の Issue で気をつけること

<style>
h1 {
  font-family: 'Kosugi Maru', 'Signika Negative', sans-serif;
}
</style>

---
layout: image-right
---


# ⑧ OSS コントリビューションマナー

<style>
h1 {
  font-family: 'Kosugi Maru', 'Signika Negative', sans-serif
}
</style>

---
layout: image-right
---

# THANKS
