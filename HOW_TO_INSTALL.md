# How to install

## Vanilla

The following installation steps are for servers NOT using ItemsAdder, but a custom resource pack.  

> **Warning**
> 
> The vanilla method uses the `IRON_HORSE_ARMOR` item model with the custom model data values `400001`, `400002`, `400003`, `400004`, `400005` and `400006`.  
> When you merge the assets of this addon into your resource pack, make sure that there isn't an existing `iron_horse_armor.json` file with the above values.

1. Download the `Foxcosmetics-Vanilla-v<version>.zip` file from the [Latest release][releases].
2. Open the Zip file.
3. Extract the content of `resource_pack/` and copy it into your resource pack's `assets/` folder.  
    The structure of your resource pack should look like this now:  
    ```
    assets/
     |
     |- foxcosmetics/
     |   |
     |   |- models/
     |   |   |
     |   |   |- cosmetic/
     |   |       |
     |   |       |- fox_ears.json
     |   |       |- fox_tail.json
     |   |       |- fox_tail_self.json
     |   |       |- snow_fox_ears.json
     |   |       |- snow_fox_tail.json
     |   |       |- snow_fox_tail_self.json
     |   |
     |   |- textures/
     |       |
     |       |- fox/
     |           |
     |           |- fox_ears.png
     |           |- fox_tail.png
     |           |- snow_fox_ears.png
     |           |- snow_fox_tail.png
     |
     |- minecraft/
         |
         |- models/
             |
             |- item/
                 |
                 |- iron_horse_armor.json
    ```
4. Update your resource pack file.
5. Extract the `foxcosmetics.yml` file from `cosmeticscore/vanilla/` and copy it into `plugins/CosmeticsCore/cosmetics/`
6. Run `/cosmeticsconfig cosmetics reload`

## ItemsAdder

The following installation steps are for servers using ItemsAdder.

1. Download the `Foxcosmetics-ItemsAdder-v<version>.zip` file from the [Latest release][releases].
2. Open the Zip file.
3. Copy the content of `resource_pack/` into `plugins/ItemsAdder/data/resource_pack/` and the content of `itemsadder/data/items_packs` into `plugins/ItemsAdder/data/items_packs/`  
    You should now find the following structures inside `plugin/ItemsAdder/`:  
    ```
    data/
     |
     |- items_packs/
     |   |
     |   |- foxcosmetics/
     |       |
     |       |- fox_ears.yml
     |       |- fox_tails.yml
     |
     |- resource_pack/
         |
         |- assets/
         |
         |- foxcosmetics/
             |
             |- models/
             |   |
             |   |- cosmetic/
             |       |
             |       |- fox_ears.json
             |       |- fox_tail.json
             |       |- fox_tail_self.json
             |       |- snow_fox_ears.json
             |       |- snow_fox_tail.json
             |       |- snow_fox_tail_self.json
             |
             |- textures/
                 |
                 |- fox/
                     |
                     |- fox_ears.png
                     |- fox_tail.png
                     |- snow_fox_ears.png
                     |- snow_fox_tail.png
    ```
4. Update your resource pack by running `/iazip`
    - Depending on your hosting method will you need to update your resource pack URL and run `/iatexture all`.
5. Extract the `foxcosmetics.yml` file from `cosmeticscore/itemsadder/` and copy it into `plugins/CosmeticsCore/cosmetics/`
6. Run `/cosmeticsconfig cosmetics reload`