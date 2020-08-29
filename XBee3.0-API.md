# 概要
XBeeを使用して複数モジュールによる双方向通信を行うことを目的として実験を行った。その結果を備忘録兼、今後の資料として残す。

# 環境
- Windows 10
- XCTU
  - Version: 6.5.1
- XBee3.0 モジュール
  - Product family: XB3-24
  - Function Set: Digi XBee3 Xigbee3.0 TH
  - Firmware version: 100A

今回はコーディネーター1つとルーター2つを使用した。

# XBeeモジュールの設定
以下に、デフォルトから変更した項目と主な項目を示す。
|項目|コーディネーター|ルーター１|ルーター２|
|:--:|:--:|:--:|:--:|
|CE<br>Device Role|From Network[1]|Join Network[0]|Join Network[0]|
|ID<br>Extended PAN ID|123|123|123|
|DH<br>Destination Address High|0|0|0|
|DL<br>Destination Address Low|FFFF|0|0|
|AP<br>API Enable|API Mode Without Wscapes[1]|API Mode Without Wscapes[1]|API Mode Without Wscapes[1]|

