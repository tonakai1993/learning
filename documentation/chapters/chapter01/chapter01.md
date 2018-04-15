# 第1章

## 画像の埋め込み
### 基本形(URL直接)
```
![写真1](../../figures/photos/photo0001-Shioiri-Manhole.png)
```
![写真1](../../figures/photos/photo0001-Shioiri-Manhole.png)

### 基本形(URL間接)
```
[photo0001]:../../figures/photos/photo0001-Shioiri-Manhole.png
![写真1][photo0001]
```
![写真1][photo0001]

### 縮小方法(方法1)
一部のMarkdownで使用可能とされている下記の書式はGitHubでは適用されない。
```
![写真1](../../figures/photos/photo0001-Shioiri-Manhole.png =100x100)
```

![写真1](../../figures/photos/photo0001-Shioiri-Manhole.png =100x100)

### 縮小方法(方法2)
表形式で複数の画像を埋め込むことで縮小は可能。
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
