The world is made of [[Tile]]s

# Defense
Each tile has a [[Tile#Defense|Defense]] value, the required damage to break it

Damage to a tile does not stack over time, the tile must take damage greater than it's [[Tile#Defense|Defense]] in a single hit to break

# Burn
Each [[Tile]] has a [[Tile#Burn|Burn]] Threshold, over which the [[Tile]] will start burning

The [[Tile#Burn|Burn]] Threshold is cumulative and does not decay, so it is possible start burning a [[Tile]] using multiple weaker [[Tile#Burn|Burn]] attacks

After a [[Tile]] has been burning for it's [[Tile#Burn|Burn]] Duration, it will either be destroyed or turn into a different [[Tile]]

Some [[Tile]]s are not [[Tile#Burn|Burn]]able

While burning, some of the [[Tile#Burn|Burn]] on a [[Tile]] will be transferred to neighboring tiles

TODO(GiGaGon): Figure out exact burn transfer/overflow formula

