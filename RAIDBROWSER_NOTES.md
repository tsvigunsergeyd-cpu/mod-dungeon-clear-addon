# Changes on top of jrad7/mod-dungeon-clear

Three commits on top of `origin/master` (`7f63c22`). **These changes need the `raidbrowser-bots` branch of [mod-playerbots-raidbrowser](https://github.com/tsvigunsergeyd-cpu/mod-playerbots-raidbrowser)**, otherwise the module will not compile.

- `af77f6f`: dungeon queue fill no longer depends on the `DungeonClear.Enable` master switch; it uses only its own `DungeonQueueFill.Enable`.
- `41fe50c`: when the tank in the group is a raid-browser bot, the addon and `.dc` commands can be used only by the raid owner and GMs. Status and boss list stay open to everyone.
- `d5130ff`: bot provisioning now calls `PlayerbotFactory::PrepareBotForContent` instead of preparing step by step. This adds consumables.

**Not verified in game:** the module after `d5130ff`, and the addon permissions (needs a second account).
