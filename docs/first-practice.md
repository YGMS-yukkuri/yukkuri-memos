# WindowsPCの使用方法

## 電源をつける

各々DXPCがある場所に座ってもらい、電源を入れる

## デスクトップからVSCodeを起動してもらう

1. デスクトップにあるVSCodeのアイコンをクリックする
2. 新規ファイル作成から、「自分の名前.html」を作成する

## HTMLの基本構造を作る
1. "!"を入力して、Enterを押すと、HTMLの基本構造が自動で作成される。
2. titleのDocumentを時計に書き換える
3. bodyの中にh1タグを作成し、idを「clock」にする

## JSの書き込み

1. scriptタグを作成する
2. scriptタグの中に、setInterval関数を使って、0.1秒ごとに現在時刻を取得し、h1タグの中身を書き換える処理を書く
```javascript
setInterval(() => {
  const clock = document.getElementById("clock");
  const now = new Date();
  clock.textContent = now.toLocaleTimeString();
}, 100);
```
3. Live Serverを起動して、ブラウザで時計が表示されることを確認する

---

### 以下時間あれば

#### CSSの書き込み

1. styleタグを作成し、h1タグの文字色を変える
2. 文字の大きさを変える
```css
h1 {
  color: red;
  font-size: 48px;
}
```
3. box-shadowを使って、文字に影をつける
```css
h1 {
  color: red;
  font-size: 48px;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
}
```
