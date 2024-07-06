# Trinity

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
