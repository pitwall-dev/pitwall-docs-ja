## ブラウザの自動化 
ブラウザを自動化させることによって、ユーザが行うブラウザ操作をシミュレートし、自動的にブラウザ操作とスクリーンショット取得を行う事が出来ます。
例えばユーザネームとパスワードが必要なサイトで自動的にユーザネームとパスワードを入力し、ログイン後のスクリーンショット取得したい場合や、
Google等の検索サイトで自動的に検索ワードを入力、クリックを押下し、画面遷移した後のスクリーンショットを取得したい場合、ブラウザ自動化機能が役立ちます。

### オートメーションを新規作成
ブラウザを自動化させ、スクリーンショットを取得するにあたって、オートメーションの新規作成を行います。
以下、ブラウザを自動化させ、ユーザが行うブラウザの操作をシミュレートし、スクリーンショットを取得する場合の例になります。

オートメーションを新規作成をクリック。モーダル画面の「スクリーンショットフローの更新」で以下のようにスクリーンショットフローを設定します。フローを作成中にプレビューしたい場合は、画面右の「このフローをプレビューする」ボタンを押下することで、プレビュー出来ます。


{% tabs %}
{% tab title="ユースケース1" %}

Tocaroでユーザーネームとパスワードを入力してログイン後のスクリーンショットを取得する場合。

- ステップ1
  - 1.「機能」を「Go to(特定のページに移動する)」に設定する。
  - 2.「引数」を「Built-in(組み込みから選ぶ)」に設定する。
  - 3.「組み込み変数」を「URL(生成されたURLを使用する)」に設定する。
  - 4.「完了」ボタンを押下。

[picture]

- ステップ2
  - 1.「機能」を「Type(ユーザーの入力アクティビティをシミュレートする)」に設定する。
  - 2.「引数」を「Selector(CSSセレクター)」に設定する。
  - 3.「値」を「#id_username」に設定する。
    - IDの取得方法は以下になります。(ID取得方法は執筆中です)
    - Tocaroのログインページを開き、メールアドレス欄にて右クリックし、「検証」を選択。
    - 右ペインのdevtoolsのelementsタブのハイライトされている箇所を右クリックし、Copy Selectorを選択。
  - 4.「下記を待機」を「Wait until(あるイベントが起こるまで待つ)」に設定する。
  - 5.「ライフサイクル」を「Network Idle 2(ネットワークアイドル2)」に設定する。
  - 6.「引数」を「Built-in(組み込みから選ぶ)」に設定する。
  - 7.「組み込み変数」を「Username(スクリーンショット設定で設定します)」に設定する。
  - 8.「完了」ボタンを押下。

[picture]

 - ステップ3
   - 1.「機能」を「Type(ユーザーの入力アクティビティをシミュレートする)」に設定する。
   - 2.「引数」を「Selector(CSSセレクター)」に設定する。
   - 3.「値」を「#id_password」に設定する。
   - 4.「下記を待機」を「Wait until(あるイベントが起こるまで待つ)」に設定する。
   - 5.「ライフサイクル」を「Network Idle 2(ネットワークアイドル2)」に設定する。
   - 6.「引数」を「Built-in(組み込みから選ぶ)」に設定する。
   - 7.「組み込み変数」を「Password(スクリーンショット設定で設定します)」に設定する。
   - 8.「完了」ボタンを押下。

[picture]

- ステップ4
  - 1.「機能」を「Click(ユーザーのクリックアクティビティをシミュレートする)」に設定する。
  - 2.「引数」を「Selector(CSSセレクター)」に設定する。
  - 3.「値」を#login-form > div.submit-row > input[type=submit]
  - 4.「下記を待機」を「Wait until(あるイベントが起こるまで待つ)」に設定する。
  - 5.「ライフサイクル」を「Network Idle 2(ネットワークアイドル2)」に設定する。
  - 6.「完了」ボタンを押下。

[picture]

※「スクリーンショットフローのプレビュー」のURL欄にTocaroのURL、ユーザー名欄にTocaroのユーザーネーム、パスワード欄にTocaroのパスワードを入力してください。

{% endtab %}

{% tab title="ユースケース2" %}
Gooleにて検索ワードを入力し、Enterを押下し、画面遷移した直後の画面のスクリーンショットを取得する場合。

- ステップ1
  - 1.「機能」を「Go to(特定のページに移動する)」に設定する。
  - 2.「引数」を「Built-in(組み込みから選ぶ)」に設定する。
  - 3.「組み込み変数」を「URL(生成されたURLを使用する)」に設定する。
  - 4.「下記を待機」を「Wait until(あるイベントが起こるまで待つ)」に設定する。
  - 5.「ライフサイクル」を「Network Idle 2(ネットワークアイドル2)」に設定する。
  - 6.「完了」ボタンを押下。

[picture]

- ステップ2
  - 1.「機能」を「Wait and Type(セレクタを待って入力します)」に設定する。
  - 2.「引数」を「Selector(CSSセレクター)」に設定する。
  - 3.「値」を「##APjFqb」に設定する。
  - 4.「引数」を「Static(CSSセレクター)」に設定する。
  - 5.「値」に「検索したい文字」を入れる。
  - 6.「完了」ボタンを押下。
  
[picture]

- ステップ3
  - 1.「機能」を「Enter(Enterキーの押下をシミュレートする)」に設定する。
  - 2.「完了」ボタンを押下。

[picture]

※「スクリーンショットフローのプレビュー」のURL欄にGoogleのURLを入力してください。

{% endtab %}
{% endtabs %}

(パラメータのそれぞれの意味は執筆中です)