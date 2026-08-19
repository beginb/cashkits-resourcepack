# CashKits Resource Pack

Public asset host for the CashKits Minecraft server. No plugin code or server details live here -- just the packaged resource pack zip, rebuilt and re-uploaded whenever the pack changes.

Currently:
- Custom worn-armor and weapon textures for the VoidGuard crate-exclusive set -- helmet/chestplate/leggings/boots (a real `minecraft:equippable` asset, not a material texture override) plus a matching sword and pickaxe icon. Gracefully degrades to plain netherite for anyone who hasn't accepted the pack.
- Colored tooltip borders for the `/stocks` Exchange GUI (a real `minecraft:tooltip_style` data component per item -- gracefully degrades to the default vanilla purple tooltip border for anyone who hasn't accepted the pack).
- Ember strand sprites for the Apex Aura (`/aura`) -- custom-textured `ItemDisplay` billboards on a `Material.PAPER` carrier, routed via `assets/minecraft/items/paper.json`'s `minecraft:select`/`custom_model_data` string cases. Gracefully degrades to plain paper icons for anyone who hasn't accepted the pack.
- A void-purple icon for the VoidGuard Bot Egg (shop item), routed via `assets/minecraft/items/egg.json`'s `minecraft:select`/`custom_model_data` case. Gracefully degrades to the plain vanilla egg icon for anyone who hasn't accepted the pack, and for any other real egg use.

Source/generators (private `cashevent` repo):
- `tools/generate_voidguard_armor.py`
- `tools/generate_voidguard_icons.py`
- `tools/generate_voidguard_weapons.py`
- `tools/generate_exchange_tooltips.py`
- `tools/generate_aura_textures.py`
- `tools/generate_bot_egg_texture.py`
