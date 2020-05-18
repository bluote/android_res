Androidのres構成について、
https://developer.android.com/guide/topics/resources/available-resources
の記述に従い纏めました。

# Androidアプリで、UIに関わるものは下記のリソースに定義されています。
res/anim/
res/color/
res/drawable/
res/layout/
res/menu/
res/font/
res/values/colors.xml
res/values/dimens.xml
res/values/strings.xml
res/values/styles.xml


# 各リソースの役割を下記に纏めました。
## res/anim/
アニメーションリソースはres/anim/ に保存します。

## res/color/
ビュー(UI)の状態に応じて変わる色のリソースはres/color/ に保存します。

## res/drawable/
ビットマップや XML でさまざまなグラフィックを定義したリソースをres/drawable/ に保存します。
例えば、よく使われる
・png/jpeg/gif等
・状態リスト(StateListDrawable)⇢ビュー(UI)の状態に応じて、同一のグラフィックに異なる画像を使用することができます。
・色やグラデーションなどを含む幾何学的図形

他は
レイヤリスト(LayerDrawable)、レベルリスト(LevelListDrawable)、スケール ドローアブル(ScaleDrawable)などのリソースもここで保存します。

## res/layout/*.xml
アプリ UI のレイアウトを定義します。

## res/menu/
アプリメニューの内容を定義したリソースはres/menu/ に保存します。

## res/font/
アプリ内で使用できるカスタム フォントはres/font/ に保存します。

## res/values/colors.xml
色コードを定義するリソースです。 色コードに名前をつけて管理することが可能になります。
※res/color/*.xmlには状態に応じて変わる色を定義すると違い、ここで色の固定値をここで定義する

## res/values/dimens.xml
dp、spなどのサイズ数値を定義するリソースです。

## res/values/strings.xml
UIで使用する定型文などを定義するリソースです。
多言語対応にも利用される
 res/values-en/strings.xml（英語）
 res/values-ja/strings.xml（日本語）

## res/values/styles.xml
UI の形式と外観を定義するリソースです。
個々の View に適用することも、Activity 全体やアプリ全体に適用することもできる
