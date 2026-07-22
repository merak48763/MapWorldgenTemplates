# Biomes

Biome templates.

## `default`

Target game version: 1.21.11, 26.1.x, 26.2

- Has no environment attribute overrides.
- Natural mob spawning is disabled.
- Bonemealing grass creates "default" flower patches, which contains poppy and dandelion.

## Palette

### Common grass & foliage color parameters

Most biomes use `temperature` and `downfall` to control grass color and foliage color.

| Biome | `temperature` | `downfall` |
| --- | --- | --- |
| The Void | 0.5 | 0.5 |
| Plains | 0.8 | 0.4 |
| Desert | 2.0 | 0.0 |
| Jungle | 0.95 | 0.9 |
| Snowy Plains | 0.0 | 0.5 |

Some biomes directly specify grass color and foliage color.

| Biome | Grass Color | Foliage Color | Dry Foliage Color |
| --- | --- | --- | --- |
| Badlands | `#90814d` | `#9e814d` | - |
| Cherry Grove | `#b6db61` | `#b6db61` | - |
| Pale Garden | `#778272` | `#878d76` | `#a0a69c` |
| Sulfur Caves | `#aba64f` | - | - |
| Dappled Forest | `#df6827` | `#e68e30` | `#8c3a04` |
| Swamp | Hardcoded | `#6a7039` | `#7b5334` |
| Dark Forest | Hardcoded | - | `#7b5334` |

### Common water visual parameters

The default water fog color is `#050533`. Most biomes don't override it.

| Biome | Water Color | Water Fog Color | Water Fog Distance |
| --- | --- | --- | --- |
| Most Biomes | `#3f76e4` | - | - |
| Cherry Grove | `#5db7ef` | `#5db7ef` | - |
| Pale Garden | `#76889d` | `#556980` | - |
| Sulfur Caves | `#34bf89` | `#17543c` | - |
| Dappled Forest | `#375154` | `#375154` | - |
| Swamp | `#617b64` | `#232317` | End distance 0.85x |
| Mangrove Swamp | `#3a7a6a` | `#4d7a60` | End distance 0.85x |
| Warm Ocean | `#43d5ee` | `#041f33` | - |
| Frozen Ocean | `#3938c9` | - | - |

### Common environment color parameters

- Sky color is always `#000000` during night.
- Fog color is multiplied by `#0f0f16` during night.

It's recommended to apply the modifiers in timelines.

| Biome | Sky Color | Fog Color |
| --- | --- | --- |
| Plains | `#78a7ff` | `#c0d8ff` |
| Desert | `#6eb1ff` | `#c0d8ff` |
| Frozen Peaks | `#859dff` | `#c0d8ff` |
| Pale Garden | `#b9b9b9` | `#817770` |
| Sulfur Caves | `#78a7ff` | `#8cb831` |
| Dappled Forest | `#7ca3ff` | `#ccd8e2` |
| Nether Wastes | - | `#330808` |
| Crimson Forest | - | `#330303` |
| Warped Forest | - | `#1a051a` |
| Soul Sand Valley | - | `#1b4745` |
| Basalt Deltas | - | `#685f70` |

### Biome Particles

Although particle config allows multiple particle entries, vanilla biomes only use one.

| Biome | Particle | Probability |
| --- | --- | --- |
| Crimson Forest | `crimson_spore` | 0.025 |
| Warped Forest | `warped_spore` | 0.01428 |
| Soul Sand Valley | `ash` | 0.00625 |
| Basalt Deltas | `white_ash` | 0.118093334 |

### Bonemeal Flowers

| Feature | Flower Types |
| --- | --- |
| `flower_default` | Poppy <br /> Dandelion |
| `flower_cherry` | Pink Petals |
| `flower_flower_forest` | Dandelion <br /> Poppy <br /> Allium <br /> Azure Bluet <br /> Red Tulip <br /> Orange Tulip <br /> White Tulip <br /> Pink Tulip <br /> Oxeye Daisy <br /> Cornflower <br /> Lily of the Valley |
| `flower_meadow` | Allium <br /> Poppy <br /> Azure Bluet <br /> Dandelion <br /> Cornflower <br /> Oxeye Daisy |
| `flower_pale_garden` | Closed Eyeblossom |
| `flower_plain` | Dandelion <br /> Orange Tulip <br /> Red Tulip <br /> Pinnk Tulip <br /> White Tulip <br /> Poppy <br /> Azure Bluet <br /> Oxeye Daisy <br /> Cornflower |
| `flower_swamp` | Blue Orchid |
