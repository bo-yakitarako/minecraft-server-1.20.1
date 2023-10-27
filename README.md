# みんなでマイクラしよう
しんにじえもです。僕のマイクラ参加型配信は基本工業MODを入れた工業サーバーになります。<br>
サーバーアドレス: mc.bo-yakitarako.dev

なんで、みなさんには当方と同じMODを入れてもらいたいんですよね。MODとconfigの共有方法をお話します。

※MOD導入云々の話はいたしません。MODの入れ方わからんって方は頑張って理解してきてください。

## forgeバージョン
[forge-1.20.1-47.1.46](https://maven.minecraftforge.net/net/minecraftforge/forge/1.20.1-47.1.46/forge-1.20.1-47.1.46-installer.jar)を使っています。

古いバージョンだと動かない場合があるのでお気をつけください。<br>
(2023/9/20現在のRecommendedバージョンである1.20.1-47.1.0では動きませんでした)

## Git分かる方向け
マイクラのゲームディレクトリにしたい1つ上の階層で
```
git clone https://github.com/bo-yakitarako/minecraft-server-1.20.1.git
```
で`minecraft-server-1.20.1`フォルダをゲームディレクトリに指定してプレイしてください。

MOD追加やconfig変更があった場合は
```
git pull
```
で変更を適用してマイクラを再起動しましょう。

## GitHub Desktopを使う方法(推奨)
GitHub Desktopを使うとこんなに便利に！
- zip持ってきて解凍なんかしなくて直接ここの内容を適用できる！
- MODやconfigの追加や変更があった場合、ボタンポチするだけで変更を適用できる！
- とにかくここと同じ内容をめっちゃ楽に適用できる！

セットアップもそんな難しくないので実際にやってみましょう。

### 1. GitHub Desktopのダウンロード
[GitHub Desktopのダウンロードページ](https://desktop.github.com/)から入れましょう

### 2. ログイン
セットアップを適当に済ませてからGitHub Desktopを開くとこんな画面になります。
![image](https://github.com/bo-yakitarako/minecraft-server-1.20.1/assets/55777096/7fe8dd01-0379-4945-97ea-7a3ae5c395f1)
`Sign in to GitHub.com`を選択するとブラウザでGitHubが開いてログインを求められますので適当にログインします。

ログインするとこの画面に遷移します。
![image](https://github.com/bo-yakitarako/minecraft-server-1.20.1/assets/55777096/a421232e-bb7d-4c4a-b9b1-97a815a513c9)
ここは何も変えずに`Finish`で良いと思います。

すると`Let's get started!`のスタート画面に移行します。

`Let's get started!`|`File`タブ
--|--
![image](https://github.com/bo-yakitarako/minecraft-server-1.20.1/assets/55777096/11ba9686-0c6e-49ea-982c-beb4db491034)|![image](https://github.com/bo-yakitarako/minecraft-server-1.20.1/assets/55777096/bff7ac54-3f5f-4f1f-b6ee-982fa8538a8d)

ここでは2個目の`Clone a reopsitory from internet...`を選択します。

もしくは画面上部の`File`から`Clone repository...`でも大丈夫です

GitHub Desktop画面|GitHubのサイトの操作
--|--
<img src="https://github.com/bo-yakitarako/minecraft-server-1.20.1/assets/55777096/4dbd707a-3bcc-4e91-b03a-5d8be00fdb78">|<img src="https://github.com/bo-yakitarako/minecraft-server-1.20.1/assets/55777096/80e85061-2ebc-4148-8dd1-01a9da48c477" width="640px">

ダイアログが開くので`URL`のタブを選択します。

- 1個目の入力欄にGitHubサイトのほうの`Code`というボタンをクリックすると出てくるURLを貼ります
  - https://github.com/bo-yakitarako/minecraft-server-1.20.1.git ←これをコピペでもOKです
- 2個目の入力欄は右の`Choose...`というボタンを押してマインクラフトの**ゲームディレクトリを入れる1個上のフォルダ**を指定します
  - 指定したフォルダの中に`minecraft-server-1.20.1`というフォルダが作成され、その中に`mods`や`config`フォルダが入ります
  - ゲームディレクトリにしようとしたフォルダを選択すると二重でフォルダが形成されてしまうのでご注意！

 入力が完了したら`Clone`をクリックします。

![image](https://github.com/bo-yakitarako/minecraft-server-1.20.1/assets/55777096/161efa95-cf0a-4553-9da2-7c019bf54441)
こんな画面になればOKです🙆

これで指定したフォルダにMODが入った`mods`フォルダや`config`フォルダが形成されます！
![image](https://github.com/bo-yakitarako/minecraft-server-1.20.1/assets/55777096/ad54f8ad-b42f-4c9e-9bc3-54545f7162c7)

あとは`minecraft-server-1.20.1`フォルダをMinecraftのゲームディレクトリに指定してforgeで起動しましょう。

#### MODの追加やconfigの変更があった場合
![image](https://github.com/bo-yakitarako/minecraft-server-1.20.1/assets/55777096/031639ea-13e3-40cc-ab2d-ff4099e0dd82)

ここの`Fetch origin`というボタンを押せば勝手にファイルを引っ張ってきて適用してくれます！

## zipインストールしてmodsやconfigを適用する場合(非推奨)
このページの`Code`というところを押して出てくる`Download ZIP`を押すと、このページの階層構造がまんま入ったZIPファイルがダウンロードできます。
![image](https://github.com/bo-yakitarako/minecraft-server-1.20.1/assets/55777096/080be972-7f76-4bc1-b503-3ca900daf7c9)

あとはZIPファイルを展開してconfigとmodsをゲームディレクトリにぶちこんでください。

MODの追加やconfigの変更があるたびこの作業しないとなので結構ダルいと思いますｗ
