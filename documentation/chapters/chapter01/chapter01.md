# 第1章：画像の埋め込み
---
## 使用可能な書式
### URL指定(相対パス可)
リポジトリ内の相対URLを指定することができる。また画像表示が無効である(または遅延している)場合の代替テキストを指定できる。
```
![URL指定した写真](../../figures/photos/photo0001-Shioiri-Manhole-smallest.png)
```
![URL指定した写真](../../figures/photos/photo0001-Shioiri-Manhole-smallest.png)

### ID指定
URLにIDを付与しIDで指定することができる。IDの定義は、参照の前後いずれでもよく、定義文自体が表示されることはない。同一の画像を複数個所で参照する場合、あるいは本文の可読性を保ちつつ画像への参照を分離する場合に有用である。
```
![ID指定した写真][photo0001]
[photo0001]:../../figures/photos/photo0001-Shioiri-Manhole.png
```
![ID指定した写真][photo0001]

## 画像サイズの調整(縮小)
### サムネイル
サイズの大きな画像については、縮小した画像を別途作成し、元画像へのリンクとしてサムネイル表示することができる。この例では、1500x500サイズである画像に対して300x100サイズのサムネイル画像を設定している。
```
[![拡大表示可能な写真][photo-small]][photo-large]
[photo-large]:../../figures/photos/photo0001-Shioiri-Manhole.png
[photo-small]:../../figures/photos/photo0001-Shioiri-Manhole-small.png
```
[![拡大表示可能な写真][photo0002]][photo0001]

### GitHubでは適用されない記法
画像サイズの調整方法として、使用可能と言われている下記のような「サイズ値を記述する」記法はGitHubでは適用されない。
```
![写真1](../../figures/photos/photo0001-Shioiri-Manhole.png =300x100)
```
![写真1](../../figures/photos/photo0001-Shioiri-Manhole.png =300x100)
```
![写真1](../../figures/photos/photo0001-Shioiri-Manhole.png | width=300)
```
![写真1](../../figures/photos/photo0001-Shioiri-Manhole.png | width=300)

### 使用すべきでない記法
表形式で複数の画像を埋め込むことでも縮小は可能だが、画像サイズの調整のためだけに表組として意味をなさない記述はすべきではない。※画像の羅列を意図して表組とする場合には有用と思われる。
```
|列1|列2|
|-|-|
|![写真1][photo0001]|![写真1][photo0001]|
```
|列1|列2|
|-|-|
|![写真1][photo0001]|![写真1][photo0001]|

<!-- URLの参照先 -->
[photo0001]:../../figures/photos/photo0001-Shioiri-Manhole.png
[photo0002]:../../figures/photos/photo0001-Shioiri-Manhole-small.png
[photo-large]:../../figures/photos/photo0001-Shioiri-Manhole.png
[photo-small]:../../figures/photos/photo0001-Shioiri-Manhole-smallest.png
