# Monokon-Shield for Arduino Uno R3
ものづくりコンテスト制御の対象基板、制作基盤と Arduino Uno R3 を接続するためのシールドです

[KiCad 6.0](https://www.kicad.org/) 用のデータです  
ガーバーファイルとドリルファイルを出力して、基板メーカ等に発注するなりしてください

![参考画像](https://github.com/jinnosukeKato/Monokon-Shield-For-Arduino-Uno-R3/blob/master/reference.png)

## 特徴
- Arduino Uno R3 と同寸法
- デバッグ用LED搭載
- 一応全国大会基板にも対応(デバッグ用LEDなし)

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
- CN1, CN2が参考画像では10ピンヘッダになっていますが、ボックスヘッダを実装することをオススメします
- CN1, CN2にボックスヘッダを実装する場合は▼がLED側に来るように実装してください
