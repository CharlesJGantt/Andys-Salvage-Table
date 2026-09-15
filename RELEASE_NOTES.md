# Andy's Salvage Table 0.7.17

Maintenance release. **Fixes the crafting recipe**, which never produced a Salvage Table: the pattern spelled the Stonecutter `minecraft:stonecutter`, but Bedrock's actual id for it is `minecraft:stonecutter_block`. All nine slots filled correctly and the output stayed empty. The block could only be obtained from the creative menu.

No other change — no balance, no behavior, no settings. Placed tables keep everything.

Everything below describes the add-on as a whole.

## What it does

A Salvage Table reverses crafting. Put a crafted item in, see exactly what you will get back, and take it. What comes back is drawn from Minecraft's own crafting recipes — **909 of them** — so a Chest returns planks and a Diamond Pickaxe returns diamonds and a stick, minus a share lost in the breaking down and less again if the item is damaged.

## Highlights

- **See the trade before you take it.** The nine material slots show the real stacks at the real counts. Nothing is consumed until you take one, so you can price an item and take it straight back out.
- **Honest arithmetic.** Recovery is a percentage of the original recipe, scaled by durability, and can never exceed what the recipe took. Sixteen Glass Panes came from six Glass, so one pane never returns one Glass.
- **Never half-done.** The whole result is checked against your inventory before the item is consumed. If it will not fit, nothing happens and the item stays put.
- **Protected by default.** Enchanted, renamed, and container items are refused unless a world owner deliberately allows each one.
- **Full automation.** Containers on four faces feed it, materials leave through the bottom, and refused items leave through a side you choose — so a rejected item can slow a farm but never jam it.
- **Per-machine filters**, six presets, category switches, and item allow/deny lists.
- **Redstone control** in three modes, per machine.
- **Operator menu and full dedicated-server console administration**, with every setting reachable headless.
- **Andy's Disenchanting Pillar integration** — when the Pillar is installed, a refused enchanted item points the player to it.
- Vibrant Visuals/PBR textures, achievement-friendly, no experiments or cheats.

## Notes

- A container **directly below the table is required** for automation.
- Power the table with a repeater or through a solid block. Redstone dust led straight in also powers the hopper beneath it, and a powered hopper stops moving items.
- Items from other add-ons are salvageable only if that add-on adds support for it.

**SHA-256:** `2D11768980E6701E73206CAC7EE02FF3CFBD9C8205FA1550E0C6FD76C7CE0DF1`
