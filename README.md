# 2017年プレ卒論配属の楽しい実習

## 宿題: GitHubの準備

### 準備0: GitHubの基本用語
以下の「Gitの基本用語」のページを読む
- http://bcl.sci.yamaguchi-u.ac.jp/~jun/notebook/git/intro

### 準備1: ローカルレポジトリの準備
プログラムを作ったフォルダを整理しておく
- 不要なファイルは消す
- ファイル名は，その内容がわかりやすい名称に

### 準備2: 手元のマシンの準備
Gitを使う方法を大別すると2通りある。**長期的には方法1を使えるようにする** こと。短期的には方法2でもいいが，使い方は各自調べること。

[方法1] コマンド直打ちで使う
- Windowsの場合は以下を見てGit Bashを使えるようにすれば，LinuxやMacと同様に
	ターミナル上で操作できる。
	https://qiita.com/shinsumicco/items/a1c799640131ae33c792
- Mac/Linuxはターミナル上で，以下のURLにある「準備3」を実行しておく。 http://bcl.sci.yamaguchi-u.ac.jp/~jun/notebook/git/preparation

[方法2] GitHub　DeskTopをつかう。
- https://desktop.github.com/ からダウンロードする。
- 使い方は各自google先生に聞いて調べる

### 準備3: GitHubを使う
1. 以下のリンクをクリック(今回の実習用レポジトリを準備する)

	https://classroom.github.com/classrooms/34051886-18bcl-exercises

2. メールが届くので”View invitation”をクリックしてGitHubにログイン
3. これでGitHub上にリモートレポジトリができる。
4. ここからの作業は，前述の「準備2」の2つ方法のどちらを使うかで方法が異なる
	(方法1)
  1. ターミナルを開き「準備1」でつくったローカルレポジトリのフォルダに移動
	2. GitHubの画面に表示されているコマンドを実行する。だいたい以下のような内容のはず。
  ```
  $ echo "# Arduino+EMGのおもしろプログラム"
  $ git init
  $ git add .
  $ git commit -m "はじめてのcommit"
  $ git remote add origin https:/// <=ここは各自異なる
  $ git push -u origin master
  ```

        - リポジトリ名はもGitHubのページの上の方にある。なれない時には余計な設定が不要なHTTPS を使う。
		- 解説は以下にもある。
		http://bcl.sci.yamaguchi-u.ac.jp/~jun/notebook/git/init
(方法2)
    1. GitHub Desktopを起動して，ローカルレポジトリの場所と，上記リモートレポジトリの登録をする
    2. ローカルレポジトリの内容をリモートレポジトリにpushする。
