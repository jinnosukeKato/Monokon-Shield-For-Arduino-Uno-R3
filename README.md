# Monokon-Shield for Arduino Uno R3

ものづくりコンテスト制御の対象基板、制作基盤と Arduino Uno R3 を接続するためのシールドです

[KiCad 6.0](https://www.kicad.org/) 用のデータです  
ガーバーファイルとドリルファイルを出力して、基板メーカ等に発注するなりしてください

![参考画像](https://github.com/jinnosukeKato/Monokon-Shield-For-Arduino-Uno-R3/blob/master/reference.png)

## 特徴

- Arduino Uno R3 と同寸法
- デバッグ用LED搭載
- 一層基板

## 使いかた

この基盤をArduino Unoに差し込み、CN3に制作基盤(当日制作する基板)を接続し、CN1, CN2に制御対象基板を接続してください。

## 必要な部品

- [330Ω 抵抗器](https://akizukidenshi.com/catalog/g/gR-25331/) x3
- [10kΩ 抵抗器](https://akizukidenshi.com/catalog/g/gR-25103/) x3
- [C1815 トランジスタ](https://akizukidenshi.com/catalog/g/gI-06475/) x3
- [お好きな色のLED](https://akizukidenshi.com/catalog/g/gI-11333/) x3
- [10ピン ボックスヘッダ](https://akizukidenshi.com/catalog/g/gC-12664/) x2
- [2.54mm ピンヘッダ](https://akizukidenshi.com/catalog/g/gC-00167/)

## 組み立て上の注意点

- ランドが少し小さいです
- J1-4はピンが裏を向くように実装してください
- トランジスタの足は、ランドに適切に刺さるよう曲げてください
- CN1, CN2のフラットケーブルが交差してしまう配線になっています
- CN1, CN2が参考画像では10ピンヘッダになっていますが、ボックスヘッダを実装することをオススメします
- CN1, CN2にボックスヘッダを実装する場合は▼がLED側に来るように実装してください
- シルクに`神奈川工業高校 ものづくり同好会`と入ってます

## ピン対応表

| Arduinoのピン | 接続先 | メモ |
| --- | --- | --- |
| 0 | NC | - |
| 1 | NC | - |
| 2 | 7セグ左ON/OFF | - |
| 3 | 7セグ右ON/OFF | - |
| 4 | ブザー | tone()で鳴らしてください |
| 5 | クロック | DCモーター/ステッピングモーター使用時に入力必須 |
| 6 | 7セグ/ステッピング | 7セグのピンは一番上の横棒から時計回り |
| 7 | 7セグ/ステッピング | - |
| 8 | 7セグ/ステッピング | - |
| 9 | 7セグ/ステッピング | - |
| 10 | 7セグ/DCモーター | - |
| 11 | 7セグ/DCモーター | - |
| 12 | 7セグ | 中央横棒 |
| 13 | 7セグ | 小数点 |
| 14 | 製作基盤入力 | digitalRead用 |
| 15 | 製作基盤入力 | digitalRead用 |
| 16 | 製作基盤入力 | digitalRead用 |
| A0 | 製作基盤入力 | AnalogRead用 |
| A1 | 製作基盤入力 | AnalogRead用 |
| A2 | 製作基盤入力 | AnalogRead用 |

## Special Thanks

- K先輩(Arduino MEGA用の基盤データ提供、LEDの回路を参考にさせてもらいました)
- 神奈川工業高校ものづくり同好会
