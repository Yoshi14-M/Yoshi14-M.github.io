# 松井 義朗 ポートフォリオ

PHP / Laravel のバックエンドエンジニア、松井 義朗（Yoshiaki Matsui）のポートフォリオサイトです。

**サイト：** https://yoshi14-m.github.io/

## 掲載内容

| ページ                         | 内容                                   |
| ------------------------------ | -------------------------------------- |
| トップ（`index.html`）         | 自己紹介・スキル・制作物・開発の進め方 |
| お問い合わせ（`contact.html`） | お問い合わせフォーム                   |

### 制作物

| 制作物               | 区分                                                      | リポジトリ                                                                  |
| -------------------- | --------------------------------------------------------- | --------------------------------------------------------------------------- |
| TrainingMax          | 個人開発（[デモ](https://trainingmax-demo.onrender.com)） | [Yoshi14-M/TrainingMax](https://github.com/Yoshi14-M/TrainingMax)           |
| 勤怠管理アプリ       | 模擬案件                                                  | [Yoshi14-M/attendance-app](https://github.com/Yoshi14-M/attendance-app)     |
| 書籍レビューアプリ   | 模擬案件                                                  | [Yoshi14-M/bookshelf-app](https://github.com/Yoshi14-M/bookshelf-app)       |
| お問い合わせフォーム | 模擬案件                                                  | [Yoshi14-M/contact-form-app](https://github.com/Yoshi14-M/contact-form-app) |

## 使用技術

- **画面**：HTML / CSS / JavaScript（フレームワーク・ビルドツールなし）
- **フォント**：Google Fonts（Noto Sans JP、JetBrains Mono）
- **お問い合わせの受付**：Google Apps Script（ウェブアプリ）＋ Google スプレッドシート
- **公開**：GitHub Pages
- **デザイン**：Figma

## 主な機能

- **日本語・英語の切り替え**：ヘッダーのボタンで切り替えます。選んだ言語はブラウザに保存され、ページを移動しても引き継がれます。
- **スクリーンショットのスライダー**：TrainingMax の画面を、ボタン・ドット・スワイプで切り替えて表示します。
- **レスポンシブ対応**：パソコンとスマートフォンの両方で表示を確認しています。
- **お問い合わせフォーム**
  - 入力内容を画面上でチェックし、エラーを項目ごとに表示します（日本語・英語）。
  - 送信内容は Google Apps Script で受け取り、スプレッドシートへの記録、自分あての通知メール、問い合わせた人への受付完了メールを行います。
  - 受付側でも入力内容をチェックし、送信の成否を画面に返します。
  - ボット対策として、人には見えない入力欄（ハニーポット）を置いています。
  - スプレッドシートで数式として実行されないよう、`=` `+` `-` `@` で始まる値は文字列として記録します。

## ディレクトリ構成

```
.
├── index.html            # トップページ
├── contact.html          # お問い合わせページ
├── favicon.svg           # ファビコン
├── apple-touch-icon.png  # ホーム画面用アイコン（iPhone）
├── ogp.png               # SNS などで共有したときのサムネイル
└── images/               # スクリーンショット・プロフィール写真
```

## ローカルでの確認

ビルドは不要です。リポジトリのフォルダで簡易サーバーを起動し、ブラウザで開きます。

```bash
python3 -m http.server 8000
# http://localhost:8000/ を開く
```

## 作成者

松井 義朗（Yoshiaki Matsui）

- GitHub：[Yoshi14-M](https://github.com/Yoshi14-M)
- お問い合わせ：[お問い合わせフォーム](https://yoshi14-m.github.io/contact.html)
