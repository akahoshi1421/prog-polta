# tp

## tpとは
特定の座標にテレポートするコマンドです。使い道としては

- ステージをクリアしたので次のステージにテレポートさせたい！
- エージェントを次のステージにテレポートさせたい！

などが挙げられます。

## 記法

```
/tp セレクタ x y z 向き(横) 向き(縦)
```
このように記述することで特定の座標にテレポートできます。また向きは省略可能です。

セレクタの意味関しては[こちら](/command/selector)で説明しています。

例えば

```
/tp @p ~ ~10 ~
```

と記述すれば**10ブロック上にテレポートします**。