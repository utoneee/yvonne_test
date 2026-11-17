# 素材資料夾

把生好的圖放進來，**檔名照下面規則**，遊戲會自動換上；沒放的角色或主場會繼續用程式畫的佔位圖。

| 種類 | 路徑 | 規格 |
|---|---|---|
| 角色立繪 | `assets/chars/{id}.png`（也接受 `.webp`） | 去背透明 PNG、全身、**面向右**，建議高度 600px 以上 |
| 主場背景 | `assets/stages/{id}.jpg`（也接受 `.png`） | 16:9，建議 1920×1080，下方三分之一是平坦地面 |
| 片頭主視覺 | `assets/intro.jpg`（也接受 `.png`） | 16:9，上方三分之一留給標題字 |

## 16 個 id

| id | 角色 | id | 角色 |
|---|---|---|---|
| `mole` | 台灣鼴鼠 | `tarantula` | 紅膝頭捕鳥蛛 |
| `palawan` | 巴拉望巨扁鍬形蟲 | `centipede` | 巨人蜈蚣 |
| `giraffe` | 長頸鹿鋸鍬形蟲 | `crab` | 椰子蟹 |
| `atlas` | 南洋大兜蟲 | `frog` | 藍箭毒蛙 |
| `hercules` | 長戟大兜蟲 | `chameleon` | 高冠變色龍 |
| `hornet` | 中華大虎頭蜂 | `axolotl` | 六角恐龍 |
| `mantis` | 蘭花螳螂 | `star_mole` | 星鼻鼴鼠 |
| `scorpion` | 帝王蠍 | `lizard` | 澳洲傘蜥蜴 |

例：`assets/chars/hercules.png`、`assets/stages/hercules.jpg`

P2 選到同一隻角色時，程式會自動做色違版本，不用另外生圖。
