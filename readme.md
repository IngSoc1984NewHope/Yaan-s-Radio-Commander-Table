# Radio Commander — No Cheat Mode Cheat Engine Table

**Version:** v0.4  
**Status:** All five features tested successfully on the user's current setup.  
**Platform:** Windows x64 / Unity Mono  
**Requirements:** Cheat Engine 7.5 or newer recommended.

## IMPORTANT — Activation Timing / 重要启用说明

**DO NOT enable any cheats until BOTH conditions are met:**

1. **The battle has fully loaded.**
2. **The first in-mission radio communication has been received.**

Only after these two conditions are satisfied should you enable the desired features in Cheat Engine.

**重要：所有功能必须在以下两个条件均满足后才能开启：**

1. **战斗已经完全加载完毕。**
2. **已经收到任务中的第一条无线电通讯。**

请勿在战斗加载过程中或刚进入任务但尚未收到第一条通讯时开启任何功能。

每次进入新战斗或重新加载任务，都应遵守上述顺序。

---

## Features / 功能列表

| Feature | 功能说明 |
|---|---|
| Infinite Ammunition | 友军无限弹药，阻止弹药消耗 |
| Infinite Stamina | 友军无限持久，阻止持久消耗 |
| Infinite Fuel | 友军无限燃油，阻止燃油消耗 |
| Friendly Invulnerability | 友军无敌，阻止正常伤害及死亡处理 |
| Friendly Map-Token Auto-Update | 友军地图标记自动更新，无需手动移动已有标记 |

All five functions can be enabled or disabled independently.

五项功能均可独立启用和关闭。

## Installation / 使用方法

**中文**

1. 启动 Radio Commander 并进入战斗。
2. 等待战斗完全加载结束。
3. 等待接收任务中的第一条无线电通讯。
4. 打开 Cheat Engine，附加到游戏进程。
5. 加载 `RadioCommander_NoCheatMode_Experimental_v0.4.CT`。
6. 根据需要勾选相应功能。
7. 结束当前战斗或加载其他任务前，建议取消所有功能勾选。

**English**

1. Launch Radio Commander and enter a mission.
2. Wait for the battle to finish loading completely.
3. Wait until the first in-mission radio communication has been received.
4. Launch Cheat Engine and attach it to the game process.
5. Open `RadioCommander_NoCheatMode_Experimental_v0.4.CT`.
6. Enable the desired features.
7. Disable all features before leaving the mission or loading another battle.

**Do not enable any feature before receiving the first radio communication, even if Cheat Engine has already attached successfully.**

## No Cheat Mode / 不激活内置作弊模式

This table modifies the game's Mono JIT runtime behavior rather than activating the built-in cheat system.

本表格通过修改游戏运行时的 Mono JIT 代码实现功能，而不是启用游戏自带的作弊系统。

- Does not activate `charliedontsurf` or `iseeyou`.
- Does not intentionally invoke `CheatEntity.SwitchCheat` or `CheatController.CheatSwitched`.
- Does not intentionally modify the game's difficulty settings.
- Does not intentionally change built-in Cheat configuration values.
- Applies combat and resource changes to friendly units.

地图标记自动更新功能不会修改原始配置项，也不会主动显示未知敌军或生成不存在的地图标记。

**Note:** These are implementation properties, not an absolute guarantee regarding every save-file flag. Back up your original saves and verify the Cheat mode status using a separate test save. Normal mission progress and outcomes may still be saved by the game.

## Compatibility and Limitations / 兼容性及注意事项

- All five features were reported working in the user's tested environment.
- Compatibility with all game versions and missions is not guaranteed.
- Mono JIT method addresses are resolved at runtime.
- Changes to the game's code or field offsets may prevent a feature from enabling.
- The map-token feature uses the game's existing update interval, rather than forcing instant position updates.
- If a checkbox fails to activate, confirm that the battle has fully loaded and the first radio communication has been received.
- Do not leave an older overlapping CE table active.
- If the game crashes or behaves unexpectedly, disable the table, restart the game, and restore a backup if necessary.
- Intended for offline single-player use.

## Changelog / 更新记录

**v0.3**
- Added infinite friendly ammunition.
- Added infinite friendly stamina.
- Added infinite friendly fuel.
- Added friendly invulnerability.

**v0.4**
- Added automatic friendly map-token updates.
- All five features passed user testing.

**README revision — 19 October 2026**
- Added critical activation-timing instructions.
- Clarified that the battle must be fully loaded and the first radio message received before enabling any feature.
- Updated documentation for all five tested functions.
- No changes to the existing v0.4 CT scripts.

---

*Unofficial Cheat Engine table for Radio Commander. Back up your saves before using memory modifications.*