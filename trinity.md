### Challenges

Evaluate *Effects* as appropriate, if the *Risky Action* is part of a *Challenge*.

#### Effects {-}

*Effects* determines the quantitative result of your *Risky Actions* towards overcoming *Challenges*.
Examples of *Effects* are:

- Damage given,
- Convincing done,
- Distance covered,
- Weakness learned.

When you roll your *Risky Actions*, choose one die to be your *Effect* (generally the second highest, if the highest was used as *Precision*).
The *Effect* die is an exploding die (i.e. if the result is a $6$, keep rolling and accumulating the result).
The *Effect* is modified by the its Tier.
Your *Effect* is subtracted from the *Challenge* *Disposition*.

| Tier                 | Examples                                                               |
| :------------------- | ---------------------------------------------------------------------- |
| $-1e$<br>**Minor**   | Primitive tool<br>Weak argument or approach<br>Small weapons           |
| $\pm 0e$<br>**Base** | Fit for purpose tool;<br>Good argument or approach; <br>Medium weapons |
| $+1e$<br>**Major**   | Expert grade tool<br>Strong rationale or approach<br>Large weapons     |

#### Challenges {-}

Sometimes, multiple actions are required to overcome *Challenges*.
Examples of *Challenges* are

- fighting an enemy,
- duelling rhetorically,
- negotiating an environment,
- crawling a location,
- journeying.

*Challenges* have a descriptive **Name**.
*Challenges* are divided in **Tiers**, which define how much *Effect* they take to be overcame (**Disposition**), and how many *Effect* dice they use (**Severity**).

|                 | Tier           | Examples                                                             |
| --------------- | :------------- | -------------------------------------------------------------------- |
| **Trivial**     | $5$<br>$d/2$   | Unskilled adversaries, low height climb, known journey               |
| **Dangerous**   | $10$<br>$1d$   | Skilled adversaries, small predator, large prey, troublesome journey |
| **Serious**     | $20$<br>$2d$   | Expert adversaries, large predator, traverse fire or acid            |
| **Formidable**  | $30$<br>$3d$   | Human prime, apex predator, climbing the Everest                     |
| **Exceptional** | $40+$<br>$4d+$ | Transhuman, often fatal environments, heroic journeys                |

Some challenges might be multifaceted.
A bulky rival might be a Dangerous *Challenge* to fight against, but a Trivial *Challenge* to be convinced to ignore you.

When *Challenge Effects* are applied to you narratively, use the table.

|       | Consequence                    |
| :---: | ------------------------------ |
| $1:3$ | Something annoying happens.    |
| $4:5$ | Something troublesome happens. |
|  $6$  | Something devastating happens. |

When *Challenge* *Effects* are applied to you as damage your *Grit* might be reduced.
Subtract the armour rating from the *Effect*, and then reduce the remainder from your *Grit*.













*Trinity* is an expanded approach to *Challenges* for the **Terran Engine**.

Like *Challenges*, a *Trinity* have descriptive **Names** and numeric **Disposition** and **Severity**.
Unlike Challenges, a *Trinity*'s **Severity** has three dimensions, namely $HER$.

- $H$ represents hardiness, force, size and/or resistance. Higher $H$ inflicts more physical harm and lasts longer.
- $E$ represents excellence, cunning, swiftness and/or wits. Higher $E$ inflicts harm more frequently, silently or from further distance.
- $R$ represents resolve, attunement, wealth, and/or resources. Higher $R$ have more ample consequences and are resolute.

## Severity $HER$

Each **Severity** dimension ($HER$) have a number assigned to them, which define how many *Effect* dice are used for their consequences.

| $HER$ | Consequence | Comparable Harm                                                                     |
| ----- | ----------- | ----------------------------------------------------------------------------------- |
| $0$   | $d/2$       | Minor injury. Sprains and bruising.                                                 |
| $1$   | $1d$        | Bleeding cuts and broken bones. Small explosions.                                   |
| $2$   | $2d$        | Close contact with bodily destructive phenomena (such as fire, explosions, or acid) |
| $3$   | $3d$        | Large explosions. Immersive contact with fi re and acid.                            |
| $4$   | $4d$        | Usually fatal harm, often immediately.                                              |

Other proprieties can also be interpreted from the **Severity** dimensions ($HER$).

| $HER$ | Area           | Party        | Duration   | Range   |
| ----- | -------------- | ------------ | ---------- | ------- |
| $0$   | $1$ closet     | $1$ person   | Moments    | Contact |
| $1$   | $1$ room       | $3$ people   | $1$ scene  | Short   |
| $2$   | $1d$ rooms     | $10$ people  | $1d$ hours | Long    |
| $3$   | Small building | $30$ people  | $1$ day    | Sniper  |
| $4$   | Large building | $100$ people | $1$ week   | Extreme |

## Magnitude $M$

The sum of the Severity dimensions ($HER$) defines a *Trinity*'s **Magnitude** $M$. 

$$M = H + E + R$$

| $M$ | Degree of power                                             |
| --- | ----------------------------------------------------------- |
| $0$ | Ordinary people and small animals                           |
| $1$ | Early heroes, fearless thugs & investigators, large animals |
| $2$ | Veterans, elite groups, predators                           |
| $3$ | Legendary mortals and world apex animals                    |
| $4$ | Transhumans and eldritch creatures                          |

The same **Magnitude** $M$ should pose a similar challenge in a game, but thematically different because of the narrative aspects of a *Trinity* (descriptive **Name**) and distribution of **Severity** dimensions ($HER$)

## Disposition $D$

The **Disposition** $D$ of a *Trinity* is how much total *Effect* is required to overcome it completely.

$$
\begin{align}
D &= (2H + E + R) \times 7\\
  &= (2H + E + R) \times 2d \text{ (alternative)}
\end{align}
$$

When a *Trinity* **Disposition** $D$ is halved, it might choose to surrender.
Roll the $R$ dice as a **Risky Action**.

|       | Outcome                                                      |
| :---: | ------------------------------------------------------------ |
| $1:3$ | The *Trinity* surrenders.                                    |
| $4:5$ | The *Trinity* continues, but it might still surrender later. |
|  $6$  | The *Trinity* will not surrender.                            |
## Conversions

The first step to convert statblocks from other games into *Trinity* is to evaluate the target **Magnitude** $M$.

From OSR games it is as simple as

$$M = (\text{HD | Level})/2$$

From 5e

$$
M =
\begin{cases}
\text{CR} &\text{if $ CR \le 6$}\\
\text{CR}/2 + 3 &\text{if $ CR \gt 6$}
\end{cases}
$$

Then, from the available stats distribute $M$ into $HER$. Everything else should be interpreted as narrative descriptions of how a *Trinity* will act.

## Trinity in other games




The simple approach to *Trinity* can be used in other games.

An approach for $d20$ and $2d6$-based systems is proposed below.

| Stat            | $d20$                                 | $2d6$            |
| --------------- | ------------------------------------- | ---------------- |
| Level \| HD     | $M\times 2$                           |                  |
| Hit Points      | $D$                                   |                  |
| Modifier (Mod)  | $+2d[2HER]$                           | $+1d[2HER]$      |
| DC \| TN        | $10 + \text{Mod}$                     | $7 + \text{Mod}$ |
| AC              | $10 + \text{Mod} [\text{ best}(H,E)]$ |                  |
| # Attacks       | $E\times$                             |                  |
| Physical Damage | $[HE]d6$                              |                  |
| Magical Damage  | $R^2$                                 |                  |
| Effort die      | $d[2R]$, ends on a $1$                |                  |
| Save            | $16+$                                 |                  |





Skills



|            | Var1                       |
| :--------- | :------------------------- |
| Clergy     | Cultures, Administration   |
| Bureaucrat | Liaison, Administration    |
| Trainer    | Athletics, Administration  |
| Agent      | Violence, Administration   |
|            | Survival, Administration   |
| Coder      | Technology, Administration |
|            | Vehicles, Administration   |
|            | Sciences, Administration   |
| Artist     | Liaison, Cultures          |
|            | Athletics, Cultures        |
|            | Violence, Cultures         |
| Criminal   | Survival, Cultures         |
|            | Technology, Cultures       |
|            | Vehicles, Cultures         |
|            | Sciences, Cultures         |
| Dilettante | Athletics, Liaison         |
| Protector  | Violence, Liaison          |
| Disciple   | Survival, Liaison          |
| Fixer      | Technology, Liaison        |
|            | Vehicles, Liaison          |
| Academic   | Sciences, Liaison          |
|            | Violence, Athletics        |
| Spy        | Survival, Athletics        |
|            | Technology, Athletics      |
| **Racer**  | Vehicles, Athletics        |
|            | Sciences, Athletics        |
| Protector  | Survival, Violence         |
|            | Technology, Violence       |
|            | Vehicles, Violence         |
|            | Sciences, Violence         |
|            | Technology, Survival       |
| Traveller  | Vehicles, Survival         |
|            | Sciences, Survival         |
| Mechanic   | Vehicles, Technology       |
| Scientist  | Sciences, Technology       |
|            | Sciences, Vehicles         |



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