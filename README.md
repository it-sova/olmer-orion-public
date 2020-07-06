# Orion scripts for Olmer shard

## Loot description
Script should be bound on any button to start. It loots all corpses around you and exists.
Depending on settings, cutting also available.

## Loot settings
If loot bag specified and available - loot will be collected to bag, in other case - to backpack
If cut_corpses == 1 - script will cut all corpses after loot
```js
var loot_bag = 0x405990CD;
var cut_corpses = 1;
```
Array that consists of items types to loot. Color doesn't matter
```js
_loot = [
    0x0EED, // Gold
    ....
];
```
Items to use after looting ( e.g. exp scrolls, point books etc...)
```js
_use_after_loot = [
    0x0E35, // Shadow exp scroll
];
```
Items to throw away after cutting ( e.g. ore from elementals, humad heads, etc...)
```js
_trash_items = [
    0x19B9, // Ore
    0x1CE1, // Human head 
];
```
