# ブラウザ拡張機能

現在、Chrome拡張機能はパッケージとしてプライベートに提供されています。

## パッケージ及びインストール方法
最新のChrome拡張機能は[ここから](https://drive.google.com/drive/folders/1KQhEO_SMMr_kfwVEthifNThVUM6TRTbh?usp=drive_link)入手できます。
インストール方法は[ここ](tutorial-get-started/browser-extension/install.md)を参照ください。

## ブラウザ拡張機能の主な機能
Chrome拡張機能は「Instant lookup」と「Clipper」の２つ機能があります。

<figure><img src="../../.gitbook/assets/pitwall_browser_extension_ja.png" width="50%" alt="PITWALL拡張機能"></figure>

### Instant Lookup
ブラウザー拡張機能のインスタントルックアップを利用し、シナリオのルックアップに設定されているURLを表示することができます。

- 利用方法
  - 右上の ![](../../.gitbook/assets/pitwall_browser_extension_icon.png) アイコン > Instant lookup を選択します。Scenario のプルダウンからシナリオを選択します。Lookup のプルダウンからルックアップを選択します。選び終わりましたら、Take screenshot ボタンをクリックして、シナリオのルックアップに設定されている "Asset" のURLのスクリーンショットがシナリオに設定されている通知先に通知メッセージが送信されます。<br>
  Find ボタンをクリックするとシナリオのルックアップに設定されている "Asset" のURLが表示されます。


### Clipper
Clipperには[Take screenshot]と[Start recording]の２つの機能があります。

#### Take screenshot
スクリーンショットを撮る時に使います。

スクリーンショットを撮るためのオプションはChromeタブ、ウィンドウ、画面全体の３種類あります。<br>
Chromeタブ：Chromeブラウザで開いている複数のタブからスクリーンショットを撮りたいタブを選択できます。<br>
ウィンドウ：開いている複数のウィンドウからスクリーンショットを撮りたいウィンドウを選択できます。<br>
画面全体：画面全体を撮りたい場合に利用するオプションです。

- 利用方法
  - 右上の ![](../../.gitbook/assets/pitwall_browser_extension_icon.png) アイコン > Clipper > Take screenshot を選択します。<br>
  Chromeタブ、ウィンドウ、画面全体の３種類のオプションから撮りたい個所のスクリーンショットを選びます。<br>
  選び終わりましたら共有ボタンをクリックします。
  - Clip name、Destination thread、Destination tabを記入して Save ボタンをクリックします。上記で記入したところにスクリーンショットが表示されます。<br>
  <figure><img src="../../.gitbook/assets/browser_extension_save_clip_ja.png" width="50%" alt="Clipper"></figure><br>
  Clip name：スクリーンショットの名前を指定します。<br>
  Destination thread：表示するスレッドの名前を指定します。<br>
  Destination tab：表示するスレッドのタブを指定します。新しいタブも指定できます。

#### Start recording
画面操作をしながら動画を撮る時に使います。実際の画面操作を簡単に共有することができます。

- 利用方法：
  - 右上の ![](../../.gitbook/assets/pitwall_browser_extension_icon.png) アイコン > Clipper > Start recording を選択します。Chromeタブ, ウィンドウ, 画面全体 の３種類のオプションから撮りたい箇所のビデオを選びます。選び終わりましたら"共有"ボタンをクリックして、録画が開始します。右上の ![](../../.gitbook/assets/browser_extension_stop_icon.png) アイコンをクリックして録画を完了します。
  - Clip name, Destination thread, Destination tabを記入してSaveボタンをクリックします。<br>
  <figure><img src="../../.gitbook/assets/browser_extension_save_clip_ja.png" width="50%"></figure><br>
  Clip name：録画したビデオの名前を指定します。<br>
  Destination thread：保存先スレッドの名前を指定します。<br>
  Destination tab：保存先スレッドのタブを指定します。新しいタブも指定できます。