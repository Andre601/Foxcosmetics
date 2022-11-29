# How to install

## Vanilla

The following installation steps are for servers NOT using ItemsAdder, but a custom resource pack.  

> **Warning**
> 
> The vanilla method uses the `IRON_HORSE_ARMOR` item model with the custom model data values `400001`, `400002`, `400003`, `400004`, `400005` and `400006`.
>   
> You can use the [JSON Merger tool][jsonmerger] from LoneDev to merge an existing `iron_horse_armor.json` with the one provided by this add-on.

1. Download the `Foxcosmetics-Vanilla-v<version>.zip` file from the [Latest release][releases].
2. Open the Zip file.
3. Extract the content of `resource_pack/assets/` and copy it into your resource pack's `assets/` folder.  
    The structure of your resource pack should look like this now:  
    ```
    assets/
    ├── foxcosmetics/
    │   ├── models/
    │   │   └── cosmetic/
    │   │       ├── fox_ears.json
    │   │       ├── fox_tail.json
    │   │       ├── fox_tail_self.json
    │   │       ├── snow_fox_ears.json
    │   │       ├── snow_fox_tail.json
    │   │       └── snow_fox_tail_self.json
    │   └── textures/
    │       └── fox/
    │           ├── fox_ears.png
    │           ├── fox_tail.png
    │           ├── snow_fox_ears.png
    │           └── snow_fox_tail.png
    └── minecraft/
        └── models/
            └── item/
                └── iron_horse_armor.json
    ```
4. Update your resource pack zip file.
5. Extract the `foxcosmetics.yml` file from `cosmeticscore/vanilla/` and copy it into `plugins/CosmeticsCore/cosmetics/`
6. Run `/cosmeticsconfig cosmetics reload`

## ItemsAdder

The following installation steps are for servers using ItemsAdder.

### v3.3.0 and newer

1. Create the `foxcosmetics/configs/` and `foxcosmetics/resourcepack/` folders inside the `contents` folder.
2. Download the `Foxcosmetics-ItemsAdder-v<version>.zip` file from the [latest release][releases].
3. Open the zip file and extract the contents of `resource_pack/assets/` and `itemsadder/data/items_packs/foxcosmetics/`.
    - You should now have two YAML files and a `foxcosmetics/` folder.
4. Move the YAML files into `contents/foxcosmetics/configs/` and the `foxcosmetics/` folder into `contents/foxcosmetics/resourcepack/`.  
    You should now have a folder structure similar to this one in `plugins/ItemsAdder/`:
    ```
    contents/
    └── foxcosmetics/
        ├── configs/
        │   ├── fox_ears.yml
        │   └── fox_tails.yml
        └── resourcepack/
            └── foxcosmetics/
                ├── models/
                │   └── cosmetics/
                │       ├── fox_ears.json
                │       ├── fox_tail.json
                │       ├── fox_tail_self.json
                │       ├── snow_fox_ears.json
                │       ├── snow_fox_tail.json
                │       └── snow_fox_tail_self.json
                └── textures/
                    └── fox/
                        ├── fox_ears.png
                        ├── fox_tail.png
                        ├── snow_fox_ears.png
                        └── snow_fox_tail.png
    ```
5. Update your resource pack by running `/iazip`
    - Depending on your hosting method will you need to update your resource pack URL and run `/iatexture all`.
6. Extract the `foxcosmetics.yml` file from `cosmeticscore/itemsadder/` and copy it into `plugins/CosmeticsCore/cosmetics/`
7. Run `/cosmeticsconfig cosmetics reload`

### v3.2.5 and older

1. Download the `Foxcosmetics-ItemsAdder-v<version>.zip` file from the [Latest release][releases].
2. Open the Zip file.
3. Copy the content of `resource_pack/` into `plugins/ItemsAdder/data/resource_pack/` and the content of `itemsadder/data/items_packs` into `plugins/ItemsAdder/data/items_packs/`  
    You should now have a folder structure similar to this one in `plugins/ItemsAdder/`:
    ```
    data/
    ├── items_packs/
    │   ├── fox_ears.yml
    │   └── fox_tails.yml
    └── resource_pack/
        └── assets/
            └── foxcosmetics/
                ├── models/
                │   └── cosmetics/
                │       ├── fox_ears.json
                │       ├── fox_tail.json
                │       ├── fox_tail_self.json
                │       ├── snow_fox_ears.json
                │       ├── snow_fox_tail.json
                │       └── snow_fox_tail_self.json
                └── textures/
                    └── fox/
                        ├── fox_ears.png
                        ├── fox_tail.png
                        ├── snow_fox_ears.png
                        └── snow_fox_tail.png
    ```
4. Update your resource pack by running `/iazip`
    - Depending on your hosting method will you need to update your resource pack URL and run `/iatexture all`.
5. Extract the `foxcosmetics.yml` file from `cosmeticscore/itemsadder/` and copy it into `plugins/CosmeticsCore/cosmetics/`
6. Run `/cosmeticsconfig cosmetics reload`

[releases]: https://github.com/Andre601/Foxcosmetics/releases/latest
[jsonmerger]: https://itemsadder.github.io/jsonmerger/
