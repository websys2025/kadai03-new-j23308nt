## 自動販売機（データ構造と各種処理）のミニレポート
### Q5-1. 自動販売機の商品データついて説明せよ。
* データ構造（各項目とその説明）
id=>    商品番号
name=>  商品名
price=> 商品の価格
stock=> 商品の在庫数
* 連想配列の配列として定義するメリット
各商品を1つのオブジェクトとして簡単に管理できる。
配列として定義することで、商品を検索できる。
### Q5-2. showItemListの処理内容について説明せよ。
* 配列の繰り返し処理
items.lengthを使ってループを制御しています。
* 連想配列の参照方法
items[i]を参照
### Q5-3. buyItemの処理内容について説明せよ。
* 商品購入の可否判定
if (no < 1 || no > items.length)
* 商品在庫を減らす処理
item.stock--
* 商品番号のエラー処理
console.log(no + "は無効な商品番号です。番号は1～8で指定してください。");
### Q5-4. プログラムの考察
* データ構造について
連想配列の配列として管理
* 商品一覧表示と購入処理を関数化したメリット
各商品の情報を一元管理できる
### Q5-5. 感想
* 今回の課題で苦労したこと
jsのエラーは詳しいことがわからないのでどこが間違えているのか探すのに苦労した
* 演習を通して理解できたこと
関数を使って呼び出すとコードを短くできる
* この自動販売機プログラムの追加機能や課題など
どの商品がいくつ売れたか