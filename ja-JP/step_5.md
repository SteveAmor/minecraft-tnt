## TNT

TNTのブロックIDは`46`です。 TNTブロックには2つのタイプがあります：爆発しないTNTブロックと爆発するTNTブロックです。 爆発するTNTブロックが欲しいです。

1. TNTのしっかりした立方体を構築してください。 爆発するTNTブロックを作成するには、`setBlocks`関数の最後に`1`を追加する必要があります。：
    
    ```python
    mc.setBlocks(x+1, y+1, z+1, x+11, y+11, z+11, 46, 1)
    ```

2. TNTブロックの立方体の上に行って、右クリックして剣を突き刺しましょう。 こうすることで、TNTが有効になります。 少し下がって立ち、ショーを見てみよう！
