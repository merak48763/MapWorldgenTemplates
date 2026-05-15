# Dimension Types

Usually your map is built in the overworld.  
So pick a dimension type template and paste it into `data/minecraft/dimension_type/overworld.json`.

## `vanilla_overworld`

Target game version: 1.21.11, 26.1.x

- The vanilla overworld preset.

## `eternal_night`

Target game version: 1.21.11, 26.1.x

- Modified from vanilla overworld.
- Ambient sound & background music are removed.
- Sleeping doesn't change spawn point.
- Nether portals don't spawn zombified piglins.
- Piglins and hoglins don't zombify.
- Clouds are removed.
- Raid is disabled.
- Eyeblossoms stay in their current state.
- Villager activity is `idle`.
- Other time-dependent environment attributes are set to always behave like midnight, regardless of daytime.
- The timeline tag reference is removed. If you want to make time-dependent features, you need to add the field back.

> [!NOTE]
> Biomes overrides sky color by default. Vanilla biomes can make the sky bright.

> [!WARNING]
> **26.1.x**  
> Due to [MC-307449](https://mojira.dev/MC-307449), spawners with custom light limits don't work at all!  
> You can set the `gameplay/sky_light_level` attribute back to 15, at the cost of trident thrower on land. (Drowned AI only works on land with sky light level ≤ 4)

## `eternal_day`

Target game version: 1.21.11, 26.1.x

- Similar to the eternal night template.
- Visually looks like noon.
- Bed is disabled.
- Other gameplay behaviors are sill like midnight.
