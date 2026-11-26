# M1C0001-microbit-ctrl

micro:bit のコントローラーから、SIYEENOVE の micro:bit カー「M1C0001（Pybit）」を制御するサンプルです。

## ファイル

| ファイル | 内容 |
|---|---|
| `microbit-m1c-controller.hex` | コントローラー側 micro:bit 用プログラム（MakeCode）。ジョイスティックの値を無線（グループ 6）で送信 |
| `microbit-motor-test.hex` | 車側 micro:bit 用プログラム（MakeCode）。無線を受信してモーターを動かす（ファイル名は `motor-test` ですが、走行用の本体プログラムです） |
| `docs/M1C0001_操作説明書.docx` | 操作説明書（Word）。初心者向けに、ダウンロードから走行までを説明 |

## ダウンロード

最新版は [Releases ページ](https://github.com/uchuika/M1C0001-microbit-ctrl/releases/latest) の「Assets」から、2 つの hex ファイルと操作説明書をダウンロードできます（GitHub アカウント不要）。

## 使い方

1. 上記の Releases ページから `.hex` ファイルを 2 つダウンロードします。
2. micro:bit を USB で接続し、`MICROBIT` ドライブに hex ファイルをドラッグ＆ドロップして書き込みます。**コントローラー側**に `microbit-m1c-controller.hex`、**車側**に `microbit-motor-test.hex` を書き込みます（取り違えに注意）。
3. 車側 → コントローラー側の順に電源を入れます。コントローラーに ♥、車に ☺ が表示されれば起動しています。
4. 最初はタイヤを浮かせた状態でジョイスティックを倒し、タイヤが回ることを確認してから走らせます。
5. 中身を確認・編集する場合は [MakeCode](https://makecode.microbit.org/) を開き、「インポート」から hex ファイルを読み込みます。

詳しい手順と安全上の注意は、操作説明書を参照してください。

## 関連リンク（公式）

本リポジトリにはメーカー公式の資料（チュートリアルPDF、アプリ、回路図、サンプルコード）は含まれていません。以下の公式リポジトリを参照してください。

- https://github.com/siyeenove/M1C0001
- https://siyeenove.com

## 免責・商標

"Siyeenove" は Siyeenove Technology Co., Ltd. の登録商標です。本リポジトリは非公式の個人プロジェクトであり、同社とは無関係です。

## ライセンス

[MIT License](LICENSE)
