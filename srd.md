# Characters

1. With the other players, define a cohesive group concept.
2. Always start with a Name and an *Archetype*.
3. Roll for *Attributes* and assign *Skills*
4. Roll for *Grit* and *Ego.*
5. **Optional:** Choose one *Advancement.*

A character sheet is available [here](docs/assets/TerranSheet.pdf).

## Archetypes

You are defined by an `Archetype`, which encapsulates your background, concept and role within the narrative.
Each `Archetype` should offer an immediate grasp of your identity and behaviours.
It is expected you will evolve beyond these initial `Archetypes` towards unique narratives.

- **Hero**: Embodies courage and strength, often the protagonist fighting against the odds.
- **Mentor**: Provides guidance and wisdom, helping the hero on their journey.
- **Everyman**: Represents the common man, relatability and realism.
- **Innocent**: Embodies purity, optimism, and faith.
- **Ruler**: Exudes control, responsibility, and sovereignty.
- **Sage**: Seeks truth, knowledge, and wisdom.
- **Explorer**: Loves discovering new worlds, autonomy, and the freedom to find out who they are through exploration.
- **Outlaw**: Represents rebellion, breaking the rules, and fighting against the status quo.
- **Magician**: Transforms reality, embodies vision and imagination.
- **Lover**: Pursues connection, romance, and passion.
- **Jester**: Values joy, humor, and light-heartedness.
- **Caregiver**: Provides nurture, generosity, and compassion.

## Skills & Attributes

There are $6$ *Skills* that you can use to overcome obstacles.

- **Intuition**: track targets, understand creatures, care, survive.
- **Reason**: concentrate, think abstractly, build knowledge.
- **Finesse**: dextrous manipulation, precision, subtle misdirection.
- **Exertion**: apply physical force and power, melee.
- **Attunement**: get in the flow and tune the arcane or technology.
- **Influence**: compel obedience, socialise, influence.

Each *Skill* has a rating (from $0$ to $4$) that determine how many dice to roll when performing *Risky Actions.*
There is a limit for *Skills* rated above $2$.
This limit may be derived from your *Archetype*.

$$
\begin{split}
Skill > 2 = \begin{cases}
3 \text{ rated at } 3 \\
1 \text{ rated at } 4 ; 1 \text{ rated at } 3
\end{cases}
\end{split}
$$

*Attributes* are groupings of two *Skills* each.
Attributes also have ratings (from $0$ to $2$) that determine how many dice to roll when facing a *Risky Action* passively (Save).

- **Insight** *Skills*: Intuition, Reason
	- Saves: Perception & Awareness
- **Prowess** *Skills*: Finesse, Exertion
	- Saves: Fortitude & Reflexes 
- **Resolve** *Skills*: Attunement, Influence
	- Saves: Sanity, Stress & Courage

For each *Attribute* (**Prowess**, **Sagacity** and **Resolve**) roll $1d$ and consult the table below to determine how many points you have to distribute to their *Skills.*

|        | $1:3$ | $4:5$ | $6$ |
| :----- | :---: | :---: | :-: |
| Points |  $1$  |  $2$  | $3$ |

In certain conditions, you might permanently lose *Attribute* points.

## Grit & Ego

> *"It's about how hard you can get hit and keep moving forward"*
> (Rocky Balboa)

While *Grit* represents your physical disposition, *Ego* represents your resilience.

Roll $1d$ to determine your initial *Grit* maximum and initial *Ego.*
Advancements and conditions may change these numbers.

After a well fed and rested night, you recover $1d$ of *Grit* lost.
At any moment, you may choose to take a *Condition* and roll $1d$ to reset your *Ego.*

You lose *Grit* when you are physically harmed. 
When your *Grit* reaches $0$ you become wounded.
You have $3$ *Wound* tracks.
You choose what they mean narratively.
Beyond those, you are mortally wounded and will die if harmed.

You spend *Ego* when you push beyond yourself in *Risky Actions* or use some character *Advancements.*
When your *Ego* reaches $0$ you are lost somehow.
With the GM determine how your last scene goes.

## Advancements

`Advancements` can have any narrative reasoning you want.
The list below are examples of a simple framework for their in-game mechanics:

- **Eager**: When you reset your `Ego`, roll $+1d$ and keep the highest.
- **Die Hard**: Roll your `Grit` maximum with $+1d$. You can choose to keep this new maximum if it is higher than your current maximum.
- **Skill**: Gain $1$ in a *Skill*.
- **Specialist**: Choose a specific type of action. *Risky Actions* are done with $+1d$ with this specialisation. For a list of specialisations, check [Cepheus SRD's skill list](https://www.orffenspace.com/cepheus-srd/skills.html#available-skills-list).
- **Buff** or **Debuff:** Roll a **Resolve** `Skill` and `Dark Dice`. Apply your `Effect` as a **Buff** or **Debuff** consequence. You may divide the result in as many targets as you want. You can take this `Advancement` multiple times if you want to **Buff** and **Debuff** with different **Resolve** `Skills`.
- **Heal** or **Hurt**: Roll an **Insight** `Skill` and `Dark Dice`. Multiply your `Effect` by the number of `Ego` spent and use the result to **Heal** or **Hurt**. You may divide the result in as many targets as you want. You can take this `Advancement` multiple times if you want to **Heal** or **Hurt** with different **Insight** `Skills`.
- **Tough**: When unarmoured your **Armour** is $1$.
- **Bodyguard**: You can choose to take damage instead of one of your allies.
- **Sensory acuity**: You have $+1d$ on noticing things through a chosen sense.
- **Whirlwind**: In combat, roll a **Prowess** `Skill` and `Dark Dice`. If you are successful, deal one additional instance of `Effect` to a `Challenge` at range.
- **Retire**: With the GM decide how your story ends. Create a new character with half (rounded up) the number of `Advancements` you have now, including this one.
- **Fast**: When you roll, your `Effect` is always applied first.

## Conditions

At any moment in the game you can re-roll your `Ego` by taking a `Condition`.
The recovery of your inner strength often comes through confronting, enduring, and adapting to hardship.
These trials teach you to integrate the traumas that permanently transform your self, strengthening your resilience.
With the GM, determine the new `Condition` you have, and how to introduce it into the narrative.

`Conditions` are detrimental mechanically, but not necessarily negative in the narrative.
The list below can be used as a starting point.
With the GM you can adapt these or create new ones.

- **Fear-Driven Vigilance**: Fear instills a heightened sense of vigilance, making you more cautious. In situations related to the your fear, you have $-1d$
- **Obsessive Focus**: Your single-minded pursuit leads to significant personal development and expertise in a specific area, in detriment of others. Gain $+1$ Point in one `Skill` and $-1$ Point in two other `Skills`.
- **Inept**: For some reason you are always inept in a specific type of action. *Risky Actions* are done with $-1d$ with this specialisation. For a list of specialisations, check [Cepheus SRD's skill list](https://www.orffenspace.com/cepheus-srd/skills.html#available-skills-list)
- **Moral Reservations**: Your steadfast morality leads to a firm stance on certain issues. Actions that go against your moral code have $-1d$.
- **Compulsive Honesty**: You vow to always speak the truth.
- **Kleptomaniac**: You are unable to resist urges to steal items that you generally don't really need.
- **Battle-Scarred**: After some injury, you develop a scar. You might have lost part of a member, an eye, or something else that impacts you physically, intellectually or socially.
- **Protective Instinct**: You are genuinely concerned with your team's welfare, and become a reluctant leader. When an ally is in danger, you have $-1d$.
- **Estranged**: You lose the bond with someone you love or cherish. With the GM, agree the mechanical impact.
- **Slow**: When you roll, your `Effect` is always applied last.

## Equipment 

With the GM define which tags, ranges and `Effect` are appropriate for your weapons.
Weapons used outside their expected ranges roll with $-1d$.

The following short list of tags may be expanded with the GM.

- **Versatile**: $+1e$ when held two-handed.
- **Nimble**: `Effect` is applied first
- **Slaughter**: `Effect` die explode on $5+$

Armours act as buffers when you take damage from `Challenges`.
Subtract the armour modifier from the `Effect` before reducing your `Grit`

| Armour     | Modifier | Details                                            |
| ---------- | :------: | -------------------------------------------------- |
| **Light**  |   $-1$   |                                                    |
| **Heavy**  |   $-2$   | $-1d$ to run, observe, sneak, swim, etc.           |
| **Shield** |   $-1$   | Can be sacrificed to completely avoid an `Effect`. |

# Rules

## Risky Actions

When you are trying your chances at a `Risky Action`, say what you intend to do.
With the GM determine your appropriate `Attribute` or `Skill`.
Then gather 6-sided dice.

|                                | Dice Pool                                                                                                                                                                                                                 |
| :----------------------------: | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![](imgs/dice-light-6-sml.png) | Take a number of `Light Dice` equal to your applicable `Attribute` or `Skill`. If you are in an advantageous or precarious position, the GM may give you $\pm 1d$. You must always have between $0$ and $4$ `Light Dice`. |
| ![](imgs/dice-dark-6-sml.png)  | Take as many `Dark Dice` as you wish to risk `Ego` for pushing yourself for a success. For each `Dark Dice` that rolls equal or lower than your current `Ego`, decrease your `Ego` in one.                                |

Roll the dice and choose one die to be your `Precision` (generally the highest, but you might choose differently if you wish) and consult the table.

|       | Outcome                                                                                                                                                   |
| :---: | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| $1:3$ | You fail, and things get worse. With the GM describe the consequences. The GM may also allow you to succeed, but things will get worse in some other way. |
| $4:5$ | You succeed, but there’s some consequences. With the GM describe the complication and how you succeed.                                                    |
|  $6$  | You succeed. With the GM describe what happens.                                                                                                           |

Evaluate `Effects` as appropriate, if the `Risky Action` is part of a `Challenge`,

## Effects

`Effects` determines the quantitative result of your `Risky Actions` towards overcoming `Challenges`.
Examples of `Effects` are:

- Damage given,
- Convincing done,
- Distance covered,
- Weakness learned.

When you roll your `Risky Actions`, choose one die to be your `Effect` (generally the second highest, if the highest was used as `Precision`).
The `Effect` die is an exploding die (i.e. if the result is a $6$, keep rolling and accumulating the result).
The `Effect` you apply is never lower than the `Effect` level of your approach, regardless of the die outcome.
Consult the table below.

| Effect     | Level | Examples                                                                          |
| ---------- | :---: | --------------------------------------------------------------------------------- |
| Improvised | $1e$  | Makeshift tool;<br>Rock, pipe, punch.                                             |
| Weak       | $2e$  | Primitive tool;<br>Weak argument<br>Knife, staff                                  |
| Standard   | $3e$  | Fit for purpose tool;<br>Good argument; <br>Revolver, one-handed sword            |
| Strong     | $4e$  | Expert grade tool;<br>Strong rationale;<br>Autofire pistol, SMG, two-handed sword |
| Extreme    | $5e$  | Tech augmented expert grade tool;<br>Rifle, shotgun, large axe and sword          |
`Challenge` `Effects` (damage) applied to you reduces your `Grit`.
Subtract the armour rating from the `Effect`, and then reduce the remainder from your `Grit`.
Your `Effects` are subtracted directly from `Challenges` Disposition (i.e. Challenges do not have armour).

Sometimes `Challenge` `Effects` fork into new `Challenges` or consequences.
Extra `Challenges` might be an encounter, an unexpected detour, a hidden threat or some unlucky event.
Consequences, on the other hand, pose some additional difficulty on the next `Risky Action` roll related to the `Challenge`.

| Effect Roll     | $\mathbf{1:3}$ | $\mathbf{4:5}$ | $\mathbf{7:11}$ | $\mathbf{13:17}$ | $\mathbf{19+}$ |
| --------------- | :------------: | :------------: | :-------------: | :--------------: | :------------: |
| Extra Challenge |    Trivial     |   Dangerous    |     Serious     |    Formidable    |    Extreme     |
| Consequence     |  $\mathbf{-}$  |      $1d$      |      $2d$       |       $3d$       |     $4d+$      |

## Challenges

Sometimes, multiple actions are required to overcome `Challenges`.
Examples of `Challenges` are

- fighting an enemy,
- dueling rhetorically,
- negotiating an environment,
- crawling a location,
- journeying.

`Challenges` have disposition, which measures how much `Effect` they take to be overcame.
`Challenges` also have `Effect` dice that are applied to you as consequences of your `Risky Actions`.

| Challenge      | Disposition | Effect | Examples                                                                               |
| -------------- | :---------: | :----: | -------------------------------------------------------------------------------------- |
| **Trivial**    |     $5$     | $d/2$  | Unskilled adversaries, low height climb, known journey                                 |
| **Dangerous**  |    $10$     |  $1d$  | Skilled adversaries, small explosions, small predator, large prey, troublesome journey |
| **Serious**    |    $20$     |  $2d$  | Expert adversaries, large predator, close contact with fire or acid                    |
| **Formidable** |    $30$     |  $3d$  | Human prime, apex predator, immersion in acid, large explosions                        |
| **Extreme**    |    $40+$    | $4d+$  | Transhuman, often fatal environments, most difficult journeys                          |

If multiple challenges gang up against you, increase the `Challenge` in one for each two additional challenges after the first.

Some challenges might be multifaceted.
A bulky rival might be a Dangerous `Challenge` to fight against, but a Trivial `Challenge` to be convinced to ignore you.

### Montage

You and the GM might prefer to resolve a `Challenge` in one single roll.
That is possible by rolling the `Challenge Effect` prior to gathering your dice.
Apply the consequence modifier to your dice and roll your `Risky Action`.
You risk $2$ `Ego` for each `Dark Die` you use.
Your companions can also pool their `Ego` to help you.
This single roll determine the outcome of the entire `Challenge`.

It is not recommended to use `Montages` if the consequence of failure would be the death of someone.
On those cases, playing the `Challenge` as a longer one gives more manoeuvre space.

## Wounds

When your `Grit` reaches $0$ and you use all your `Wound` tracks you become mortally wounded, and will die if further harmed.
While mortally wounded you cannot gather `Light Die` for your `Risky Actions`.
You will die in minutes if not attended to.

If you survive a mortal wound, you develop a permanent consequence.
Roll $1d$ and consult the table below.
With the GM, describe it narrativelly.

|     | Consequence                                                            |
| :-: | ---------------------------------------------------------------------- |
| $1$ | No consequence this time                                               |
| $2$ | $-1$ **Prowess**, you die if it becomes $0$                            |
| $3$ | $-1$ **Sagacity**, you die if it becomes $0$                           |
| $4$ | $-1$ **Resolve**, you die if it becomes $0$                            |
| $5$ | When you re-roll your `Ego`, use $-1d$ from now on. Its minimum is $1$ |
| $6$ | Re-roll your `Grit` with $-1d$ from now on. Its minimum is $1$.        |

Each `Wound` track recovers through appropriate care and a week of rest.

## Experience

You get $2$ *Experience* for each session you play.
You gain $+1$ *Experience* per *Condition* you develop.

Each new *Advancement* costs the current number of *Advancements* times $2$ in *Experience*.
Decide with the GM how to carry this development out in the narrative.
When you gain a new *Advancement* you also re-roll your *Grit* and keep the maximum between the current $+1$ or the new value.

## Fortune die

When the GM wants to leave some decision to the dice, determine the chances and roll $1d$.

# Making a Game

**Terran Engine** is focuses on the grimdark aesthetics, which might not be the thematic choice of every game.

By adapting the `Archetypes` and `Advancements`, and reskinning `Ego` (and `Conditions`), other genres can easily be emulated. A few playtested examples are given. The Rules section can mostly be used as is.

## Ego in Pulp Fantasy

For the Pulp Fantasy genre, Ego can be used as a measure of how far the next climax is. Whenever relevant, the GM rolls one die. If the die is higher than the highest Ego of the Party, a climax event happens. After this climax, all Ego is restored to its original max.

