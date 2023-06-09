# セレクタ

## セレクタとは

コマンドの対象者を絞るコマンドです。使い道としては

- 特定の人だけにコマンドを実行させたい！
- 特定のエンティティだけテレポートさせたい！

などが挙げられます。

## 記法

```
/tp @p ~ ~10 ~
```

@p はプレイヤーを指しています。これがセレクタです。つまり**プレイヤーを 10 ブロック上にテレポートさせる**といった意味になります。

セレクタの一覧は以下の通りです。

- @p プレイヤー
- @s コマンドを実行した本人
- @a 全てのプレイヤー及びエンティティ
- @e エンティティ
- @c エージェント

エンティティはプレイヤーや村人のような存在で基本的にはブロック以外のものが全てそうと思ってもらって大丈夫です。

また@s はコマンドブロックからでは動作しないので注意してください(本人が存在しなくなるため)

## より絞りたい場合

エンティティの中でも村人だけ動作させたい！といった場合は以下のように記述します。

```
/tp @e[type=villager] 100 20 100
```

type はエンティティの種類を表しています。

さらに

```
/tp @e[type=villager,c=1] 100 20 100
```

と書けば
**最もプレイヤーに近い村人のみ**動作します
