# 通知
シナリオに通知先を設定をすると、シナリオが発動された際に通知が送付されます。通知先の設定については[通知先の設定](./studio/recipient-settings.md)を参照してください。  
通知から様々なアクションを実行することで、素早いアセットの現状把握を支援します。例えば、アセットを過去の状態と比較、スレッドを作成して分析、アセットに設定されているURLへの遷移など、通知からPITWALLの各ページへ遷移することが可能です。通知を受けてから、PITWALLで当該通知の内容を探す手間なども省略できます。通知先によって、通知のレイアウトや表示などが変化しますが、通知コンテンツは原則同じです。

下記の例は、Webhook機能を利用してTeamsに通知を受領した際のサンプル画面です。  <figure><img src="../.gitbook/assets/Notification_Teams_Sample_jp.png" width="50%" alt="通知サンプル"></figure>
通知ヘッダー
- 件名：PITWALLからの通知であること、シナリオタイプ、そしてシナリオ名が記載されます。
- Triggered：シナリオが実行された日時。
- 説明：シナリオタイプ名と実行されたシナリオ名が記載されます。
<figure><img src="../.gitbook/assets/Notification_Teams_Title_jp.png" width="50%" alt="通知タイトル"></figure>

通知は下記のコンテンツで構成されます。<figure><img src="../.gitbook/assets/Notification_Teams_Title_Contents_jp.png" width="50%" alt="通知コンテンツ"></figure>
- View Alert：シナリオがアラート起因の場合、アラートの履歴ページへ遷移します。
- Open All：シナリオに設定されているアセットへジャンプすることができます。
- Download：シナリオの設定で取得されたスクリーンショットをダウンロードすることができます。
- Compare：直近で取得されたスクリーンショット画像と、過去に取得されたスクリーンショット画像を比較する画面へ遷移します。
- Create a Thread：直近で取得されたスクリーンショットをもとに、スレッドを作成します。スレッド機能については[スレッド](../tutorial-get-started/collaboration/threads.md)ページを参照してください。

最後にアセットグループ名とシナリオ名が記載されています。<figure><img src="../.gitbook/assets/Notification_Teams_Title_Footer_jp.png" width="50%" alt="通知コンテンツ"></figure>
シナリオ名をクリックすることで、シナリオに登録されているアセットへジャンプすることができます。スクリーンショット設定をしていない場合は、通知に記載されません。