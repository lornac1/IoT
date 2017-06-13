---

copyright:
  years: 2016, 2017
lastupdated: "2016-10-16"

---

{:new_window: target="blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}

# ユーザー役割のアクセス・レベル

デフォルトのユーザー役割のそれぞれのアクセス・レベルを、以下の表に示します。

表には、以下のものについてのアクセス・レベルが示されています。
- [デバイス操作](#user-device-ops)
- [ログ操作](#user-log-ops)
- [キャッシュ操作](#user-cache-ops)
<!-- [Historian Operations](#user-historian) -->
- [組織操作](#user-org-ops)
- [アクセス制御操作](#user-access-ops)
- [分析操作](#user-analytics-ops)
- [サード・パーティー操作](#user-third-party)  
<!-- - [Risk Management Operations](#user-risk-mgt) -->

## ユーザー役割アクセス権{: #user-roles}

### デバイス操作{: #user-device-ops}

デバイス操作 ||| ユーザー役割|||
:--------: | -------------|-------------|---------------|-----|---
           | **管理者** | **オペレーター** | **開発者** | **アナリスト** | **リーダー**
デバイスの作成、更新、または削除 | X | X | X | - | -
デバイスの表示 | X | X | X | X | X
デバイスのアクティブ化 | X | X | X | - | -
イベントのパブリッシュ | - | - | - | - | -
イベントへのサブスクライブ | X | X | X | X | X
コマンドのパブリッシュ | X | X | X | - | -
コマンドのサブスクライブ | - | - | - | - | -
デバイス管理アクションの開始 | X | X | X | - | -
デバイス管理アクションの表示 | X | X | X | X | X
デバイス管理アクションのクリア | X | X | X | - | -
デバイス管理アクション・バンドルの管理 | X | X | X | - | -
デバイス・タイプの作成、更新、削除 | X | X | X | - | -
デバイス・タイプの表示 | X | X | X | X | X
診断ログの管理 | X | X | X | - | -
診断ログの表示 | X | X | X | - | -

### ログ操作{: #user-log-ops}

ログ操作 ||| ユーザー役割|||
:--------: | -------------|-------------|---------------|-----|---
           | **管理者** | **オペレーター** | **開発者** | **アナリスト** | **リーダー**
サーバー・ログの表示 | X | X | X | X | X

### キャッシュ操作{: #user-cache-ops}

キャッシュ操作 ||| ユーザー役割|||
:--------: | -------------|-------------|---------------|-----|---
           | **管理者** | **オペレーター** | **開発者** | **アナリスト** | **リーダー**
稼働中データ (イベント・キャッシュ) の表示 | X | X | X | X | X
稼働中データ (イベント・キャッシュ) の管理 | X	| X | X |	X	| -

### 組織操作{: #user-org-ops}

組織操作 ||| ユーザー役割|||
:--------: | -------------|-------------|---------------|-----|---
           | **管理者** | **オペレーター** | **開発者** | **アナリスト** | **リーダー**
ストレージ・パラメーターの構成|	X| - |-|-|-
認証プロバイダーの構成|	X|-|-|-|-
メール構成の作成、表示、更新、削除	|X|-|-|-|-				
使用可能 IoTP メール・プロバイダーの表示	|X|	X|-|-|-
メール・テンプレートの作成、表示、更新、削除	|X	|X	|-|-|-
ユーザーの作成、更新、削除	|X|	X|-|-|-
ユーザーの表示	|X|	X|	X|	X|-
ユーザー送信勧誘の作成、更新、削除|	X	|X	| -|-|-
ユーザー送信勧誘の表示	|X	|X	|- |- |-
送信勧誘の完了	|X|	X|	X|	X|	X
API キーの作成、更新、削除	|X	|X	| -|-|-
API キーの表示	|X	|X	|- |- |-
ORG 使用情報の表示	|X	|X	| -|-|-		

### アクセス制御操作{: #user-access-ops}

アクセス制御操作 ||| ユーザー役割|||
:--------: | -------------|-------------|---------------|-----|---
           | **管理者** | **オペレーター** | **開発者** | **アナリスト** | **リーダー**
ユーザー・プロパティーの表示 (アクセス権を含む)	|X|	X|	X|	X| -
ユーザー独自のプロパティーの表示 (アクセス権を含む)	|X|	X|	X|	X|	X
ユーザーの管理 (アクセス権を含む)	|X	|X	|-|-|-
API キー・プロパティーの表示 (アクセス権を含む)|	X|	X|	X|	X|-
API キー独自のプロパティーの表示 (アクセス権を含む)	|-|	-|	-| -| -
API キーの作成、更新、削除 (アクセス権を含む)	|X	|X	|-|-|-
デバイス・プロパティーの表示 (アクセス権を含む)	|X|	X|	X|	X|	X
デバイス独自のプロパティーの表示 (アクセス権を含む)	|-	|- |- |- |-
デバイスの作成、更新、削除 (アクセス権を含む)	|X|	X|	X|	-| -
役割の表示	|X	|X	|X	|X	|X
カスタム役割の作成、更新、削除	|X	|X |- |- |-
操作の表示*	|X	|X	|X	|X	|X

### 分析操作{: #user-analytics-ops}

分析操作 ||| ユーザー役割|||
:--------: | -------------|-------------|---------------|-----|---
           | **管理者** | **オペレーター** | **開発者** | **アナリスト** | **リーダー**
分析ルールの表示|	X|	X|	X|	X|	X
分析ルールの管理|	X|	X|	X|	X| -
分析アクションの表示|	X|	X|	X|	X|	X
分析アクションの管理|	X|	X|	X|	X| -
分析アラートの表示|	X|	X|	X|	X|	X
分析メッセージ・スキーマの表示|	X|	X|	X|	X|	X
分析メッセージ・スキーマの管理|	X|	X|	X|	X| -

### サード・パーティー・サービス操作{: #user-third-party}

サード・パーティー・サービス操作 ||| ユーザー役割|||
:--------: | -------------|-------------|---------------|-----|---
           | **管理者** | **オペレーター** | **開発者** | **アナリスト** | **リーダー**
外部プラットフォームからのバッチ通知の処理	|X|	X	|X |-|-
バッチ通知の処理と外部プラットフォームへの送信	|X|	X	|X| -| -
デバイスのイベントのパブリッシュ	|X|	X	|X|	- |-
デバイスからイベントへのサブスクライブ	|X	|X	|X |-| -
外部プラットフォームのコールバック URL の設定	|X	|X	|X|	-| -
外部プラットフォームのサブスクリプション・レベルの設定|	X|	X|	X |- |-
コネクターからの状況ヘルス状況の取得	|X|	X	|X	|- |-
外部システムが稼働しているかどうかの確認と資格情報の検証	|X	|X|	X	|- |-