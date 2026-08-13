# CashKits Resource Pack

Public asset host for the CashKits Minecraft server. No plugin code or server details live here -- just the packaged resource pack zip, rebuilt and re-uploaded whenever the pack changes.

Currently (adds sword + pickaxe to the VoidGuard Crate pool):
- Custom worn-armor textures for the VoidGuard crate-exclusive armor set (a real `minecraft:equippable` asset, not a material texture override -- gracefully degrades to plain netherite for anyone who hasn't accepted the pack).
- Colored tooltip borders for the `/stocks` Exchange GUI (a real `minecraft:tooltip_style` data component per item -- gracefully degrades to the default vanilla purple tooltip border for anyone who hasn't accepted the pack).

Source/generators (private `cashevent` repo):
- `tools/generate_voidguard_armor.py`
- `tools/generate_exchange_tooltips.py`
