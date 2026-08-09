# Guitar Chord v0.0.16

BBC micro:bit V2 専用の MakeCode 拡張機能です。

## ボタン入力
- ボタン1 = P1
- ボタン2 = P2
- ボタン3 = P9

MakeCode のブロックでは、ピン番号ではなく「ボタン1」「ボタン2」「ボタン3」と表示されます。

例：

```typescript
guitarchord.assignChord(guitarchord.ChordButton.Button1, guitarchord.Chord.C)
guitarchord.assignChord(guitarchord.ChordButton.Button2, guitarchord.Chord.G)
guitarchord.assignChord(guitarchord.ChordButton.Button3, guitarchord.Chord.Am)
```

ブロック表示：
- ボタン1 に和音 C を割り当てる
- ボタン2 に和音 G を割り当てる
- ボタン3 に和音 Am を割り当てる

各スイッチは対応する入力ピンと GND の間に接続します。内部プルアップを使用します。

## 音声出力
- P8 = 出力1
- P14 = 出力2
- P16 = 出力3

## 登録コード
A, A7, Aadd9, Am, Am7, AM7, Asus4,
B7, B♭, Bm, Bm7-5,
C, C7, Cadd9, Cdim, Cm, CM7, Csus4, C♯m7-5,
D, D7, Dm, Dm7, Dsus4, D/F♯,
E, E7, Em, Em7, Esus4,
F, Fm, FM7, Fsus4, F♯dim, F♯m,
G, G7, Gadd9, Gsus4

7th / add9 / m7 など本来4音のコードは、3出力用に3音へ省略しています。

## アイコン
拡張機能の選択画面用に `icon.png` を同梱しています。
※ MakeCode のブロックカテゴリ内の小さな白い記号は Font Awesome アイコン指定であり、任意画像には置き換えできません。

## カテゴリ表示 v0.0.8
- カテゴリ色：黄色系 `#F2B705`
- カテゴリアイコン：スピーカー（Font Awesome `volume-up`, `\uf028`）

## v0.0.12 カテゴリアイコン
Font Awesome 4 の headphones (Unicode f025) を使用。カテゴリ色は #F2B705。


## v0.0.15
カテゴリのアイコンを volume-up (`\uf028`) に戻しました。


## v0.0.16
カテゴリ表示名を `Guitar Chord` に変更しました。


## v0.0.17
MakeCodeのカテゴリ更新を確実にするため、TypeScript namespace を `guitarchord` に変更しました。


## v0.0.18
サムネイル画像（icon.png）は同梱していません。
