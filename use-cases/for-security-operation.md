# セキュリティ運用向け

<!--
# 🖥️ セキュリティ運用向け
-->


## Overview

近年の企業のIT運用では、毎日のように新たな脅威を対処しなければなります。セキュリティ製品が以下のような情報を含むアラートを送信する際、セキュリティ チームはそのアラートが疑わしいものと判断した場合、どの程度危険であるかを調査し、証拠を記録として収集する必要があります。

## 種類

* IPレピュテーション
* サイトレピュテーション（マルウェア）
* CVE
* ファイルチェック（ハッシュ）

## 例

上記を確認できる広く使用されている有名なサイトがあります。 以下に例として複数のサイトをまとめて、それらのルックアップを PITWALL Studioで設定する方法も記載しています。 詳細についてはこちらをご参照ください。\
[#create-a-new-ondemand-lookup](../tutorial-get-started./shinariono/insutantorukkuappu/2-ondemandorukkuappu.md#create-a-new-ondemand-lookup "mention")

&#x20; &#x20;

{% tabs %}
{% tab title="IPレピュテーション" %}
<table><thead><tr><th width="152">Site</th><th width="358">PITWALL URL (Parameterized)</th><th>Key sample</th></tr></thead><tbody><tr><td>AbuseIPDB</td><td><a href="https://www.abuseipdb.com/check/202.14.122.217">https://www.abuseipdb.com/check/{$key}</a></td><td>202.14.122.217<br>(This IP is real. Be careful.)</td></tr><tr><td>VirusTOTAL</td><td><a href="https://www.virustotal.com/gui/ip-address/210.209.125.142">https://www.virustotal.com/gui/ip-address/{$key}</a></td><td>210.209.125.142<br>(This IP is real. Be careful.)</td></tr></tbody></table>


{% endtab %}

{% tab title="サイトレピュテーション（マルウェア）" %}
<table><thead><tr><th width="196">Site</th><th>PITWALL URL (Parameterized)</th></tr></thead><tbody><tr><td>URLhaus</td><td><a href="https://urlhaus.abuse.ch/browse.php?search=222.139.79.18">https://urlhaus.abuse.ch/browse.php?search={$key</a>}</td></tr><tr><td>IBM X-Force Exchange</td><td><a href="https://exchange.xforce.ibmcloud.com/url/222.139.79.18">https://exchange.xforce.ibmcloud.com/url/{$key}</a></td></tr></tbody></table>
{% endtab %}
{% endtabs %}