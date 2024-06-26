# Trinity

*Trinity* is an expanded approach to *Challenges* for the **Terran Engine**.

Like *Challenges*, *Trinity* have descriptive **Names** and numeric **Disposition** and **Severity**.
Unlike Challenges, *Trinity*'s **Severity** has three dimensions, namely $H$, $E$ and $R$.

- $H$ represents hardiness, force, size and/or resistance.
- $E$ represents excellence, cunning, finesse and/or wits.
- $R$ represents resolve, attunement, wealth, and/or resources.

Each of these dimensions have numbers assigned to them, which define how many *Effect* dice are used for different approaches towards overcoming the *Trinity*.











## Statblocks

NPC statblocks are defined mainly by their **Concepts** and **Attributes**. **Concepts** can be used as roleplay cues for the GM and as a theme for the NPC powers (if they have any). **Attributes** define mechanical prowess in three interaction dimensions: **Hard**, **Edge** and **Will**.

NPCs do not need to be balanced with characters, but the process below can help define relative balanced power levels for NPCs based on their attributes, which define their relative Level to other NPCs.

With **Concepts** and **Attributes**, augmented with **Calculated Stats** which are based on **Attributes** only, an NPC statblock is mostly ready for play. If the GM is inclined to put more work on it, choosing special abilities (preferably related to the **Concepts**) can add flavour to the NPC.

Simplify yml to target fwn4b template.

### Concepts
***Inspired by Godbound and Forge of Foes*** 

NPC statblocks defined with concepts are richer. Concepts should be related to their behaviours and (special) abilities. In general, two or three concept words are enough. Books like Godbound, Best Left Buried, D&D MMs (all versions), Forge of Foes, Nightmares Underneath, etc. have many examples of concepts and special abilities. A list of fantasy special abilities from Godbound is available in [Special abilities](README.md#Special%20abilities).

### Attributes and Level
***Inspired by Best Left Buried***

NPCs are defined by three attributes: **Hard**, **Edge** and **Will**. Attributes are abstraction of abilities, skills, characteristics and powers. They are the main driver of further calculated stats for social and combat mechanics.

- **Hard**: represents the NPC's physical prowess and toughness. Related actions are *violence, exert, intimidate*. Related to **physical** resistance.
- **Edge**: represents the NPC's gut brain and sagacity. Related actions are *finesse, sneak, notice*. Related to **evasion** resistance.
- **Will**: represents the NPC's intellect and resolve. Related actions are *learn, survive, command, sway*. Related to **mental** resistance.

Attributes have a die assigned to them, which is added as **Modifier** to any checks where they are relevant, including attacks.

| Attribute Value | Modifier Die |
| --------------- | ------------ |
| -1              | -1 (-1d2)   |
| 0               | 0            |
| 1               | +1 (+1d2)   |
| 2               | +d4          |
| 3               | +d6          |
| 4               | +d8           |
| 5               | +d10          |
| 6-9             | +d12          |
| 10+             | +d20          |

For passive values (i.e. **Difficulty Targets**) the die is rolled and added to 10 on d20 based systems or 5 to 2d6 based systems.

An NPC **Level**, also reflected on its Hit Dice (**HD**) encoding, is defined as
$$\text{Level} = \sum{(\text{Hard, Edge, Will})}$$

| Level | Degree of power                                             |
| ----- | ----------------------------------------------------------- |
| 0-1   | Ordinary people and small animals                           |
| 2-3   | Early heroes, fearless thugs & investigators, large animals |
| 4-5   | Veterans, elite groups, predators                           |
| 6-10  | Legendary mortals and world apex animals                    |
| 10+   | Transhumans and eldritch creatures                          |

### Calculated stats (autostats)
***Inspired by 5e's DMG, Forge of Foes, AD&D, Best Left Buried, Cairn, Knave, and the Without Number games***

The stats generation procedure below creates a statblock that is cohesive for their attribute distribution and estimated level. For a specific NPC, they should only serve as a guide, and can **and should** be changed.

**Armour**: The value shown on the statblock represents armour in two systems as "**AC** (**Protection**)".  **AC** is used for d20 systems with target **To Hit** values, whereas **Protection** is used for both 2d6 systems with target **To Hit** values (+7 to **Protection**) or subtracted from damage taken.
$$
\text{Armour} =
		\begin{cases}
		10+\min(4,\text{Hard})*2 + \min(4,\text{Edge}) &\text{AC systems}\\
		\min(4,\text{Hard}) + \lfloor\min(4,\text{Edge})/2\rfloor &\text{Protection systems}
		\end{cases}
$$

It is perfectly valid that an NPC has a suit of armour to increase its **AC** - in that case, ignore the guidance. 

Hit points (**HP**): Defined based on **Hard** and **Level** as below.
$$\text{HP} = (\text{Level} + \text{Hard}) \cdot d6$$

**Speed** depends on **Edge**. Multiple attacks capabilities can be informed by the NPC's **Speed**, but should be only available to **Melee** attacks.
$$
\text{Speed} = \sqrt{\text{Edge}}
$$

Attack damage (**Atk Dmg**) is defined by the weapon used. However, some NPCs would use brute force or spellcasting attacks, which are defined by the attributes **Hard** or **Will**. Will attacks are generally treated as spellcasting or intelligence driven attacks (i.e. artillery). For spellcasting attacks, consider requiring effort usage.
$$
\text{Atk Dmg} =
\begin{cases}
(\text{Hard} + 1) /2 \cdot d6 &\ Melee \\
(\text{Edge} + 1) /2 \cdot d6 &\ Ranged \\
\mathscr{L}(\theta d6 + \alpha | \text{Will} \cdot \text{Level} / 2)) &\ Effort 
\end{cases}$$

**Effort** is used to power special abilities NPCs *might* have. Effort is used as a modified [usage dice rule](https://nothingventured.obsidianportal.com/wikis/usage-dice). Instead of decreasing the die, once a 1 or 2 is rolled, no more effort is available to the NPC.  Defined by **Will** as below.
$$\text{Effort} = \mathscr{L}(d\theta | \text{Will}), \text{ for Will} \in \mathbb{N}$$

**Save** targets are $15$ unless specified differently. An attribute modifier is applied to the roll.

### Special Abilities

During creation, consider choosing a number of special abilities. One or two are sufficient for more generic NPCs, whereas a powerful Spellcaster can have many, to reflect their prowess. **Most special abilities require Effort to be used**.

A non-comprehensive list of special abilities, grouped by concept:

- **Alacrity**: Blindingly-fast strikes, Charges that hit everyone in passing, Snatching projectiles from the air, Dodging incoming blows, Tying up or snaring foes before they can react
- **Artifice**: Eldritch guns or projectile weapons, Hurled explosives, Mechanised armour, Automaton minions, Impairing rays or auras
- **Beasts**: Swarms of attacking vermin, Transformation into bestial war-shape, Impervious scales or shell, inhuman vitality, Clouds of musk or debilitating venom  
- **Bow**: Bolt penetrating multiple foes, Hyper-accurate archery, Shooting projectiles out of the air, Firing to make a melee assailant pull back, Shooting important gear or making precise debilitating shots
- **Command**: Commanding a foe to commit suicide, Ordering a group to attack each other, Commanding an assailant to halt, Ordering bystanders to be human shields, Commands that linger and force listeners to resist them for several rounds  
- **Death**: Cause death to a living target, Drain the life from a group, Fuel healing with vampiric force, Defy wounds that should cause death, Compel the spirits of the dead to impair foes  
- **Deception**: Backstab a victim from surprise, Trick foes into attacking each other, Hide behind illusions, Turn invisible, Confuse and impair targets  
- **Earth**: Hurl stones, Kill groups with sudden stone spikes or gnashing cracks, Exhibit obduracy of stone, Summon stone barriers against foes, Trap or impair foes with clinging rock, toxic earth vapours, or sudden mud
- **Endurance**: Strike foes with unrelenting vigour, Leap into a group to let their blows pass through you and into each other, Contemptuously ignore hits, Fight on regardless of wounds, Exhaust enemies with unnaturally relentless attacks  
- **Fertility**: Induce hideous cancers on a foe, Strangle a group with sudden plant growth, Conjure plants to shield you, Spawn minions to defend you, Snare or poison foes with obedient plants  
- **Fire**: Cause a foe to spontaneously combust, Hurl balls of fire at groups, Melt incoming attacks, Drive foes back with a wall of fire, Scorch, suffocate, and blind foes with heat and light  
- **Health**: Strike a person down with a sudden lethal disease, Infect a group with a hideous plague, Instantly heal from a wound, Regrow lost or damaged body parts, Infect with disease or siphon health from a foe  
- **Journeying**: Bring a distant calamity to the foe, Force a group into the way of some natural hazard, Be elsewhere and away from a blow, Bring allies from afar to defend you, Make foes lost and wandering even in familiar surrounds
- **Knowledge**: Blast a victim’s brain with unendurable insight, Overload a group with incapacitating knowledge, Be aware of where to stand to avoid an attack, Know how to block a strike, Impair a victim’s understanding of the situation
- **Luck**: Kill someone with a ridiculously implausible accident, Set a group accidentally murdering each other with their blows, Luckily avoid an attack, Their foe fumbles the assault, Enemies suffer impairment from bad luck
- **Might**: Smash a foe with tremendous strength, Hurl something big at a cluster of enemies, Leap vast distances to escape or engage, Create barriers to enemies by toppling obstacles in their paths
- **Night**: Dissolve a foe into darkness, Melt a group into fading shadows, Cloak in defensive shadows, Disappear into the darkness, Blind foes with primal night
- **Passion**: Enslave an enemy with an overwhelming sensation of love, Daze a group by sapping all desire from them, Force bystanders to attack by infusing them with focused rage, Send enemies scattering by appearing as an eidolon of unendurable terror
- **Sea**: Blast a victim with high-pressure water, Drown a group in cling- ing water, Deflect blows with watery shields, Flow like liquid around an attack, Drag and impair foes with flowing currents
- **Sky**: Smite a target with lightning, Tumble a group with raging winds, Turn aside attacks with gusts of air, Fly out of the range of attacks, Beat down foes with rain, hail, and storms
- **Sorcery**: Blast a victim with an eldritch bolt, Conjure a foe to assault a group, Invoke a defensive shield, Summon a meat-shield minion, Curse victims with magical impairment
- **Sun**: Ignite an enemy with solar light, Scatter a group with a torrent of killing radiance, Dazzle an attacker and force them to miss, Melt or drive back an attack, Blind and exhaust foes with terrible light
- **Sword**: Skewer a foe in melee, Leap into a group and slaughter them all with a few sweeping strokes, Parry an attack, Redirect a blow, Cut straps, slash tendons, or knock the breath out of foes
- **Time**: Bring a future death to a foe, Slaughter a group with future wounds, Foretell an attack in time to dodge, Slow an attack in time to evade it, Hinder foes by slowing time or foretelling their actions
- **Wealth**: Bury a target in heavy wealth, Hurl molten gold or jagged diamond spikes, Bribe a group to kill each other, Pay spirits to de- fend you, Create barrier of gold, Impair targets with suddenly-failing material possessions

### Conversions
***To be reviewed after changing from version 3 to 4.***

#### From D&D 5e

Look at equivalent from Those Outside the walls. If there is no equivalent, Convert to **Level** based on CR as

$$
\text{Level} =
		\begin{cases}
		\text{CR} * 2 &\text{if $ CR \le 6$}\\
		\text{CR} + 6 &\text{if $ CR \ge 7$}
		\end{cases}
$$
Distribute **Brawl**, **Wit** and **Will** based on attribute modifiers. **HP**, **Saves** and **Effort** should be left as calculated by autostats (5e versions are not power-compatible). All the other stats can be defined either by autostats or the original 5e statblocks. A few special powers and traits should be copied from the original 5e statblock.
#### From Those Outside The Walls

Convert HD to Level, 1:1. Distribute **Brawl**, **Wit** and **Will** based on:

- Attack damage and shock for **Brawl**
- Instinct and skill for **Wit**
- Morale for **Will**

**HP**, **Saves** and **Effort** should be left as calculated by autostats (WN versions are not power-compatible). All the other stats can be defined either by autostats or the original WN statblocks. A few special powers and traits should be copied from the original WN statblock.
#### From Shadowdark and Nightmares 

...


#### From Best Left Buried



# Trinity Challenges

**Trinity Challenges** integrates *Terran Engine*'s **Challenges** and *fwn4-autostats* statistics. **Trinity Challenge**s are designed to be usable with `d20` and `2d6` based games, as well as **Terran Engine**.

When creating a **Trinity Challenge**, choose a **Name** and **Concept**. and assign values for the three interaction **Dimensions**: `HARD`, `EDGE`, and `WILL`. While **Concepts** can be used as one line descriptors and theme for the **Challenge**, the three **Dimensions** define its mechanical prowess. The `Statblock` contains other entries for powers, drives, roleplay cues, etc. These are extra details and are optional.

**Challenges** do not need to be balanced with characters, but the process below can help define relative balanced power levels for **Challenges** based on their **Dimensions**, which define their relative `Level` to other **Challenges**.


### Concepts
***Inspired by Godbound and Forge of Foes*** 

NPC statblocks defined with concepts are richer. Concepts should be related to their behaviours and (special) abilities. In general, two or three concept words are enough. Books like Godbound, Best Left Buried, D&D MMs (all versions), Forge of Foes, Nightmares Underneath, etc. have many examples of concepts and special abilities. A list of fantasy special abilities from Godbound is available in [Special abilities](README.md#Special%20abilities).

### Attributes and Level
***Inspired by Best Left Buried***

NPCs are defined by three attributes: **Hard**, **Edge** and **Will**. Attributes are abstraction of abilities, skills, characteristics and powers. They are the main driver of further calculated stats for social and combat mechanics.

- **Hard**: represents the NPC's physical prowess and toughness. Related actions are *violence, exert, intimidate*. Related to **physical** resistance.
- **Edge**: represents the NPC's gut brain and sagacity. Related actions are *finesse, sneak, notice*. Related to **evasion** resistance.
- **Will**: represents the NPC's intellect and resolve. Related actions are *learn, survive, command, sway*. Related to **mental** resistance.

Attributes have a die assigned to them, which is added as **Modifier** to any checks where they are relevant, including attacks.

| Attribute Value | Modifier Die |
| --------------- | ------------ |
| -1              | -1 (-1d2)   |
| 0               | 0            |
| 1               | +1 (+1d2)   |
| 2               | +d4          |
| 3               | +d6          |
| 4               | +d8           |
| 5               | +d10          |
| 6-9             | +d12          |
| 10+             | +d20          |

For passive values (i.e. **Difficulty Targets**) the die is rolled and added to 10 on d20 based systems or 5 to 2d6 based systems.

An NPC **Level**, also reflected on its Hit Dice (**HD**) encoding, is defined as
$$\text{Level} = \sum{(\text{Hard, Edge, Will})}$$

| Level | Degree of power                                             |
| ----- | ----------------------------------------------------------- |
| 0-1   | Ordinary people and small animals                           |
| 2-3   | Early heroes, fearless thugs & investigators, large animals |
| 4-5   | Veterans, elite groups, predators                           |
| 6-10  | Legendary mortals and world apex animals                    |
| 10+   | Transhumans and eldritch creatures                          |

### Calculated stats (autostats)
***Inspired by 5e's DMG, Forge of Foes, AD&D, Best Left Buried, Cairn, Knave, and the Without Number games***

The stats generation procedure below creates a statblock that is cohesive for their attribute distribution and estimated level. For a specific NPC, they should only serve as a guide, and can **and should** be changed.

**Armour**: The value shown on the statblock represents armour in two systems as "**AC** (**Protection**)".  **AC** is used for d20 systems with target **To Hit** values, whereas **Protection** is used for both 2d6 systems with target **To Hit** values (+7 to **Protection**) or subtracted from damage taken.
$$
\text{Armour} =
		\begin{cases}
		10+\min(4,\text{Hard})*2 + \min(4,\text{Edge}) &\text{AC systems}\\
		\min(4,\text{Hard}) + \lfloor\min(4,\text{Edge})/2\rfloor &\text{Protection systems}
		\end{cases}
$$

It is perfectly valid that an NPC has a suit of armour to increase its **AC** - in that case, ignore the guidance. 

Hit points (**HP**): Defined based on **Hard** and **Level** as below.
$$\text{HP} = (\text{Level} + \text{Hard}) \cdot d6$$

**Speed** depends on **Edge**. Multiple attacks capabilities can be informed by the NPC's **Speed**, but should be only available to **Melee** attacks.
$$
\text{Speed} = \sqrt{\text{Edge}}
$$

Attack damage (**Atk Dmg**) is defined by the weapon used. However, some NPCs would use brute force or spellcasting attacks, which are defined by the attributes **Hard** or **Will**. Will attacks are generally treated as spellcasting or intelligence driven attacks (i.e. artillery). For spellcasting attacks, consider requiring effort usage.
$$
\text{Atk Dmg} =
\begin{cases}
(\text{Hard} + 1) /2 \cdot d6 &\ Melee \\
(\text{Edge} + 1) /2 \cdot d6 &\ Ranged \\
\mathscr{L}(\theta d6 + \alpha | \text{Will} \cdot \text{Level} / 2)) &\ Effort 
\end{cases}$$

**Effort** is used to power special abilities NPCs *might* have. Effort is used as a modified [usage dice rule](https://nothingventured.obsidianportal.com/wikis/usage-dice). Instead of decreasing the die, once a 1 or 2 is rolled, no more effort is available to the NPC.  Defined by **Will** as below.
$$\text{Effort} = \mathscr{L}(d\theta | \text{Will}), \text{ for Will} \in \mathbb{N}$$

**Save** targets are $15$ unless specified differently. An attribute modifier is applied to the roll.

### Special Abilities

During creation, consider choosing a number of special abilities. One or two are sufficient for more generic NPCs, whereas a powerful Spellcaster can have many, to reflect their prowess. **Most special abilities require Effort to be used**.

A non-comprehensive list of special abilities, grouped by concept:

- **Alacrity**: Blindingly-fast strikes, Charges that hit everyone in passing, Snatching projectiles from the air, Dodging incoming blows, Tying up or snaring foes before they can react
- **Artifice**: Eldritch guns or projectile weapons, Hurled explosives, Mechanised armour, Automaton minions, Impairing rays or auras
- **Beasts**: Swarms of attacking vermin, Transformation into bestial war-shape, Impervious scales or shell, inhuman vitality, Clouds of musk or debilitating venom  
- **Bow**: Bolt penetrating multiple foes, Hyper-accurate archery, Shooting projectiles out of the air, Firing to make a melee assailant pull back, Shooting important gear or making precise debilitating shots
- **Command**: Commanding a foe to commit suicide, Ordering a group to attack each other, Commanding an assailant to halt, Ordering bystanders to be human shields, Commands that linger and force listeners to resist them for several rounds  
- **Death**: Cause death to a living target, Drain the life from a group, Fuel healing with vampiric force, Defy wounds that should cause death, Compel the spirits of the dead to impair foes  
- **Deception**: Backstab a victim from surprise, Trick foes into attacking each other, Hide behind illusions, Turn invisible, Confuse and impair targets  
- **Earth**: Hurl stones, Kill groups with sudden stone spikes or gnashing cracks, Exhibit obduracy of stone, Summon stone barriers against foes, Trap or impair foes with clinging rock, toxic earth vapours, or sudden mud
- **Endurance**: Strike foes with unrelenting vigour, Leap into a group to let their blows pass through you and into each other, Contemptuously ignore hits, Fight on regardless of wounds, Exhaust enemies with unnaturally relentless attacks  
- **Fertility**: Induce hideous cancers on a foe, Strangle a group with sudden plant growth, Conjure plants to shield you, Spawn minions to defend you, Snare or poison foes with obedient plants  
- **Fire**: Cause a foe to spontaneously combust, Hurl balls of fire at groups, Melt incoming attacks, Drive foes back with a wall of fire, Scorch, suffocate, and blind foes with heat and light  
- **Health**: Strike a person down with a sudden lethal disease, Infect a group with a hideous plague, Instantly heal from a wound, Regrow lost or damaged body parts, Infect with disease or siphon health from a foe  
- **Journeying**: Bring a distant calamity to the foe, Force a group into the way of some natural hazard, Be elsewhere and away from a blow, Bring allies from afar to defend you, Make foes lost and wandering even in familiar surrounds
- **Knowledge**: Blast a victim’s brain with unendurable insight, Overload a group with incapacitating knowledge, Be aware of where to stand to avoid an attack, Know how to block a strike, Impair a victim’s understanding of the situation
- **Luck**: Kill someone with a ridiculously implausible accident, Set a group accidentally murdering each other with their blows, Luckily avoid an attack, Their foe fumbles the assault, Enemies suffer impairment from bad luck
- **Might**: Smash a foe with tremendous strength, Hurl something big at a cluster of enemies, Leap vast distances to escape or engage, Create barriers to enemies by toppling obstacles in their paths
- **Night**: Dissolve a foe into darkness, Melt a group into fading shadows, Cloak in defensive shadows, Disappear into the darkness, Blind foes with primal night
- **Passion**: Enslave an enemy with an overwhelming sensation of love, Daze a group by sapping all desire from them, Force bystanders to attack by infusing them with focused rage, Send enemies scattering by appearing as an eidolon of unendurable terror
- **Sea**: Blast a victim with high-pressure water, Drown a group in cling- ing water, Deflect blows with watery shields, Flow like liquid around an attack, Drag and impair foes with flowing currents
- **Sky**: Smite a target with lightning, Tumble a group with raging winds, Turn aside attacks with gusts of air, Fly out of the range of attacks, Beat down foes with rain, hail, and storms
- **Sorcery**: Blast a victim with an eldritch bolt, Conjure a foe to assault a group, Invoke a defensive shield, Summon a meat-shield minion, Curse victims with magical impairment
- **Sun**: Ignite an enemy with solar light, Scatter a group with a torrent of killing radiance, Dazzle an attacker and force them to miss, Melt or drive back an attack, Blind and exhaust foes with terrible light
- **Sword**: Skewer a foe in melee, Leap into a group and slaughter them all with a few sweeping strokes, Parry an attack, Redirect a blow, Cut straps, slash tendons, or knock the breath out of foes
- **Time**: Bring a future death to a foe, Slaughter a group with future wounds, Foretell an attack in time to dodge, Slow an attack in time to evade it, Hinder foes by slowing time or foretelling their actions
- **Wealth**: Bury a target in heavy wealth, Hurl molten gold or jagged diamond spikes, Bribe a group to kill each other, Pay spirits to de- fend you, Create barrier of gold, Impair targets with suddenly-failing material possessions

### Conversions
***To be reviewed after changing from version 3 to 4.***

#### From D&D 5e

Look at equivalent from Those Outside the walls. If there is no equivalent, Convert to **Level** based on CR as

$$
\text{Level} =
		\begin{cases}
		\text{CR} * 2 &\text{if $ CR \le 6$}\\
		\text{CR} + 6 &\text{if $ CR \ge 7$}
		\end{cases}
$$
Distribute **Brawl**, **Wit** and **Will** based on attribute modifiers. **HP**, **Saves** and **Effort** should be left as calculated by autostats (5e versions are not power-compatible). All the other stats can be defined either by autostats or the original 5e statblocks. A few special powers and traits should be copied from the original 5e statblock.
#### From Those Outside The Walls

Convert HD to Level, 1:1. Distribute **Brawl**, **Wit** and **Will** based on:

- Attack damage and shock for **Brawl**
- Instinct and skill for **Wit**
- Morale for **Will**

**HP**, **Saves** and **Effort** should be left as calculated by autostats (WN versions are not power-compatible). All the other stats can be defined either by autostats or the original WN statblocks. A few special powers and traits should be copied from the original WN statblock.
#### From Shadowdark and Nightmares 

...


#### From Best Left Buried


Effort = Can use 10 Disposition to use an effect.





- [ ] Exploding 1d
- [ ] Effort uses Disposition (5 disposition?)
- [ ] Simplify yml to target fwn4b template.



# Terra Campaigns NPC generation
***Procedural creation and documentation for playable NPCs***

The NPC generation procedure (and generators) on this folder are divided into two modules: `npcGen.R` and `autostatsGen`.  The first is responsible for generating a NPC's personality and playable cues for the GM, while the second generates statblocks using a 3-attribute definition.

## NPC Gen

The procedural generator leverages assorted NPC generation tables, from multiple games, mixed and matched with not a lot of rigour. The output in yaml is ready to be used in Obsidian's starblocks.

## Statblocks

NPC statblocks are defined mainly by their **Concepts** and **Attributes**. **Concepts** can be used as roleplay cues for the GM and as a theme for the NPC powers (if they have any). **Attributes** define mechanical prowess in three interaction dimensions: **Hard**, **Edge** and **Will**.

NPCs do not need to be balanced with characters, but the process below can help define relative balanced power levels for NPCs based on their attributes, which define their relative Level to other NPCs.

With **Concepts** and **Attributes**, augmented with **Calculated Stats** which are based on **Attributes** only, an NPC statblock is mostly ready for play. If the GM is inclined to put more work on it, choosing special abilities (preferably related to the **Concepts**) can add flavour to the NPC.

Simplify yml to target fwn4b template.

### Concepts
***Inspired by Godbound and Forge of Foes*** 

NPC statblocks defined with concepts are richer. Concepts should be related to their behaviours and (special) abilities. In general, two or three concept words are enough. Books like Godbound, Best Left Buried, D&D MMs (all versions), Forge of Foes, Nightmares Underneath, etc. have many examples of concepts and special abilities. A list of fantasy special abilities from Godbound is available in [Special abilities](README.md#Special%20abilities).

### Attributes and Level
***Inspired by Best Left Buried***

NPCs are defined by three attributes: **Hard**, **Edge** and **Will**. Attributes are abstraction of abilities, skills, characteristics and powers. They are the main driver of further calculated stats for social and combat mechanics.

- **Hard**: represents the NPC's physical prowess and toughness. Related actions are *violence, exert, intimidate*. Related to **physical** resistance.
- **Edge**: represents the NPC's gut brain and sagacity. Related actions are *finesse, sneak, notice*. Related to **evasion** resistance.
- **Will**: represents the NPC's intellect and resolve. Related actions are *learn, survive, command, sway*. Related to **mental** resistance.

Attributes have a die assigned to them, which is added as **Modifier** to any checks where they are relevant, including attacks.

| Attribute Value | Modifier Die |
| --------------- | ------------ |
| -1              | -1 (-1d2)   |
| 0               | 0            |
| 1               | +1 (+1d2)   |
| 2               | +d4          |
| 3               | +d6          |
| 4               | +d8           |
| 5               | +d10          |
| 6-9             | +d12          |
| 10+             | +d20          |

For passive values (i.e. **Difficulty Targets**) the die is rolled and added to 10 on d20 based systems or 5 to 2d6 based systems.

An NPC **Level**, also reflected on its Hit Dice (**HD**) encoding, is defined as
$$\text{Level} = \sum{(\text{Hard, Edge, Will})}$$

| Level | Degree of power                                             |
| ----- | ----------------------------------------------------------- |
| 0-1   | Ordinary people and small animals                           |
| 2-3   | Early heroes, fearless thugs & investigators, large animals |
| 4-5   | Veterans, elite groups, predators                           |
| 6-10  | Legendary mortals and world apex animals                    |
| 10+   | Transhumans and eldritch creatures                          |

### Calculated stats (autostats)
***Inspired by 5e's DMG, Forge of Foes, AD&D, Best Left Buried, Cairn, Knave, and the Without Number games***

The stats generation procedure below creates a statblock that is cohesive for their attribute distribution and estimated level. For a specific NPC, they should only serve as a guide, and can **and should** be changed.

**Armour**: The value shown on the statblock represents armour in two systems as "**AC** (**Protection**)".  **AC** is used for d20 systems with target **To Hit** values, whereas **Protection** is used for both 2d6 systems with target **To Hit** values (+7 to **Protection**) or subtracted from damage taken.
$$
\text{Armour} =
		\begin{cases}
		10+\min(4,\text{Hard})*2 + \min(4,\text{Edge}) &\text{AC systems}\\
		\min(4,\text{Hard}) + \lfloor\min(4,\text{Edge})/2\rfloor &\text{Protection systems}
		\end{cases}
$$

It is perfectly valid that an NPC has a suit of armour to increase its **AC** - in that case, ignore the guidance. 

Hit points (**HP**): Defined based on **Hard** and **Level** as below.
$$\text{HP} = (\text{Level} + \text{Hard}) \cdot d6$$

**Speed** depends on **Edge**. Multiple attacks capabilities can be informed by the NPC's **Speed**, but should be only available to **Melee** attacks.
$$
\text{Speed} = \sqrt{\text{Edge}}
$$

Attack damage (**Atk Dmg**) is defined by the weapon used. However, some NPCs would use brute force or spellcasting attacks, which are defined by the attributes **Hard** or **Will**. Will attacks are generally treated as spellcasting or intelligence driven attacks (i.e. artillery). For spellcasting attacks, consider requiring effort usage.
$$
\text{Atk Dmg} =
\begin{cases}
(\text{Hard} + 1) /2 \cdot d6 &\ Melee \\
(\text{Edge} + 1) /2 \cdot d6 &\ Ranged \\
\mathscr{L}(\theta d6 + \alpha | \text{Will} \cdot \text{Level} / 2)) &\ Effort 
\end{cases}$$

**Effort** is used to power special abilities NPCs *might* have. Effort is used as a modified [usage dice rule](https://nothingventured.obsidianportal.com/wikis/usage-dice). Instead of decreasing the die, once a 1 or 2 is rolled, no more effort is available to the NPC.  Defined by **Will** as below.
$$\text{Effort} = \mathscr{L}(d\theta | \text{Will}), \text{ for Will} \in \mathbb{N}$$

**Save** targets are $15$ unless specified differently. An attribute modifier is applied to the roll.

### Special Abilities

During creation, consider choosing a number of special abilities. One or two are sufficient for more generic NPCs, whereas a powerful Spellcaster can have many, to reflect their prowess. **Most special abilities require Effort to be used**.

A non-comprehensive list of special abilities, grouped by concept:

- **Alacrity**: Blindingly-fast strikes, Charges that hit everyone in passing, Snatching projectiles from the air, Dodging incoming blows, Tying up or snaring foes before they can react
- **Artifice**: Eldritch guns or projectile weapons, Hurled explosives, Mechanised armour, Automaton minions, Impairing rays or auras
- **Beasts**: Swarms of attacking vermin, Transformation into bestial war-shape, Impervious scales or shell, inhuman vitality, Clouds of musk or debilitating venom  
- **Bow**: Bolt penetrating multiple foes, Hyper-accurate archery, Shooting projectiles out of the air, Firing to make a melee assailant pull back, Shooting important gear or making precise debilitating shots
- **Command**: Commanding a foe to commit suicide, Ordering a group to attack each other, Commanding an assailant to halt, Ordering bystanders to be human shields, Commands that linger and force listeners to resist them for several rounds  
- **Death**: Cause death to a living target, Drain the life from a group, Fuel healing with vampiric force, Defy wounds that should cause death, Compel the spirits of the dead to impair foes  
- **Deception**: Backstab a victim from surprise, Trick foes into attacking each other, Hide behind illusions, Turn invisible, Confuse and impair targets  
- **Earth**: Hurl stones, Kill groups with sudden stone spikes or gnashing cracks, Exhibit obduracy of stone, Summon stone barriers against foes, Trap or impair foes with clinging rock, toxic earth vapours, or sudden mud
- **Endurance**: Strike foes with unrelenting vigour, Leap into a group to let their blows pass through you and into each other, Contemptuously ignore hits, Fight on regardless of wounds, Exhaust enemies with unnaturally relentless attacks  
- **Fertility**: Induce hideous cancers on a foe, Strangle a group with sudden plant growth, Conjure plants to shield you, Spawn minions to defend you, Snare or poison foes with obedient plants  
- **Fire**: Cause a foe to spontaneously combust, Hurl balls of fire at groups, Melt incoming attacks, Drive foes back with a wall of fire, Scorch, suffocate, and blind foes with heat and light  
- **Health**: Strike a person down with a sudden lethal disease, Infect a group with a hideous plague, Instantly heal from a wound, Regrow lost or damaged body parts, Infect with disease or siphon health from a foe  
- **Journeying**: Bring a distant calamity to the foe, Force a group into the way of some natural hazard, Be elsewhere and away from a blow, Bring allies from afar to defend you, Make foes lost and wandering even in familiar surrounds
- **Knowledge**: Blast a victim’s brain with unendurable insight, Overload a group with incapacitating knowledge, Be aware of where to stand to avoid an attack, Know how to block a strike, Impair a victim’s understanding of the situation
- **Luck**: Kill someone with a ridiculously implausible accident, Set a group accidentally murdering each other with their blows, Luckily avoid an attack, Their foe fumbles the assault, Enemies suffer impairment from bad luck
- **Might**: Smash a foe with tremendous strength, Hurl something big at a cluster of enemies, Leap vast distances to escape or engage, Create barriers to enemies by toppling obstacles in their paths
- **Night**: Dissolve a foe into darkness, Melt a group into fading shadows, Cloak in defensive shadows, Disappear into the darkness, Blind foes with primal night
- **Passion**: Enslave an enemy with an overwhelming sensation of love, Daze a group by sapping all desire from them, Force bystanders to attack by infusing them with focused rage, Send enemies scattering by appearing as an eidolon of unendurable terror
- **Sea**: Blast a victim with high-pressure water, Drown a group in cling- ing water, Deflect blows with watery shields, Flow like liquid around an attack, Drag and impair foes with flowing currents
- **Sky**: Smite a target with lightning, Tumble a group with raging winds, Turn aside attacks with gusts of air, Fly out of the range of attacks, Beat down foes with rain, hail, and storms
- **Sorcery**: Blast a victim with an eldritch bolt, Conjure a foe to assault a group, Invoke a defensive shield, Summon a meat-shield minion, Curse victims with magical impairment
- **Sun**: Ignite an enemy with solar light, Scatter a group with a torrent of killing radiance, Dazzle an attacker and force them to miss, Melt or drive back an attack, Blind and exhaust foes with terrible light
- **Sword**: Skewer a foe in melee, Leap into a group and slaughter them all with a few sweeping strokes, Parry an attack, Redirect a blow, Cut straps, slash tendons, or knock the breath out of foes
- **Time**: Bring a future death to a foe, Slaughter a group with future wounds, Foretell an attack in time to dodge, Slow an attack in time to evade it, Hinder foes by slowing time or foretelling their actions
- **Wealth**: Bury a target in heavy wealth, Hurl molten gold or jagged diamond spikes, Bribe a group to kill each other, Pay spirits to de- fend you, Create barrier of gold, Impair targets with suddenly-failing material possessions

### Conversions
***To be reviewed after changing from version 3 to 4.***

#### From D&D 5e

Look at equivalent from Those Outside the walls. If there is no equivalent, Convert to **Level** based on CR as

$$
\text{Level} =
		\begin{cases}
		\text{CR} * 2 &\text{if $ CR \le 6$}\\
		\text{CR} + 6 &\text{if $ CR \ge 7$}
		\end{cases}
$$
Distribute **Brawl**, **Wit** and **Will** based on attribute modifiers. **HP**, **Saves** and **Effort** should be left as calculated by autostats (5e versions are not power-compatible). All the other stats can be defined either by autostats or the original 5e statblocks. A few special powers and traits should be copied from the original 5e statblock.
#### From Those Outside The Walls

Convert HD to Level, 1:1. Distribute **Brawl**, **Wit** and **Will** based on:

- Attack damage and shock for **Brawl**
- Instinct and skill for **Wit**
- Morale for **Will**

**HP**, **Saves** and **Effort** should be left as calculated by autostats (WN versions are not power-compatible). All the other stats can be defined either by autostats or the original WN statblocks. A few special powers and traits should be copied from the original WN statblock.
#### From Shadowdark and Nightmares 

...


#### From Best Left Buried



### Magnitude

Sometimes you and the GM might need to compare different dimensions of *Magnitudes*.

| Tier                 | Area     | Party        | Duration | Range    | Harm Severity                                                                             |
| -------------------- | -------- | ------------ | -------- | -------- | ----------------------------------------------------------------------------------------- |
| $0$<br>**Poor**      | Closet   | $1$ person   | Moment   | Contact  | $d/2$ Minor injury. Sprains and bruising.                                                 |
| $1$<br>**Good**      | Corner   | $3$ people   | Scene    | Reach    | $1d$  Bleeding cuts and broken bones. Small explosions.                                   |
| $2$<br>**Excellent** | Room     | $10$ people  | Hour     | Nearby   | $2d$ Close contact with bodily destructive phenomena (such as fire, explosions, or acid). |
| $3$<br>**Impecable** | Wing     | $30$ people  | Day      | Far away | $3d$ Large explosions. Immersive contact with fi re and acid.                             |
| $4$<br>**Legendary** | Building | $100$ people | Week     | Remote   | $4d$ Usually fatal harm, often immediately.                                               |


Total war = combat = disposition from all HER