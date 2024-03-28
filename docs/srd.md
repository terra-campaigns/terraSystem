# System Reference Document
(`terra-v0.1.1`)

**Terra** is a rules light system focused on narrative, player agency and consequences. Only 6-sided dice are used, in two tones: **Light Dice** and **Dark Dice**.
## Taxonomy

- "You" and "Your" are used interchangeably to refer to players and their characters. For disambiguation "The Player" is used when referring to the player outside the context of their character.
- "Challenge" is used to represent anything that is antagonistic to you, be that an NPC, the environment, etc.
- Meta game names, stats and currencies are marked in **bold**.
- Book references are marked in *italic*, they might be accompanied by page ranges.
# Character creation

1. Always start with a **Name** and a **Concept**.
2. Roll for **Attributes**.
3. Calculate **HP** (hit points) and **Ego**.
4. Choose one **Advancement**.
## Concepts

`TBD`
## Attributes

**Attributes** are grouped in **Body** or **Mind** and **Power** or **Finesse**.

- **Body/Power**: represents physical strength, endurance and might.
- **Body/Finesse**: represents dexterity, precision and physical sagacity.
- **Mind/Power**: represents mental force, willpower and personality heft.
- **Mind/Finesse**: represents reasoning, understanding and mental sagacity. 

To determine **Attribute** values, roll 1d for each, and consult the table below. After rolling, you may swap two values.

| Attribute Roll |  1  | 2-3 | 4-5 |  6  |
| -------------- | :-: | :-: | :-: | :-: |
| **Stat Value** |  0  |  1  |  2  |  3  |

Your **Attributes** define the initial size of your **Dice Pool** when you are doing something that you are capable of, and have appropriate the equipment.

In certain conditions, you might lose **Attributes**. **Attribute** loss is permanent and when any attribute goes below 0 you are lost somehow.
## HP and Ego

You have two measures of survival: **HP** (hit points) and **Ego**.

**HP** (hit points) represent your health, disposition and fighting spirit. You lose **HP** when you are physically harmed. To determine your starting maximum **HP**, sum your **Body Attributes** and add 3.

**Ego** combines willpower, sanity and humanity. It is spent to increase dice pools and used to fuel some character **Advancements**. **Ego** is depleted when facing stressful situations or infectious environments. To determine your character's starting maximum **Ego**, sum your **Mind Attributes** and add 3.

The base rate of recovery is 1 **HP** per day. If you are being attended by someone, recover an addition **HP**. **Ego** does not recover with rest or care, but by taking a **Consequence**. When you take a **Consequence** your **Ego** recovers to its maximum.
# Character development

## Advancements

Every time PCs accumulate 8 XP, they gain an **Advancement**. Alongside an **Advancement**, a PC also gains +1 maximum **HP** and +1 maximum **Ego**.
### General advancements

- **Extra Attribute**: Gain +1 in one chosen **Attribute**. Limit is 2 in the first 10 advancements Limit is 3 thereafter.

`TBD`
## Consequences

`TBD`

# Rules

## Rolling the dice

Every time you try to overcome a **Challenge**, you will roll your **Dice Pool**. The baseline number of **Light Dice** in your **Dice Pool** is your appropriate **Attribute** for the intended action. With the GM, determine which **Attribute** it is.

Your **Dice Pool** can be modified in a number of ways:

- If you are in an advantageous position, roll **+1d (Light)**. A major advantageous position might give you **+2d (Light)**.
- If you are in an disadvantageous position, roll **-1d (Light)**. A major disadvantageous position might give you **-2d (Light)**.
- Roll **+1d (Light)** for each **Ego** you expend in the action.

Your **Dice Pool** can never have more than 4 **Light Dice**. If after adding and removing dice your **Dice Pool** is zero or lower, add **+1d (Dark)** to your **Dice Pool**.

The GM determines the **Challenge**, and add an appropriate number of **Dark Dice** to your **Dice Pool**.

After you roll, choose one **Light Die** to be your **Success Die** and one **Light Die** to be your **Effect Die**. If you only have one **Light Die** in your pool, this is your **Success Die**.

If your **Success Die** is:

- 1-3 you have failed, with complications: You fail and the challenge might **Retribute**.
- 4-5 you have succeeded, with complications: You accomplish your goal and apply your effect, but the challenge might **Retribute**.
- 6 you have completely succeeded: You accomplish your goal without **Retribution**.

Your **Effect Die** determines the effect of your action (damage, progress in a task, etc.). If you only have a **Success Die** (i.e. you rolled one single **Light Die**) your effect result is a "1".

The highest **Dark Die** is the **Challenge Retribution**.

**Effect** and **Retribution** are exploding dice. Every time the result is a natural 6, re-roll and accumulate the result. Equipment and conditions may modify **Effect** and **Retribution** results. The modified result does not affect dice explosion - which is only when a natural 6 occur.

## Effects

If you are in combat, different weapons modify the Effect Die in different ways. A few examples are:

| Weapon type   | Effect Die | Details                                                                                                      |
| ------------- | :--------: | ------------------------------------------------------------------------------------------------------------ |
| Light melee   |   **d3**   | Apply **Effects** before **Retributions**                                                                    |
| Medium melee  | Unmodified | Effect die is read as **d6+1** when held with both hands                                                     |
| Heavy melee   | Unmodified | Advantageous (**+1d**)<br>Apply **Retributions** before **Effects**<br>Two handed                            |
| Light ranged  | Unmodified |                                                                                                              |
| Medium ranged | Unmodified | Advantageous (**+1d**)<br>Expend all ammo when **Effect Die** explodes (one action to reload).<br>Two handed |
| Heavy ranged  | Unmodified | Major advantageous (**+2d**)<br>Require one action to ready before every shot<br>Two handed                  |
| Improvised    |   **d3**   | Disadvantageous (**-1d**)                                                                                    |
## Retributions

**Retributions** can be of three types: body harm, mind harm or **Challenge** fork.

Body harm **Retributions** impacts your **HP**. The armour you wear might modify the **Retribution Die**. Subtract the modified **Retribution** from your **HP**. If your **HP** reaches 0 you lose one to a random **Attribute**. You are unconscious and wake up with 1 **HP** after the scene ends. **Attribute** loss is permanent and when any attribute goes below 0 you die.

| Armour type | Retribution modifier | Details                                                      |
| ----------- | :------------------: | ------------------------------------------------------------ |
| Light       |          -1          |                                                              |
| Heavy       |          -2          | Disadvantageous (**-1d**) to run, observe, sneak, swim, etc. |
| Shield      |          -1          | Can be sacrificed to completely avoid the **Retribution**.   |

Mind harm **Retributions** impacts your **Ego**. If the **Retribution Die** is equal or higher than your current **Ego**, subtract one from your current **Ego**. If your **Ego** reaches 0 you are lost somehow. With the GM determine how your last scene goes.

**Challenge** fork **Retributions** are spawn from within an ongoing Challenge. They might be an encounter, an unexpected detour or some unlucky event. Consult the **Challenge** fork table.

| Retribution Roll   |   1-3   |    4-5    |  7-11   |    13+     |
| ------------------ | :-----: | :-------: | :-----: | :--------: |
| **Challenge** fork | Trivial | Dangerous | Serious | Formidable |

## Challenges

**Challenges** can be a fighting enemy, a rhetoric duel, an environment, etc. **Challenges** don't have **HP** or **Ego**. A generic measure of **Disposition** is used to determine how much **Effort** it takes to overcome a **Challenge**. Armours do not modify **Effects** applied to a **Challenge's Disposition**. Depending on the **Challenge**, more **Dark Dice** might be added to the **Dice Pool**.

| Challenge Level | Disposition | Retribution Dice | Examples                                                              |
| --------------- | ----------- | ---------------- | --------------------------------------------------------------------- |
| Trivial         | 1           | **d3**           | Unskilled adversaries, low height climb, known journey                |
| Dangerous       | 5           | **1d**           | Skilled adversaries, small explosions, troublesome journey            |
| Serious         | 10          | **2d**           | Expert adversareis, predator, close contact with fire or acid         |
| Formidable      | 15          | **3d**           | Human prime, apex predator, immersion in acid, large explosions       |
| Extreme         | 20          | **4d**           | Transhuman, often fatal environments, most difficult journey possible |

If multiple challenges gang up against you, increase the **Challenge Level** in one for each two additional challenges after the first.

Some challenges might be multifaceted. A bulky rival might be a Dangerous **Challenge** to fight against, but a Trivial **Challenge** to be convinced to ignore you.
# Appendices

## Book references


## Copyright

_This work is based on [Trophy](https://trophyrpg.com/), product of Jesse Ross and Hedgemaze Press, and licensed for our use under the [Creative Commons Attribution 4.0 License](https://creativecommons.org/licenses/by/4.0/). Trophy is adapted from Cthulhu Dark with permission of Graham Walmsley. Trophy is also based on [Blades in the Dark](http://www.bladesinthedark.com/), product of One Seven Design, developed and authored by John Harper, and licensed for our use under the [Creative Commons Attribution 3.0 Unported license](http://creativecommons.org/licenses/by/3.0/)._

_Trophy™ is a trademark of Hedgemaze Press. The trademark and “Rooted in Trophy” Logo are © Hedgemaze Press, and are used with permission._

![](https://i.imgur.com/Dc8H3RU.png)

*This work also draws inspiration on the [Best Left Buried Zine Edition](https://soulmuppet-store.co.uk/products/best-left-buried-zini-edition) (as well as any games that inspired it).*

