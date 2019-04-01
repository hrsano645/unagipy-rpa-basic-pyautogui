# Unagi.py 勉強会16枚目 LT 

pyautoguiでお手軽業務RPAしてみた

Hiroshi Sano

---

# お前誰よ

- twitter:hrs_sano645

- 本業:自動車プレス金型の設計 [佐野設計事務所](https://sano-design.info)
	- の設計以外の全て担当
- 時々[東海大学 石井研究室](https://ishiilab.net) お手伝い

- 最近は雑務を極力Python（マシン）に投げまくってる

---

# 本業でよくやること

- 機械の設計 -> いろんな部品を扱う
- 3D CADでモデリングする -> 3Dで扱う部品のデータをよく取ってくる

面倒なので自動化したい 

---

# WEB スクレイピングでよくない？

- 大抵はそれでおk
    - 簡易なWEBサイトが結構多いので...
    - selenium-python + webdriver（headless chromeとか）
- そうもいかない場所
    - ActiveXとかはもうないと思います
    - 特殊なプログラムを扱うようなもの(専用のダウンローダーが動くやつ）
    
---

# こういうの面倒

(画像入れる

Clickonceという技術で、WEBでC#のプログラムが動かせるらしいです。割とこういうの多い
WEB scrapingだとそこまでカバーできない

---

# そこでRPAという救世主が！！

---

# RPA(とは

---

# RPA期待高い話多い

[なんと平均約85%の効率化？！自治体のRPA実証実験で驚愕の結果が【iNTERNET magazine Reboot】 - INTERNET Watch](https://internet.watch.impress.co.jp/docs/imreboot/news/1177196.html)


[ Apple、イタリアのRPA企業Stamplayを買収 - ITmedia NEWS](https://www.itmedia.co.jp/news/articles/1903/22/news075.html)


[‪Google トレンドで「ロボティック・プロセス・オートメーション, RPA - すべての国、過去 5 年間」の 人気度の動向 を見る](https://trends.google.co.jp/trends/explore/TIMESERIES/1554083400?hl=ja&tz=-540&date=today+5-y&q=%2Fg%2F11c3p_5fs0,RPA&sni=3‬)


---

# RPAのいいところ悪いところ

いいところ
- 単純に時間の節約につながる
- 作業=コードやフローにできて明文化できる
- 人が関与しなくて良いので品質、信頼性につながる

悪いところ
- 複雑なものを単純にするのは難しい
- マシンでできない作業はできない（印鑑押すとか

---

# pyautogui使ってみた

こちらです -> 

簡単に言うと GUIでの操作をオートメーションするためのライブラリ
---

# pyautoguiの使い方