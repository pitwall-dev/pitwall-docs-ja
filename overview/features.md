# 機能紹介

<!--
# ✨ 機能紹介
-->

## Studio

Studioでは、さまざまなツールを横断して確認する必要がある情報を、アラートへ付加することができます。インシデントの状況に応じたアドホック調査を可能にし、組織内でのプロセスの標準化にもつながります。

* ルックアップ機能を構築
* 即座にトリアージと分析を行うためのスクリーンショット機能
* お使いのツールへの変更は不要

<figure><img src="https://lh7-us.googleusercontent.com/7y1ps6PAy_YUwi_FifO_BggULmAUTTSO1yksSdRvfF8ODiDQrzEjwA8CWKzqjqCo_IksRcaMn6A736d8nLdGo9SMIc1KV9QZzdHYDqgx9ShSOtUNSQL2_WMCjbrtV-yERDfLW8lIVE-zzs8dum95sLFInw=s2048" alt=""><figcaption></figcaption></figure>

## アラートマネージャー

PITWALLは、Coralogix, Splunk, New Relicなどの監視ツールから受け取ったアラートを、さまざまなツール間でレビューしたい内容をクリック可能なリンクとして、横断的につなぎ合わせます。

これにより、必要な情報に即座にアクセスできます。ブラウザを開いたり、ツールを切り替えたり、アラート発生時間までダッシュボード上の時間範囲を調整したりする必要はもうありません。今お使いのツールに変更を加えずに、Studio上で設定するだけで済みます。


<figure><img src="../.gitbook/assets/image (46).png" alt=""><figcaption><p>Alert in Slack</p></figcaption></figure>

## ブラウザ拡張機能

ブラウザ拡張で、ブラウザ内の文字列をキーとして調査を実施できます。この軽量な検索ツールでさまざまなデータを手作業で検索する時間を節約できます。<br>

例：
* DevOps
  * アプリケーションパフォーマンスのトレースデータ取得
* セキュリティ
  * IPレピュテーション確認
  * マルウェアサイト確認
  * フィッシングサイト確認
  * ファイルハッシュ値確認
* 一般的な用途
  * Google検索

<figure><img src="../.gitbook/assets/image (53).png" alt=""><figcaption><p>Browser Extension</p></figcaption></figure>

{% embed url="https://drive.google.com/file/d/1BEEYkK2UUlHN-OfNpkXtMpKki2NeA0Lg/view?usp=sharing" %}

## イベントログ / インサイト

イベントログ（Snapview）とインサイトは、下記を用いてインシデントを比較・分析するのに役立ちます。PITWALLは、ログ、メトリクス、トレーシングなど異なるツール間のデータを相関させる手段をDevOPsチームに提供します。しかしこれらツールから得られる相関関係は、アラートやインシデント発生時のものでしかないため、問題の根本原因を即座に分析できるとは限りません。SnapViewでは、ツールごとに3つの異なる観点で、DevOPsチームが問題特定のお手伝いをします。

以下、機能比較

1. （過去のある時点の）ルックバック機能
2. 過去のイベント
3. ベースライン機能

<figure><img src="../.gitbook/assets/image (63).png" alt=""><figcaption><p>SnapView</p></figcaption></figure>

### ルックバック機能 <a href="#other-times" id="other-times"></a>

この機能では、対象データを、任意の時間帯で見ることができます。

たとえば、あるダッシュボードをある時点で使用し、また、過去のある時点でも使用していた場合、 事前設定したルックバックオプションやオンデマンドにて特定時間の比較が可能です。

### 過去のイベント <a href="#past-evemts" id="past-evemts"></a>

対象の参照したい過去のイベント（アラート / インシデント）を見ることができます。例として、#125が分析の必要なイベントであった場合、それ以前のイベントも参照できます。

* \#125 - 分析が必要なイベント
* \#120 - 過去のイベント
* \#081 - 過去のイベント

### ベースライン機能 <a href="#baselines" id="baselines"></a>

この機能では、機械学習とデータ（スクリーンショット）のセットが必要となりますが、トラブルシューティングに必要な情報をDevOpsチームに提供します。 この例ではAWS合成データにより分析をおこないます。具体的にはウエブサイトへ継続的にアクセスし、その応答時間にもとづいてベースラインを規定します。PITWALLでは、事前定義したスナップショット（ダッシュボード上のイメージ）を元に、これをおこないます。

{% hint style="info" %}
ベースライン機能は、ロードマップに含まれており、2024年にリリースされる予定です。
{% endhint %}
