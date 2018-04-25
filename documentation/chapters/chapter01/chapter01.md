# 第1章

## 画像の埋め込み
### 基本形(URL指定)
リポジトリ内の相対URLを指定することができる。また画像表示が無効である(または遅延している)場合の代替テキストを指定できる。
```
![URL指定した写真](../../figures/photos/photo0001-Shioiri-Manhole.png)
```
![URL指定した写真](../../figures/photos/photo0001-Shioiri-Manhole.png)

### 基本形(ID指定)
URLにIDを付与し、IDで指定することもできる。
```
[photo0001]:../../figures/photos/photo0001-Shioiri-Manhole.png
![ID指定した写真][photo0001]
```
![ID指定した写真][photo0001]

### 縮小方法(サムネイル方式)
サイズの大きな画像については、サムネイルとなる縮小した画像を別途作成し、元画像へのリンクとして設定することができる。
```
[photo0001]:../../figures/photos/photo0001-Shioiri-Manhole.png
[photo0002]:../../figures/photos/photo0001-Shioiri-Manhole-small.png
[![拡大表示可能な写真][photo0002]][photo0001]
```
[![拡大表示可能な写真][photo0002]][photo0001]

### 縮小方法(誤り)
画像サイズの調整方法として、使用可能と言われている下記の書式はGitHubでは適用されない。
```
![写真1](../../figures/photos/photo0001-Shioiri-Manhole.png =300x100)
```
![写真1](../../figures/photos/photo0001-Shioiri-Manhole.png =300x100)
```
![写真1](../../figures/photos/photo0001-Shioiri-Manhole.png | width=300)
```
![写真1](../../figures/photos/photo0001-Shioiri-Manhole.png | width=300)

### 縮小方法(非推奨)
表形式で複数の画像を埋め込むことで縮小は可能だが、画像サイズの調整のために表組として意味をなさない記述はすべきではない。
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
