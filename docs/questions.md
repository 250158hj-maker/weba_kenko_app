## 注意点
- データベースは「管理者」画面で**「セットアップを実行」でDB初期化**できます。
- このアプリの AI処理は Gemini API を利用しています。動作確認するには env.php の GEMINI_API_KEY の設定が必要です。

```env
const GEMINI_API_KEY = 'Google AI Studio で発行した APIキー';
```

## Q. このアプリで利用する**データベース名**はどれですか？

1. mysql
2. 127.0.0.1
3. health_log
4. kenko_log

## Q. ログイン後に**自動的に健康ダッシュボードページに移動する**ことをなんと言いますか？

1. リダイレクト
2. セッション
3. CSR
4. SSR

## Q. 健康ダッシュボードページ（dashboard/）で、データベースとレンダリング処理の説明で正しいのはどれですか？

1. PHPだけで処理している。
2. JavaScriptだけで処理している。
3. データベースはJavaScript、一部PHPでレンダリングしている。
4. データベースはPHP、一部JavaScriptでレンダリングしている。

## Q. 健康管理の一覧ページ（health/）で、データベースとレンダリング処理の説明で正しいのはどれですか？

1. PHPだけで処理している。
2. JavaScriptだけで処理している。
3. データベースはJavaScript、一部PHPでレンダリングしている。
4. データベースはPHP、一部JavaScriptでレンダリングしている。

## Q. トップページの「日々の健康を、もっと楽しく、かんたんに記録。」を表示しているファイルはどれですか？

1. index.php
2. components/nav.php
3. components/message.php
4. components/top/hero_left.php

## Q. アクティビティ記録画面で「種類」が**Warning:** になっています。どのファイルを修正しますか？

1. register/index.php
2. health/index.php
3. activity/index.php
4. exercise/index.php

## Q. そのファイルで、**Waring箇所をどう修正**しますか？

1. $row['type']
2. $row['category']
3. $row['activity_type']
4. $row['exercise_type']

## Q. 健康管理の「健康記録を追加」画面では、登録するとSQLエラーになります。health/add.php の insert() で、SQLの 「xxxx」 の部分はつぎのどれですか？

```php
$sql = "INSERT INTO xxxx (user_id, weight, heart_rate, systolic, diastolic, recorded_at) 
        VALUES (:user_id, :weight, :heart_rate, :systolic, :diastolic, :recorded_at)";
```

1. healths
2. health_records
3. exercises
4. exercise_records

## Q. 健康管理の編集画面では「該当する記録が見つかりません。」のエラーになります。 health/edit.php の $id で正しいのはどれですか？

1. $_GET['id']
2. $_POST['id']
3. $_GET['health_id']
4. $_POST['health_id]

## Q. アクティビティの「アクティビティ記録を追加」画面で、登録すると「不正なリクエストです。」のエラーになります。なぜですか？

1. データが未入力で登録している
2. GETリクエストで登録している
3. CSRF によるなりすまし攻撃
4. ユーザセッションが取得できない

## Q. 健康管理ページの「CSVダウンロード」をリクエストするとエラーになります。CSVダウンロードできるようプログラム修正し、CSVの中身をコピー＆ペーストして回答してください。

## Q. 健康管理の「AI分析」を実行するとエラーになります。js/health_ai.js の API URLを修正してAI分析してください。回答は、AI履歴で**CSVダウンロードしたファイルの中身をコピー＆ペースト**してください。

## Q. アクティビティの「アクティビティグラフ」はAPIエラーでグラフ表示できません。js/activity_chart.js の API URLを修正してグラフ表示してください。回答は**ダウンロードした画像をアップロード**してください。