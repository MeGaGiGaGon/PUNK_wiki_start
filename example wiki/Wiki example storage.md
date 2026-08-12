# Example PUNK Playtest Index
```
== Note to admins ==

We are planning to structure the wiki like the [https://noita.wiki.gg Noita Wiki], giving pages for:
* 65 Entities
* 29 Modules
* 22 Weapons
* 12 Gadgets
* 12 Tiles

As well as the corresponding overview pages, and other guide/tutorial/advanced mechanics pages. Most of the data is already gathered and just needs formatted.


== Tile Pages ==

[[Example PUNK Playtest Bubble Tile]]

[[Example PUNK Playtest Electricity Tile]]

=== Tile copyable code ===
<syntaxhighlight lang="wikitext" style="overflow: auto;">
{{Example PUNK Playtest Infobox Tile
|title=
|image=

|Defense=
|Burn Threshold=
|Burn Duration=
|Contact Damage=

|Loot 1=
|Loot 2=
|Loot 3=
|Loot 4=
|Loot 5=
}}
</syntaxhighlight>

== Enemy Pages ==

[[Example PUNK Playtest Turret Seeker Enemy]]

[[Example PUNK Playtest Basic Fly Enemy]]

=== Enemy copyable code ===
<syntaxhighlight lang="wikitext" style="overflow: auto;">
{{Example PUNK Playtest Infobox Enemy
|title=
|image=

|Faction=
|Blocks Station Unlock=
|Power Level=

|Burn Threshold=
|Burn Cooling Speed=
|Burn Fire Tick Rate=
|Burn Fire Damage Per Tick=

|Health Max=
|Health Regen=

|Gel Max=
|Gel Regen=
|Gel Shield=

|Caps Max=
|Caps Regen=
|Caps Shield=

|Tech Max=
|Tech Regen=
|Tech Shield=

|Electron Max=
|Electron Regen=
|Electron Shield=

|Loot 1=
|Loot 2=
|Loot 3=
|Loot 4=
|Loot 5=
}}
</syntaxhighlight>
```

# Example PUNK Playtest Bubble Tile
```
{{Example PUNK Playtest Infobox Tile
|title=Bubble Tile
|image=Example-PUNK-Playtest-Bubble-Tile.png

|Defense=1
|Burn Threshold=1.3
|Burn Duration=0.6
|Contact Damage=

|Loot 1=1 Stamina Pickup
|Loot 2=
|Loot 3=
|Loot 4=
|Loot 5=
}}

Easily breakable tile found in almost all biomes

Can give extra Stamina during fights if using a weapon with multiple projectiles like Shotgun and Worm, or explosive radius like Dart
```

# Example PUNK Playtest Electricity Tile
```
{{Example PUNK Playtest Infobox Tile
|title=Electricity Tile
|image=Example-PUNK-Playtest-Electricity-Tile.png

|Defense=10
|Burn Threshold=0
|Burn Duration=2
|Contact Damage=1

|Loot 1=
|Loot 2=
|Loot 3=
|Loot 4=
|Loot 5=
}}
```

# Example PUNK Playtest Turret Seeker Enemy
```
{{Example PUNK Playtest Infobox Enemy
|title=Turret Seeker
|image=Example-PUNK-Playtest-Turret-Seeker-Enemy.png

|Faction=Fly
|Blocks Station Unlock=Yes
|Power Level=10

|Burn Threshold=3
|Burn Cooling Speed=1
|Burn Fire Tick Rate=1
|Burn Fire Damage Per Tick=1

|Health Max=100
|Health Regen=3

|Gel Max=
|Gel Regen=
|Gel Shield=

|Caps Max=50
|Caps Regen=5
|Caps Shield=Yes

|Tech Max=
|Tech Regen=
|Tech Shield=

|Electron Max=
|Electron Regen=
|Electron Shield=

|Loot 1=30x10 Value Gold Pickups
|Loot 2=20x20 Value Gold Pickups
|Loot 3=10xResource Tech
|Loot 4=
|Loot 5=
}}

Spawns primarily in the Quartz and Overgrown biomes

The rocket projectile they shoot is extremely dangerous, but also does massive self damage if you can lure into the turret/other enemies
```

# Example PUNK Playtest Basic Fly Enemy
```
{{Example PUNK Playtest Infobox Enemy
|title=Basic Fly
|image=Example-PUNK-Playtest-Basic-Fly-Enemy.png

|Faction=Fly
|Blocks Station Unlock=True
|Power Level=5

|Burn Threshold=3
|Burn Cooling Speed=1
|Burn Fire Tick Rate=1
|Burn Fire Damage Per Tick=1

|Health Max=3
|Health Regen=

|Gel Max=
|Gel Regen=
|Gel Shield=

|Caps Max=
|Caps Regen=
|Caps Shield=

|Tech Max=
|Tech Regen=
|Tech Shield=

|Electron Max=
|Electron Regen=
|Electron Shield=

|Loot 1=1-3x10 Value Gold Pickups
|Loot 2=
|Loot 3=
|Loot 4=
|Loot 5=
}}

Spawns primarily in the start biomes

Rushing down with Worm or Shotgun is very effective
```

# Template:Example PUNK Playtest Infobox Tile
```
<includeonly>{{#invoke:Infobox|main
|sep=,
|image={{#if:{{{image|}}}|[[File:{{{image}}}{{!}}300px]]}}
|sections=Tile Info, Burn Info, Loot Info

|Tile Info=Defense, Contact Damage
|Tile Info_nolabel=yes

|Burn Info={{#ifeq:{{{Burn Threshold|}}}|0||Burn Threshold}}, {{#ifeq:{{{Burn Threshold|}}}|0||Burn Duration}}, burnable
|burnable={{#ifeq:{{{Burn Threshold|}}} |0| <div style="text-align:center;">Not Burnable</div> | }}
|burnable_nolabel=yes

|Loot Info=Loot 1, Loot 2, Loot 3, Loot 4, Loot 5,Value
|Loot 1_nolabel=yes
|Loot 2_nolabel=yes
|Loot 3_nolabel=yes
|Loot 4_nolabel=yes
|Loot 5_nolabel=yes


}}</includeonly><noinclude>{{documentation}}</noinclude>
```

# Template:Example PUNK Playtest Infobox Enemy
```
<includeonly>{{#invoke:Infobox|main
|sep=,
|image={{#if:{{{image|}}}|[[File:{{{image}}}{{!}}300px]]}}
|sections=General Info, Burn Info, Resources Info, Loot Info

|General Info=Faction, Blocks Station Unlock, Power Level
|General Info_nolabel=yes

|Burn Info=Burn Threshold, Burn Cooling Speed, Burn Fire Tick Rate, Burn Fire Damage Per Tick
|Burn Info_collapsible=Yes
|Burn Info_collapsed=Yes

|Resources Info=Health Max, Health Regen, Gel Max, Gel Regen, Gel Shield, Caps Max, Caps Regen, Caps Shield, Tech Max, Tech Regen, Tech Shield, Electron Max, Electron Regen, Electron Shield

|Loot Info=Loot 1, Loot 2, Loot 3, Loot 4, Loot 5
|Loot 1_nolabel=yes
|Loot 2_nolabel=yes
|Loot 3_nolabel=yes
|Loot 4_nolabel=yes
|Loot 5_nolabel=yes

}}</includeonly><noinclude>{{documentation}}</noinclude>
```
