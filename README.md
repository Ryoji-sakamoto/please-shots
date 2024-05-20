# なんでこんなものを作ってしまったのか
バーでバイトしているのですが、オーナーに"お客様にショットを飲んでもらうにはどうすればいいか"と聞かれた時に私は"QRコードとか手軽なもので伝えるようにしたらいいのでは"と言いました。"じゃあ作って"と言われました.
軽はずみな発言でした、「沈黙は金なり」まさにこのことではないか。

## 備忘録として残しておきたいので、具体的な手順とともに説明します。

GitHub Pagesを使用する具体的な手順（自動再生対応）
### 1. リポジトリにファイルをアップロードリポジトリページで「Add file」→「Upload files」をクリックします。
### 2.MP4動画ファイルを選択してアップロードします。
### 3.以下の内容のHTMLファイル（index.html）を作成してアップロードします。
index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Auto-play Video</title>
</head>
<body>
    <video width="100%" height="auto" autoplay controls>
        <source src="your-video.mp4" type="video/mp4">
        Your browser does not support the video tag.
    </video>
</body>
</html>
```
your-video.mp4をアップロードしたMP4ファイル名に置き換えてください。
「Commit changes」をクリックしてファイルをリポジトリに追加します。
### 4. GitHub Pagesを有効化
リポジトリのトップページに移動し、右上の「Settings」をクリックします。
左側のメニューから「Pages」を選択します。
「Branch」を選択し、main（またはmaster）ブランチを選択します。
「Save」をクリックします。
ページがリフレッシュされると、公開されたページのURLが表示されます。これがあなたのサイトのURLです（例: https://username.github.io/repository-name/）。
### 5. QRコードを生成
公開されたページのURLをコピーします。
QRコードジェネレーター（私が使った[サイト](https://qr.quel.jp/url.php)です）を使って、コピーしたURLを入力し、QRコードを生成します。
生成されたQRコードをダウンロードして、おしまいです
