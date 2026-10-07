# ChatToPod

![ChatToPod](assets/logo.png)

会話で「音声にして」と頼むと、自分の知りたい話をポッドキャストにできます。仕事の資料、本の原文、調べた結果、講義資料を渡し、知りたい切り口を伝えてください。Claudeが原稿と章立てを作り、ChatToPodが日本語の一人語りの音声にします。

会話内で原稿を読み、完成した章から聴けます。倍速の変更、章ごと・全体のMP3の保存にも対応しています。作成には接続したアカウントの利用時間が必要です。18歳以上の方が利用できます。

## Claudeに追加

1. Claudeの「カスタマイズ」→「プラグイン」→「追加」→「プラグインをアップロード」を開きます。
2. `chattopod-claude-plugin.zip`を選びます。
3. ChatToPodの「コネクタ」で接続します。

接続先はパッケージに含まれています。URLやAPIキーの入力は不要です。接続許可後、会話で「この資料をもとに、自分の仕事に関係する話をポッドキャストにして」と頼めます。

公式ディレクトリへの掲載は申請・審査・公開の後です。このパッケージの配布や個人アカウントへの追加は、掲載の承認を意味しません。会話内プレーヤーはClaudeのチャットで使います。CoworkとClaude Codeでも同じスキルと接続を利用できますが、各画面の表示機能は異なります。

## 接続とデータ

OAuthで音声の作成と本人の音声の読み取りを許可します。初回の匿名接続には30分の枠があり、継続利用にはGoogleまたはAppleログインと有料契約が必要です。Googleログインだけでは枠は増えません。

原稿はGoogle Geminiの音声生成APIへ送ります。原稿と音声はCloudflareの非公開保存領域に保管し、接続した本人だけが取得できます。WebはVercel、支払いはStripeを使います。会話全体を取り込む機能はありません。ツールの引数として渡した原稿・章名だけを音声化します。保存期間、退会時の削除、利用者の権利はプライバシーポリシーをご確認ください。

停止は未開始の生成を対象にします。処理中の生成の中断は保証しません。画面ロック中の継続再生と章の切り替えは、会話サービスと端末によって異なります。

## About

ChatToPod creates a personal Japanese podcast from material you choose in your conversation. Ask for the perspective you need: understand a work document, hear an original text you are permitted to use, catch up on research during your commute, or get an explanation of lecture notes. The plugin includes the workflow and its authenticated connector. No API key or server address needs to be entered by the user. Audio generation requires available usage time, and the service is for users aged eighteen and over.

[ホームページ](https://chattopod.com) · [お問い合わせ](https://chattopod.com/support.html) · [プライバシー](https://chattopod.com/legal/privacy.html) · [利用規約](https://chattopod.com/legal/terms.html)

Publisher: Boson. License: Proprietary. Service use is governed by the linked terms. This package contains no server source, private credentials, or user recordings.
