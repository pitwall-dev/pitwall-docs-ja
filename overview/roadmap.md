# ロードマップ

<!--
# 🏎️ ロードマップ
-->

## 機能

* [x] チームアカウント
* [x] Studio
  * [ ] シナリオのコピー機能
  * [x] ドラッグ＆ドロップ操作 :tada:
* [x] アセット
* [x] シナリオ
  * [x] 1-Click Alert
  * [x] 1-Click Search
  * [x] 定期チェック機能 - 通知先へ送るスクリーンショットの定期取得
* [x] 自動化とインサイト
  * [x] [**WebhookエンドポイントでシナリオIDの有効化**](https://app.gitbook.com/o/1bWl1a6t3MA8rgLDH3HU/s/2PzA1fb3Iusw0nIBuaxX/\~/changes/3/overview/rirsunto/web-ui-and-backend/web-ui-backend-kaibu/web-ui-and-backend-pre-ga/rirsunto-v07x) **-**:tada:
  * [ ] Triage room
    * [ ] Clipper
  * [ ] オンプレミス接続
    * [ ] PITWALL 専用 IP の払出し
    * [ ] CloudFlare&#x20;
* [x] イベントログ & インサイト
  * [x] PIN、タグ、コメント機能
  * [x] PITWALL AI (コンピューター ビジョン / チャート分析)
    * [x] 相似分析 (カラーベース分析)- :tada:
    * [x] テキスト分析 - :tada:
    * [ ] ベースライン機能
    * [ ] アノマリー検知
  * [x] Snapview
    * [x] スナップショット再取得 :tada:
* [x] Debrief
  * [x] イベントログ
    * [x] アラートログ&#x20;
    * [x] オンデマンド検索時の検索ログ （ブラウザ拡張機能） :tada:&#x20;
  * [x] PIN、タグ、コメント機能
    * [x] 検索レベル
    * [x] イベントレベル
    * [x] PIN、タグ、コメント機能によるイベント検索 :tada:
  * [x] アノテーション :tada:
    * [x] 囲み線 :tada:
    * [x] コメント:tada:
    * [x] 矢印 :tada:
  * [ ] Studioへのフィードバック
* [x] アセット
* [x] PITWALL ダッシュボード
  * [x] アセット登録
  * [x] 日時コマンダ
  * [x] キーコマンダー
  * [x] リサイズ機能

## セキュリティ ＆ スケーラビリティ

* [x] RBAC
* [ ] MFA
* [ ] SSO / SAML
* [ ] リテンション期間の設定

## プラグイン ＆ 拡張機能

{% tabs %}
{% tab title="アラートスキーマ" %}
（アラート送信元）監視ツールのサポート対象範囲の拡大

オープンソース コミュニティの"**Open Alert**"による駆動

* [ ] "Open Alert Project"の開始
* [x] AWS SNS (Simple Notification Service)
* [x] Backlog
* [x] Coralogix
* [ ] Cisco AppDynamics
* [ ] Cisco ThousandEyes
* [x] Datadog
* [ ] Dynatrace
* [ ] Google Monitoring
* [x] Grafana
* [ ] IBM Instana
* [x] Mackerel
* [x] New Relic
* [x] PagerDuty
  * [x] V1
  * [x] V2
  * [x] V3
* [ ] Splunk
* [x] Splunk Oncall (VictorOps)
* [ ] Zabbix
* [x] General Parser
  * [x] OpsRamp
{% endtab %}

{% tab title="送信先" %}
PITWALLにて統合された情報の送信先サポート範囲の拡大

* [x] Slack
* [x] MS Teams :tada:
* [x] Email :tada:
* [ ] Webhook
* [ ] Opsgenie
* [ ] Jira
* [ ] Miro
{% endtab %}

{% tab title="ブラウザ Ext." %}
スナップショット

* [x] シングル / マルチサイト :tada:
* [x] 検索ログ :tada:

サポート対象の拡大

* [x] Chrome 拡張機能
* [ ] MS Edge
* [ ] Firefox

AppStoreへの公式リリース

* [ ] Chrome 拡張機能
* [ ] MS Edge
* [ ] Firefox
{% endtab %}

{% tab title="拡張機能" %}

{% endtab %}
{% endtabs %}

## オープンソースプロジェクト

<details>

<summary>オープンアラート</summary>

SaaS、ホスト型オープンソースおよびプロプライエタリソフトウェア、または自社開発ツールを含む、組織内のさまざまなツールスタックを横断的によりよい標準化をします。このプロジェクトでは、すべての組織がより簡単な方法で利用したいと考えている情報に対し、ツールそれぞれが異なる名前を付けてしまう、現状のそのような課題に対処します。

プロジェクト開始 - CQ4 / 2022.

</details>

<details>

<summary>WebQL (オープンWebクエリ)</summary>

私たちは Web & API生態系の中にいます。今日では誰もが目にするようなサイト。たとえば、日付、空港、ホテル名などがURLクエリとして実装され、自分で旅行計画を立てられる予約サイトなど。これは誰にとっても簡単に共有、拡張、カスタマイズできるものです。このプロジェクトは、単一のURLからいかにして見たいものを取得するかというモーメントを加速させるために開始されました。

プロジェクト開始 - Q1, 2023

</details>

## コンプライアンス

* [ ] SOC2
* [ ] GDPR
* [ ] ISO27001
* [ ] ISO27017
* [ ] HIPPA
