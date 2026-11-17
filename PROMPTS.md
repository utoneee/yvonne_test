# 生圖詠唱詞（Image-Gen Prompts）

生好的圖請依 [`assets/README.md`](assets/README.md) 的檔名放進 `assets/`。

---

## 一、角色立繪

### 通用基底模板

```
Full-body character portrait of a {SPECIES_DESCRIPTION}, anthropomorphic fighting-game hero pose, dynamic heroic stance facing right, three-quarter view, entire body visible from head to toe, centered composition,
semi-realistic stylized 2D game art, cel-shaded with bold clean outlines, rich vibrant colors, dramatic rim lighting with warm golden amber highlights, subtle golden energy aura,
highly detailed textures, anatomically faithful to the real species, fierce determined expression,
isolated on a pure solid white background, no shadow on ground, no text, no watermark, no frame, no extra creatures,
--ar 3:4
```

**負面詠唱詞：**
```
cropped, cut off limbs, multiple characters, background scenery, ground shadow, text, logo, watermark, blurry, low resolution, deformed anatomy, extra limbs, human face, photorealistic photo
```

> 把 `{SPECIES_DESCRIPTION}` 換成下面的特徵詞。白底方便用 rembg、remove.bg 去背。存成 `assets/chars/{id}.png`，**角色要面向右**。

### 16 位角色特徵詞

| # | id | 角色 | 特徵詞 |
|---|---|---|---|
| 1 | `mole` | 台灣鼴鼠 | Taiwanese Mole (Mogera insularis) with velvety dark brown fur, large pink digging claws raised like boxing gloves, tiny pink snout |
| 2 | `palawan` | 巴拉望巨扁鍬形蟲 | Palawan Giant Stag Beetle (Dorcus titanus palawanicus) with massive glossy black serrated mandibles opened wide, heavy armored thorax |
| 3 | `giraffe` | 長頸鹿鋸鍬形蟲 | Giraffe Stag Beetle (Prosopocoilus giraffa) with extremely long slender jagged mandibles extended forward like a fencing rapier, glossy black shell |
| 4 | `atlas` | 南洋大兜蟲 | Atlas Beetle (Chalcosoma atlas) with three huge curved metallic dark-green horns, iridescent bronze-green carapace |
| 5 | `hercules` | 長戟大兜蟲 | Hercules Beetle (Dynastes hercules) with a massive golden-yellow spotted carapace and gigantic curved black horn |
| 6 | `hornet` | 中華大虎頭蜂 | Asian Giant Hornet (Vespa mandarinia) hovering aggressively with translucent wings, bright yellow-orange head, black-and-yellow striped abdomen, sharp stinger |
| 7 | `mantis` | 蘭花螳螂 | Orchid Mantis (Hymenopus coronatus) in martial arts mantis-style stance, white and pastel pink petal-like legs and scythe forelimbs |
| 8 | `scorpion` | 帝王蠍 | Emperor Scorpion (Pandinus imperator) with massive glossy black pincers raised and segmented stinger tail arched overhead |
| 9 | `tarantula` | 紅膝頭捕鳥蛛 | Mexican Redknee Tarantula (Brachypelma hamorii) with velvety black body and vivid bright orange-red leg joints, front legs raised in threat pose |
| 10 | `centipede` | 巨人蜈蚣 | Giant Centipede (Scolopendra) in a dynamic S-curve striking stance, glossy dark reddish-black segmented armor plates, vibrant bright orange-yellow legs, sharp venomous forcipule fangs raised in front |
| 11 | `crab` | 椰子蟹 | Coconut Crab (Birgus latro) with thick purple-blue and burnt-orange armored exoskeleton and colossal crushing claws raised |
| 12 | `frog` | 藍箭毒蛙 | Blue Poison Dart Frog (Dendrobates azureus) in an agile leaping combat crouch, vivid sapphire-blue skin with black spots |
| 13 | `chameleon` | 高冠變色龍 | Veiled Chameleon (Chamaeleo calyptratus) with tall head casque, vibrant emerald green and yellow striped scales, curled tail, alert turret eyes |
| 14 | `axolotl` | 六角恐龍 | Axolotl salamander in a cute yet fierce water-kung-fu stance, pale pink body with fluffy bright magenta external gill frills |
| 15 | `star_mole` | 星鼻鼴鼠 | Star-nosed Mole (Condylura cristata) with sleek dark charcoal fur, 22-tentacle bright pink star-shaped nose, broad paddle-like digging claws |
| 16 | `lizard` | 澳洲傘蜥蜴 | Australian Frill-necked Lizard (Chlamydosaurus kingii) standing upright on hind legs with its huge orange-brown patterned neck frill flared wide |

> P2 色違版由程式自動產生（色相旋轉 150°＋飽和度 1.6 倍），不必另外生圖。

---

## 二、主場背景（16:9）

### 通用基底模板

```
Wide panoramic 2D fighting game stage background of {STAGE_DESCRIPTION},
side-scrolling arena composition with a clear flat walkable ground plane across the lower third, open empty space in the center for two fighters, strong depth with layered foreground, midground and distant background,
painterly semi-realistic style, cinematic lighting, atmospheric perspective, vibrant but slightly desaturated so characters stand out, subtle floating golden amber particles,
no characters, no creatures, no people, no text, no UI, no watermark,
--ar 16:9
```

**負面詠唱詞：**
```
characters, animals, insects, people, text, logo, watermark, cluttered center, tilted horizon, fisheye, blurry, low resolution
```

> 存成 `assets/stages/{id}.jpg`。對戰時使用 P2（或 CPU）角色的主場。

### 16 大主場描述

| id | 主場描述 |
|---|---|
| `mole` | an underground forest humus soil burrow with tree roots, glowing crystals, and packed dark earth floor |
| `palawan` | a Palawan tropical rainforest clearing beside a giant mossy fallen log and flat dirt ground |
| `giraffe` | high canopy branches of a Southeast Asian hardwood tree with golden amber tree sap glowing in sunlight |
| `atlas` | a misty mountain cloud forest with ferns and a flat rocky moss terrace |
| `hercules` | a towering Central American giant tree canopy surrounded by hanging wild orchids and sturdy flat branch platform |
| `hornet` | high mountain pine branches beside a massive papery giant hornet nest overlooking misty peaks |
| `mantis` | a lush tropical orchid garden trellis filled with pink and white blossoms and flat stone walkway |
| `scorpion` | a shadowed West African forest rock crevice cave with damp leaf litter and subtle blue bioluminescent moss |
| `tarantula` | an arid Mexican red-earth desert floor with saguaro cacti, desert rocks, and warm sunset sky |
| `centipede` | a humid tropical rainforest floor under a giant hollow mossy log, damp fallen leaves, glowing mushrooms, dappled forest light |
| `crab` | a tropical coral sand beach lined with coconut palm trees and fallen coconuts under bright turquoise sky |
| `frog` | a Suriname rainforest waterfall creek bank with wet mossy stones and bromeliad plants |
| `chameleon` | sunlit Madagascar forest canopy boughs with dappled golden light and broad flat tree limbs |
| `axolotl` | the crystal-clear underwater floor of Lake Xochimilco with swaying green aquatic plants and sunlit water ripples |
| `star_mole` | a misty peat bog creek bank with dark wet soil, reeds, and shallow stream reflections |
| `lizard` | an Australian red-earth savanna outback with eucalyptus trees, dry grass, and flat red dirt ground |

---

## 三、片頭「黃金琥珀核心」主視覺

```
Epic fighting game title key art: a colossal glowing golden amber gemstone core floating at the center, with a perfectly preserved ancient prehistoric insect fossil visible inside the translucent amber, radiating intense golden light beams and swirling energy rings,
the amber core hovers above a massive ancient tree stump in a primeval jungle, cracked earth below glowing with golden veins,
dramatic silhouettes of giant beetles, a mantis, a scorpion, a hornet, a frog and a frilled lizard gathered around the core in battle-ready poses, partially backlit, rim-lit by the amber glow,
floating amber shards, glowing pollen particles, god rays through mist, deep dark-brown and black shadows contrasting with brilliant gold #F5A623,
cinematic epic composition, low-angle hero shot, semi-realistic stylized 2D game illustration, ultra detailed, high contrast,
empty space at the top third for the game title logo, no text, no watermark,
--ar 16:9
```

> 存成 `assets/intro.jpg`。標題文字由遊戲程式疊上，圖上不要有字。
