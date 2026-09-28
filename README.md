# Alloyer Uranium - Sun (NeoForge 1.21.1)

Requires: Mekanism 10.7+, Mekanism: Sun 1.2.0+.

- Mekanism: Sun has no electrum ore. Electrum = 1 gold ingot + 1 silver ingot + 100 mB helium -> 2 electrum (Alloyer).
- 10 extra silver veins per chunk (size 9, Y -64 to 48).
- Silver ore / deepslate silver ore: 1-2 raw silver base + Fortune bonus (uniform_bonus_count, multiplier 2). Silk Touch works.
- Alloyer: 1 lapis lazuli + 1 electrum ingot + 25 mB hydrogen -> 2 uranium ingots.
- Pressurized Reaction Chamber: 40 mB helium + 10 mB water + 1 redstone dust -> 10 mB hydrogen (lossy 4:1, so the Artificial Sun's waste helium can be recycled into fuel without creating a free-energy loop).

Tuning: worldgen/placed_feature/silver_extra.json (count, height), configured_feature/silver_extra.json (size),
data/mekanismsun/loot_table/blocks/*.json (Fortune multiplier).

Build: JDK 21, run `gradle wrapper` once (or copy gradlew + gradle-wrapper.jar from a NeoForge 1.21.1 MDK),
then `./gradlew build`. Jar: build/libs/alloyer_sun-1.0.0.jar
