## Minecraft irányítása Pythonnal

1. Nyiss meg egy új Python ablakot, és írd be a következő kódot:
    
    ```python
from mcpi.minecraft import Minecraft 

mc = Minecraft.create () 

mc.postToChat ("Hello world")
```

2. Futtasd a kódot az `F5` paranccsal és a Minecraft ablakban megjelenik a "Hello világ" üzenet.

3. Add hozzá a következő sorokat a kódodhoz:
    
    ```python
x, y, z = mc.player.getPos () 

mc.setBlock (x + 1, y, z, 1)
```

4. Futtasd a kódot, és megjelenik egy kőblokk a játékosod közelében. Ha nincs előtted, nézegess körbe.

5. Váltsd az `1` -t a `setBlock` sor végén `2`-re:
    
    ```python
mc.setBlock (x + 1, y, z, 2)
```

6. Most egy fűtömbönek kellene megjelennie. Próbáld újra megváltoztatni a számot, és figyeld meg, hogy milyen blokk jelenik meg.

7. Próbáld megváltoztatni a `setBlock`-t `setBlocks`-ra, így egy blokk helyett egy 10x10x10 kockád lesz:
    
    ```python
mc.setBlocks (x + 1, y + 1, z + 1, x + 11, y + 11, z + 11, 1)
```

Most egy nagy kőtömbnek kellene megjelennie!