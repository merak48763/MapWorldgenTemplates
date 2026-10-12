# Timelines

## `eternal_night`

Target game version: 1.21.11, 26.1.x, 26.2, 26.3

- Sleeping doesn't change spawn point.
- Eyeblossoms stay in their current state.
- Villager activity is `idle`.
- Other time-dependent environment attributes are set to always behave like midnight, regardless of daytime.
- Supposed to be combined with `empty` dimension type preset.

> [!WARNING]
> **26.1 ~ 26.2**  
> Due to [MC-307449](https://mojira.dev/MC-307449), spawners with custom light limits don't work at vanilla night.  
> To patch the issue, `gameplay/sky_light_level` attribute is set to 15. This breaks some hardcoded mechanisms:
>
> - Drowned AI doesn't work on land
> - Spider is blind under sky
>
> To mitigate the side effects, set `has_fixed_time` to `true` in dimension type. This revives drowned on land while introducing some new negligible side effects.

## `eternal_day`

Target game version: 1.21.11, 26.1.x, 26.2, 26.3

- Similar to the eternal night template.
- **Visually** looks like noon.
- Bed is disabled.
- Other gameplay behaviors are sill like midnight.
- Supposed to be combined with `empty` dimension type preset.
