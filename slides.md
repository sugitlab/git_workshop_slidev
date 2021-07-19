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

<div class="text-3xl font-bold">早速ですが質問です</div>

---
layout: center-image
---

<div class="text-5xl font-bold">どうして Git を使っているのですか??</div>


---
layout: center-image
---

<div class="text-5xl font-bold">Git以外...選択肢あるの? 🤔</div>

<br>

<v-click>
  <div class="text-4xl font-bold">安心してください。Git でOKです 💁🏻‍♂️</div>
</v-click>

---
layout: center-image
---

<div class="text-2xl font-bold leading-relaxed">
  ソースコードを管理するなら、現時点での最善はGitだと思います <br>
  しかし、まだまだ Git ではない現場というのもあるのです… 
</div>

---
layout: center-image
---

<div class="text-2xl font-bold leading-relaxed">
  これに対して<br>
  「なんだ、時代遅れの会社か 🤷🏼‍♂️」<br>
  と言う人は、大体何もわかってない人です。<br>
  無視しましょう🙆‍♂️
</div>

---
layout: center-image
---

<div class="text-2xl font-bold leading-relaxed">
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
image: '/assets/git-svn.png'
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
image: '/assets/distributed.png'
equal: false
---

<div class="text-2xl font-bold">
  Git は 分散型 だからです
</div>

---
layout: image-right
image: '/assets/centralized.png'
equal: false
---

<div class="text-2xl font-bold">
  一方、Subversion は 中央集中型 と呼ばれます
</div>

---
layout: image-left
image: '/assets/git01.png'
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
image: '/assets/svn01.png'
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
  Git + GitHub is Champion!!
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
image: '/assets/git-svn.png'
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

<div class="text-3xl">
適当なフォルダで
</div>

```shell
$ git log
```

<div class="text-3xl">
とたたくと
</div>

```shell
fatal: not a git repository (or any of the parent directories): .git
```

と怒られます

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
