## where we play
Visit our website [here](https://we-are-tentatively.github.io/in-correspondence/)!

## where we talk
ひるめり [@hirumeri](http://twitter.com/hirumeri)  
s.kawano [@kkhaiya](http://twitter.com/kkhaiya)

## welcome to our playground!

いっしょに遊ぶために、いくつか準備いただかなくてはいけないことがあります。ぼくたちも決してこうしたことに明るいわけではないので、なんともおぼつかないご案内になってしまうのですが、とにかく書き始めてみようと思います。

### GitHubのアカウントを作成する

まずはGitHubのアカウントを作成し、ぼくたちにお知らせください。あなたのアカウントがこの場所のテキストを編集できるようご招待します。

じつはこれだけで、GitHub上のコードを直接ブラウザから編集し、直接リモートリポジトリにcommitすることもできてしまうはずです。ブラウザからの編集はさほど快適ではないかもしれませんが、最初はこの環境ではじめてしまって構いません（ただし、別の人による競合した変更があった際にブラウザ上の変更がコミットできず、リロードが必要になる可能性があるのでご留意ください）。

下記では、ローカルリポジトリ、つまりあなたのPCのフォルダ上でファイルを編集するための設定をご紹介します。きっと下記の説明にしたがったとしてもエラーが出ることになってしまうのではと思うのですが、なにか困ったことがあったら、どうぞ遠慮なくご連絡ください。最初の設定にちょっと手こずることがあるとしても、そのあとはとても簡単につかうことができます。

### gitをインストールする

GitHubは、gitというツールを便利に使用するためのサービスです。この場所のテキストをローカルで編集できるよう、まずはローカルのPCにgitをインストールする必要があります。

（インストールの方法は、たとえば[こういうサイト](http://proengineer.internous.co.jp/content/columnfeature/6893)を参考にしてみてください。）

### VS Codeをインストールする

必ずしもVS Code（Visual Studio Code）を使わなくてもかまわないのだけど、これがあればこの場所のテキストを書くためのマークダウン形式のファイルが確実に開けるし、しかもほとんどコマンドを打たずにgitを使うことができます。だからとりあえずインストールしてしまっていいんじゃないかしら（たとえば[こういうサイト](https://www.karelie.net/install-vscode-windows/)を参考にしてみてください）。

このVS Codeが、世に言うテキストエディタのひとつです。もちろん、すでに使い慣れたテキストエディタがあればそちらをご使用ください。

### このリポジトリをクローンする

インストールを済ませたら、VSCodeを起動し、F1キーを押してみてください（Macであれば、fn+F1のほうがよいかもしれない）。画面上部に検索窓が現れるので、`clone`と打ち、さらにこのリポジトリのURL`https://github.com/we-are-tentatively/in-correspondence.git`を入力します。すると、あなたのPCのどこかに"in-correspondence"というディレクトリが作成され、そしてそれがVS Codeから見えるようになっているはずです（ディレクトリとフォルダの意味はほとんど同じであるそうですが、ディレクトリといったほうが、前途洋々とした古き佳き計算機の夢のにおいがするような気がしませんか？）。

このディレクトリがローカルリポジトリで、なかにはGitHubのリモートリポジトリにあるのと同じファイルたちがコピーされているはずです。

### 変更したいテキストのファイルを見つけて、編集する

ローカルリポジトリの"in-correspondence"配下に、"_posts"というディレクトリがあるかと思うのですが、このなかに、マークダウン形式で書かれたそれぞれの記事のテキストが入っています。たとえばぼくたちの最初の犬の記事ならば、2019-04-09-with-dogs.md という具合に。

さしあたり、編集に関する羅針盤はありません！　好きな記事を選んで、どこまでも遠くへ旅をなさってください（でも、最初は大事をとって、少しだけテキストを編集したうえでcommitとpushを試してみたほうがいいかもしれません）。もしさまざまな仕組みに馴染んできたら、あたらしく記事を追加いただいても大丈夫です。

### commitする

編集を終えたら、Ctrl+Sなどを押して保存します。 それから、VS Codeの左サイドのメニューに、消防署の地図記号のようなY字形のアイコンがあると思うので、これを押すとあなたが編集したファイルの名前がすべて見えるはずです。ファイルの横のプラスの形のアイコンを押すと、変更がstageされます。stageするというのは、この変更をつぎのcommitに含めてね、と指示することです。

その上にメッセージを書く窓があるので、そこにコミットメッセージを書き込みます（一般的な開発であればちゃんとしたルールのもとにコミットメッセージを書いたほうが良いのだと思うのですが、ぼくたちはきわめて気ままに記入しています）。そしてチェックマークのアイコンを押して、commitします。commitすることで、変更内容の差分の記録がローカルレポジトリに作成されます。保存とcommitは感覚的にはとても似ていますが、保存とは上書きであるのに対し、commitとは差分の確定である、といったような感じでぼくたちはふんわり理解しています。

そうそう、VS Codeは、stageするのを忘れてcommitしたとしても、stageしたうえでcommitしますか？と親切にメッセージを出してくれるので、stageのことはあまり心配しなくてかまいません。

### pushする

commitはローカルリポジトリでの差分の確定でしたが、これをリモートリポジトリに反映させるのがpushです。commitしたら、「…」マークのメニューから「push」を選択します。すると、なにもかもうまくいっていれば、あなたのcommitがリモートリポジトリ、つまりはGitHubのページから見えるファイルに反映されているはず！

GitHubに変更が反映されると、それがそのままビルド&デプロイされる（つまりはウェブサイトも更新される！）なので、（反映に時間がかかることがあるのですが）それも確かめてみてください。

### pullする

編集を再開する際には、リモートリポジトリに他の人がくわえたcommitを自分のローカルリポジトリに反映させる必要があります。これをpullするというのですが、VS Code上での操作はpushとほとんど同じです。

### we will be taking off shortly....

ここまで来れば、あとのルーティンはとても簡単です。PCを起動し、VS Codeを開き、まずはpullして、他のひとがpushしたかもしれない差分をローカルリポジトリに反映する。それから、VS Codeから見える_postsフォルダの中の、マークダウン形式のファイルの内容を自由に編集し（場合によってはファイルを新規追加し）、編集がある程度まとまったらcommitする。作業が一段落したらpushし、リモートリポジトリに自分の変更を反映する。しばらくすると、ぼくたちのあのウェブサイトに自動的に変更が反映され、記事の内容が最新化されているはずです。