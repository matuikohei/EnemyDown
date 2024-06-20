# Minecraft プラグイン EnemyDown

**開発背景**
---
私は現在、未経験からのエンジニア転職に向けてプログラミングスクールでJavaを学習しています。
このプラグインは、Minecraftのプラグイン開発を通して、Webアプリケーション開発で使用する技術を学習することを目的に作成しました。


**プラグイン概要**
---
「EenemyDown」は、プライヤーが制限時間内に敵を倒してスコアを競うミニゲームです。ゲームの難易度を、easy、nomal、hardから選択することができます。「enemydown」+「難易度」をコマンド入力することでゲームが開始します。ゲーム終了後に、スコアが表示され、スコアはデータベース（MySQL）に保存されます。「enemydown list」とコマンド入力することで、スコアの履歴を確認することができます。


<img width="1440" alt="スクリーンショット 2024-06-20 20 32 49" src="https://github.com/matuikohei/EnemyeDown/assets/135627017/48c82120-6aac-480c-9f6a-1d120ae20219">


<img width="1440" alt="スクリーンショット 2024-06-20 20 34 13" src="https://github.com/matuikohei/EnemyeDown/assets/135627017/58a5d332-6755-400b-a067-78a97b857285">


<img width="1440" alt="スクリーンショット 2024-06-20 20 40 21" src="https://github.com/matuikohei/EnemyeDown/assets/135627017/cfc1ab24-5f36-487a-929a-fe9185e26d06">


<img width="1440" alt="スクリーンショット 2024-06-20 20 33 40" src="https://github.com/matuikohei/EnemyeDown/assets/135627017/63cce96c-8627-45be-b59d-9d1c33cf1e7c">


**主要機能**
---
* ゲーム開始時、体力や空腹ゲージを最大化
* ゲーム開始時、装備や武器を毎回同じものへ変更
* 一定のエリア内でのみ敵が発生
* 敵の種類はランダムに決定
* 敵を倒すと点数が加算
* 敵の種類によって異なる点数を設定
* 時間制限を設定
* 時間制限が来たらエリア内の敵を消滅
* ゲーム開始時と終了時に特殊効果や状態異常を無効化
* ゲーム終了時にスコアボードで合計点数を表示
* スコア、プレイヤー名、日時をデータベース（MySQL）に保存(上書きではなく、全て保存すること)


**プラグイン実装方法**
---
* Java(バージョン17.0.11)のインストール
https://www.oracle.com/java/technologies/downloads/
* Spigot（バージョン1.19.3）のインストール
https://getbukkit.org/
* Minecraft（バージョン1.19.3）のインストール
https://www.minecraft.net/ja-jp
* URLのファイルをダウンロード
https://drive.google.com/file/d/1lvgYwcjXMaafYsV3eEeobxUXBzRPbUjY/view?usp=sharing
* Minecraftフォルダのpluginsフォルダの中に、ダウンロードしたファイルを移動することで、プラグインを実装できます

**使用技術**
---
* Java　17.0.11
* Spigot 1.19.3
* MySQL　8.0
* GitHub
* IntelliJ IDEA
* Gradle
