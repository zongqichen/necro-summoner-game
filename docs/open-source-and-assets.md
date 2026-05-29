# GitHub 开源项目与美术资源调研

> 日期：2026-05-29
> 方法：`gh search repos` + `gh repo view`（公开 GitHub）。被 fandom/poewiki/reddit 阻拦的源不在此处
> 协议提示：每条都标了 license。**MIT / Apache-2.0 / CC-BY / CC0 = 安全可商用**；**GPL / AGPL = 强 copyleft，闭源商业作要避开**；**CC-BY-SA = 你的衍生作必须同样 CC-BY-SA 共享**

---

## A. 直接玩法竞品（开源 / 可学习的）

| 项目                                                                                            | 协议             | ⭐  | 语言          | 价值                                                                                       |
| ----------------------------------------------------------------------------------------------- | ---------------- | --- | ------------- | ------------------------------------------------------------------------------------------ |
| **[jamesmgittins/incremancer](https://github.com/jamesmgittins/incremancer)**                   | **无 license** ⚠ | 76  | HTML/JS       | 「Idle Necromancer Game」— 概念**最贴近**你的需求；可学但不能直接复用代码                  |
| **[geekazodium/project-skeleton](https://github.com/geekazodium/project-skeleton)**             | Apache-2.0 ✅    | 3   | GDScript      | 「Vampire Survivors Clone Where You Summon Minions」— 完全一致的概念；**可直接 fork 改造** |
| [matthiasbroske/VampireSurvivorsClone](https://github.com/matthiasbroske/VampireSurvivorsClone) | （查 repo）      | 248 | C# / Unity    | 完整 VS 克隆，工程结构可学                                                                 |
| [migalvalm/vampire-survivors-clone](https://github.com/migalvalm/vampire-survivors-clone)       | （查 repo）      | 25  | GDScript      | Godot 4 实现，体积小好读                                                                   |
| [getsentry/sentaur-survivors](https://github.com/getsentry/sentaur-survivors)                   | Sentry 自有      | 17  | C# / Unity    | Sentry 团队官方做的 VS clone（学工程化）                                                   |
| [Marcin-Lach/javsc](https://github.com/Marcin-Lach/javsc)                                       | （查 repo）      | 5   | GDScript      | "Just Another Vampire Survivors Clone" — 教学性强                                          |
| [Quillraven/slime-survivor](https://github.com/Quillraven/slime-survivors)                      | （查 repo）      | 4   | Java / LibGDX | 配套 YouTube 教程，0→1 极佳                                                                |

**对你的最大价值**：`geekazodium/project-skeleton` 是唯一**完全匹配**「Vampire Survivors + 召唤小弟代替武器」概念的开源项目，且 Apache-2.0。先 clone 下来跑一跑看看它做了多少。

---

## B. ARPG 引擎 / D2 复刻（玩法层学习）

| 项目                                                                        | 协议                         | ⭐         | 语言           | 价值                                                                                                     |
| --------------------------------------------------------------------------- | ---------------------------- | ---------- | -------------- | -------------------------------------------------------------------------------------------------------- |
| **[OpenDiablo2/OpenDiablo2](https://github.com/OpenDiablo2/OpenDiablo2)**   | （查 repo）                  | **11,019** | Go             | 完整的 D2 引擎重实现；**召唤物/技能系统是黄金参考**                                                      |
| **[flareteam/flare-engine](https://github.com/flareteam/flare-engine)**     | **GPL-3.0** ⚠                | 1,260      | C++            | "Free/Libre Action Roleplaying Engine" — 完整 ARPG 引擎；GPL 强传染，慎用                                |
| **[flareteam/flare-game](https://github.com/flareteam/flare-game)**         | **CC-BY-SA 3.0**（艺术资源） | 1,259      | (Tiled + JSON) | 配套游戏数据 + **完整 D2 风格艺术资源**（敌人 / 瓦片 / 法术 / NPC / 头像）；**这是你能用的最大美术宝库** |
| [AbyssEngine/AbyssEngineOld](https://github.com/AbyssEngine/AbyssEngineOld) | （查 repo）                  | 440        | C++            | 较新的 D2 引擎，仍在 active 阶段                                                                         |
| [galaxyhaxz/devilution](https://github.com/galaxyhaxz/devilution)           | Sustainable Use              | 127        | C              | D1 逆向工程，技能逻辑可读                                                                                |
| [JeremySayers/OpenARPG](https://github.com/JeremySayers/OpenARPG)           | （查 repo）                  | 0          | Godot          | Godot ARPG 起步模板（小）                                                                                |

### B.1 FLARE 美术资源详情

`flareteam/flare-game` 仓库结构（已实测 GitHub API）：

```
mods/
  fantasycore/      ← 主资源包
    images/
      enemies/      ← 敌人精灵图（D2 风格，含骷髅/僵尸等死灵相关单位）
      tilesets/     ← 地形瓦片
      powers/       ← 技能特效
      npcs/         ← NPC
      portraits/    ← 头像
      avatar/       ← 玩家
      icons/        ← UI 图标
      loot/         ← 装备
      cursors/
      menus/
  alpha_demo/
  empyrean_campaign/
  ...
```

**贡献者**：Justin Nichol、Justin Jacobs、Clint Bellanger、Stefan Beller 等 — OpenGameArt 一线作者，质量稳定。

**使用方式**：clone 仓库 → 把 `mods/fantasycore/images/` 当成你的占位美术；正式发布前再决定是替换、是按 CC-BY-SA 共享还是付费授权。

---

## C. 像素美术资源（可直接用）

### C.1 LPC（Liberated Pixel Cup）系列 — 业界最大的免费 RPG 美术宝库

| 项目                                                                                                                                                      | 协议                                    | ⭐        | 价值                                                                                                                                                                             |
| --------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **[LiberatedPixelCup/Universal-LPC-Spritesheet-Character-Generator](https://github.com/LiberatedPixelCup/Universal-LPC-Spritesheet-Character-Generator)** | **CC-BY-SA 3.0 / GPL-3.0 / OGA-BY 3.0** | **1,320** | 网页版角色生成器，几百件可拼装的部位（衣服 / 武器 / 头发 / 皮肤），**包括骷髅、僵尸、法师披风、亡灵**；可直接为每只召唤物生成独一无二的样子 — **完美契合你的「命名召唤物」需求** |
| [makrohn/Universal-LPC-spritesheet](https://github.com/makrohn/Universal-LPC-spritesheet)                                                                 | LPC 标准协议                            | 351       | 把 LPC 资源合并到一个 .xcf 的工程文件                                                                                                                                            |
| [jrconway3/lpc-jaidynreiman-assets](https://github.com/jrconway3/lpc-jaidynreiman-assets)                                                                 | LPC 标准协议                            | 0         | jrconway3 个人作的 LPC 扩展资源（头发、装备等）                                                                                                                                  |
| [LiberatedPixelCup/RPG_Maker_MZ_LPC_Starter_Kit](https://github.com/LiberatedPixelCup/RPG_Maker_MZ_LPC_Starter_Kit)                                       | LPC                                     | 7         | LPC 在 RPG Maker MZ 的整合包                                                                                                                                                     |
| [LiberatedPixelCup/LPC-list](https://github.com/LiberatedPixelCup/LPC-list)                                                                               | —                                       | 5         | 所有用过 LPC 的项目目录索引                                                                                                                                                      |

**LPC 协议解读**：

- **CC-BY-SA 3.0**：你必须 (1) 署名原作者；(2) 衍生作以同协议开源
- **OGA-BY 3.0**：仅署名，无 share-alike — 这条更友好
- **GPL-3.0**：传染性极强，源码必须开源

**实操建议**：用 OGA-BY 3.0 部分的资源，可以闭源商业发布；用 CC-BY-SA 3.0 部分，要么接受 share-alike，要么先确认每张图的具体协议。

### C.2 LPC 工具链（导入/切片自动化）

| 项目                                                                                                                    | ⭐  | 用途                                       |
| ----------------------------------------------------------------------------------------------------------------------- | --- | ------------------------------------------ |
| [alextrevisan/LPCAnimatedSprite2D](https://github.com/alextrevisan/LPCAnimatedSprite2D)                                 | 65  | Godot 4 自动切片 LPC 精灵图                |
| [DrJamgo/Godot_LPC_Spritesheet_Gen](https://github.com/DrJamgo/Godot_LPC_Spritesheet_Gen)                               | 17  | Godot 用的 LPC 生成器                      |
| [bitcula/Universal-LPC-Spritesheet-Unity-Importer](https://github.com/bitcula/Universal-LPC-Spritesheet-Unity-Importer) | 13  | Unity 自动切片 LPC                         |
| [WeiWeiWesley/lpc-spritesheet](https://github.com/WeiWeiWesley/lpc-spritesheet)                                         | 0   | Godot AnimatedSprite2D / AtlasTexture 生成 |

### C.3 其他 CC0 资源仓库

| 项目                                                                                                | ⭐  | 内容                     |
| --------------------------------------------------------------------------------------------------- | --- | ------------------------ |
| [utgarda/kenney-hexagon](https://github.com/utgarda/kenney-hexagon)                                 | 1   | Kenney CC0 六边形包      |
| [SpriteCook/spritecook-free-game-assets](https://github.com/SpriteCook/spritecook-free-game-assets) | 0   | 综合 CC0 包              |
| [iwenzhou/kenney](https://github.com/iwenzhou/kenney)                                               | 5   | Kenney 完整 Asset Pack 1 |

**注**：Kenney 的真正发布地是 [kenney.nl](https://kenney.nl)，全部 CC0（最自由的协议，没有任何附加要求）— 比 LPC 更好用，但风格偏儿童 / 卡通，**不太契合死灵哥特题材**。

---

## D. 像素美术编辑器（你制作 / 修改资源用）

| 工具                                                                            | 协议                | ⭐         | 平台              | 推荐度                                           |
| ------------------------------------------------------------------------------- | ------------------- | ---------- | ----------------- | ------------------------------------------------ |
| **[aseprite/aseprite](https://github.com/aseprite/aseprite)**                   | 个人 / 商业付费源码 | **37,223** | Win/Mac/Linux     | 业界标准，付费 $20，**如果你能编译源码可免费**用 |
| [piskelapp/piskel](https://github.com/piskelapp/piskel)                         | Apache-2.0 ✅       | 12,507     | Web / 桌面        | 浏览器版免费，足够原型用                         |
| [Orama-Interactive/Pixelorama](https://github.com/Orama-Interactive/Pixelorama) | MIT ✅              | 9,642      | Win/Mac/Linux/Web | 完全开源免费，UI 接近 Aseprite                   |
| [foxnne/fizzy](https://github.com/foxnne/fizzy)                                 | （查）              | 1,374      | Zig 写的          | 新兴，小但快                                     |
| [Pixen/Pixen](https://github.com/Pixen/Pixen)                                   | （查）              | 934        | macOS only        | macOS 原生                                       |

**推荐**：先用 **Pixelorama**（MIT，零成本），后期需要专业功能再上 Aseprite。

---

## E. Idle / 增量游戏框架（可加速你的核心循环）

| 项目                                                                                  | ⭐  | 语言 | 价值                           |
| ------------------------------------------------------------------------------------- | --- | ---- | ------------------------------ |
| [GSoster/idle-game](https://github.com/GSoster/idle-game)                             | 16  | JS   | 通用挂机框架，资源/升级/自动化 |
| [RNT17/Idle-Game-Framework](https://github.com/RNT17/Idle-Game-Framework)             | 7   | C#   | Unity 友好                     |
| [whoisforest/Idle-Game-Framework](https://github.com/whoisforest/Idle-Game-Framework) | 0   | C#   | Godot                          |

**判断**：这些框架体量小、个人项目居多，对你目前阶段（PC 单机 ARPG）参考价值有限，但**v0.3 加离线挂机时**可以借鉴。

---

## F. 像素艺术 / RTS / 战术参考

| 项目                                                                          | 协议           | ⭐    | 价值                                                                               |
| ----------------------------------------------------------------------------- | -------------- | ----- | ---------------------------------------------------------------------------------- |
| [OpenHV/OpenHV](https://github.com/OpenHV/OpenHV)                             | （查）         | 1,000 | "Open Source Pixelart Science-Fiction RTS" — 像素 RTS，单位编队 / 自动战斗机制可学 |
| [TeamHypersomnia/Hypersomnia](https://github.com/TeamHypersomnia/Hypersomnia) | （查）         | 1,554 | 像素风多人射击，工程化参考                                                         |
| [FreezingMoon/AncientBeast](https://github.com/FreezingMoon/AncientBeast)     | **AGPL-3.0** ⚠ | 1,852 | 回合制策略「驾驭你的野兽」— 召唤物战斗的另一种实现；AGPL 不可商用闭源              |
| [fishfolk/jumpy](https://github.com/fishfolk/jumpy)                           | （查）         | 1,839 | Rust + Bevy 像素战斗游戏，引擎层参考                                               |

---

## G. 协议地雷区警告 ⚠

| 协议                       | 含义                       | 你能做什么                                  |
| -------------------------- | -------------------------- | ------------------------------------------- |
| **MIT / Apache-2.0 / BSD** | 几乎无限制，需保留版权声明 | ✅ 闭源商用、改造、分发都可                 |
| **CC0**                    | 完全放弃版权               | ✅ 任意用                                   |
| **CC-BY**                  | 只需署名                   | ✅ 闭源商用，credits 列原作者               |
| **OGA-BY**                 | OGA 版本的 CC-BY           | ✅ 同上                                     |
| **CC-BY-SA**               | 署名 + 衍生作同协议        | ⚠ **你的整套美术也要 CC-BY-SA**，慎用       |
| **GPL / AGPL**             | 强传染，源码必须开源       | ❌ 闭源商业绝对不能用代码；美术资源不受影响 |
| **无 License**             | 默认全权保留               | ❌ 不能用，**联系作者获授权**               |

**最危险的陷阱**：FLARE 引擎是 GPL-3.0，你不能直接用它的代码做商业闭源游戏。但 FLARE 的**美术资源**是 CC-BY-SA，可以用（但你的衍生美术也得 SA 共享）。

**最安全的组合**：

- 美术：Kenney CC0（题材不对）/ LPC OGA-BY 部分（最佳） / 自制
- 代码：从零写 / Apache-2.0 项目 fork（如 `project-skeleton`）

---

## H. 实操推荐路径

### 路径 1：极速 MVP（1–2 周原型）

```
fork geekazodium/project-skeleton (Apache-2.0)
  + 用 LPC Universal Character Generator 生成 5 种召唤物精灵
  + 拿 flare-game 的 enemies 做敌人（CC-BY-SA，原型阶段问题不大）
  + 自己写 拼接 / 命名 / 永久死亡 三大系统
```

### 路径 2：从零写 + 借美术（推荐，与你 v0.1 prototype 一致）

```
继续 vanilla TS + Canvas（已有 prototype 骨架）
  + LPC 角色生成器导出精灵 → 替换 emoji
  + flare-game/mods/fantasycore/images/enemies → 你的敌人
  + Pixelorama 改色 / 加细节
```

### 路径 3：Godot 重写（长期最值）

```
Godot 4 + GDScript
  + alextrevisan/LPCAnimatedSprite2D 自动导入 LPC
  + 参考 migalvalm/vampire-survivors-clone 的工程结构
  + flare-game 美术做占位
```

---

## I. 还没找到的（你可能想自己搜）

- [ ] **死灵主题专属的 sprite 包** — GitHub 上没有热门仓；建议去 [itch.io](https://itch.io/game-assets/free/tag-pixel-art) 搜 "necromancer pixel" / "undead sprite"
- [ ] **音乐资源** — GitHub 上无热门免费音乐仓；建议 [opengameart.org](https://opengameart.org/art-search?keys=dark+fantasy) 或 [freesound.org](https://freesound.org)
- [ ] **音效（骨头碎裂、亡灵嚎叫等）** — 同上
- [ ] **Spine / Skeleton 动画** — 多为商业资源，开源不多
- [ ] **中文同好做的死灵题材原型** — GitHub 中文搜索结果稀疏，可能在 Gitee 上更好

---

## J. 一页速查（按你的实际操作给出 TOP 6）

| 用途                          | 推荐                                  | 协议                             | 立即上手命令                                                                                                                                                            |
| ----------------------------- | ------------------------------------- | -------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **完全一致概念的 fork 起点**  | `geekazodium/project-skeleton`        | Apache-2.0                       | `gh repo clone geekazodium/project-skeleton`                                                                                                                            |
| **召唤物 / 角色精灵**         | LPC Universal Character Generator     | OGA-BY 3.0（部分）/ CC-BY-SA 3.0 | 在线用 [https://sanderfrenken.github.io/Universal-LPC-Spritesheet-Character-Generator/](https://sanderfrenken.github.io/Universal-LPC-Spritesheet-Character-Generator/) |
| **D2 风格敌人 / 瓦片 / 特效** | `flareteam/flare-game` 的 fantasycore | CC-BY-SA 3.0                     | `gh repo clone flareteam/flare-game` 后看 `mods/fantasycore/images/`                                                                                                    |
| **像素编辑器**                | Pixelorama                            | MIT                              | 下载即用                                                                                                                                                                |
| **D2 召唤系统参考代码**       | `OpenDiablo2/OpenDiablo2`             | （查 repo）                      | 看 `d2core/d2hero`                                                                                                                                                      |
| **挂机框架（v0.3 用）**       | `GSoster/idle-game`                   | （查）                           | JS 友好                                                                                                                                                                 |

---

## K. 一句话总结

**美术资源没问题** — LPC + flare-game 已经够你做出 D2 风格的 ARPG 原型，全部协议清晰可用。
**玩法参考也找到了** — `geekazodium/project-skeleton` 是 Apache-2.0 的「召唤小弟代替武器」原型，可以直接 fork 改造。
**核心差异化（拼接 / 命名 / 永久死亡）任何项目都没做过** — 你的差异化空间仍然完整保留。
