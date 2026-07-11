# Customization Guide

## How to Modify Lucky Block Rewards

### Edit Loot Tables

1. Open `behavior_pack/loot_tables/lucky_block_rewards.json`
2. Modify the `weight` values to change reward probabilities
3. Add new items to the `entries` array
4. Adjust min/max counts for item quantities

### Example: Add Custom Reward

```json
{
  "type": "item",
  "name": "minecraft:dragon_egg",
  "weight": 3,
  "functions": [
    {
      "function": "set_count",
      "count": 1
    }
  ]
}
```

### Probability Calculation

- Total weight = sum of all weights
- Item probability = item weight / total weight

For example, if an item has weight 10 and total is 100:
- Probability = 10/100 = 10%

## Changing Block Properties

Edit `behavior_pack/blocks/lucky_block.json`:

- `destroy_time`: How long to break (0.5 = very fast)
- `explosion_resistance`: Explosion protection
- `map_color`: Block color on maps (#FFD700 = gold)

## Custom Textures

1. Create 16x16 PNG images for:
   - `lucky_block_top.png`
   - `lucky_block_side.png`
   - `lucky_block_bottom.png`

2. Place in `resource_pack/textures/blocks/`

3. Update the texture references in `lucky_block.json`

## Adding Sound Effects

1. Create OGG audio files
2. Place in `resource_pack/sounds/`
3. Reference in `sounds.json`

## Testing Your Changes

1. Make changes to the JSON files
2. Reload Minecraft
3. Test in a creative world
4. Verify all changes work as expected
