# Limits of Predictability in Human Mobility

> Under constrcution... 04.22/2024

### Research Problem:

To what extent human mobility is predictable?
(Note: )

### Research Method:

**Entropy Measurement**

1. The random Entropy: $S^{rand}_{i} = log_2{N_i}$, where N represents the number of distinct locations for a user.

2. The Temporal unrelatted Entropy: $S^{unc}_i = -\sum^{N_i}_j{p_i(j)}*log_2{p_i(j)}$, where $p(j)$ represents the probability of j in previous visitation by user i.

3. The actural Entropy: $S_i = -\sum^{Num_{T_i}}_1{P_i(T_
i)}*log_2{P_i(T_i)}$, where $T_i$ represents a consecutive temporal location pair in form of {$X_1,X_2$} for user i. And $P_i$ represents the probability of this pair.

**generally speaking, for each user, $S_i\leq S^{unc}_i\leq S^{rand}_{i}$** (larger diversity cause larger entropy)

**radius of gyration**

回旋半径，测度一个人的活动范围大小

**Π: measurement of predictability**

> Cannot fully understand the mathematic inference for this index

Π measures the limits of predictability of user based on historical information.
$Π_{max}$ shows the limit of the predictability of a user.

### Findings

1. Real uncertainty for a typical user's next-step whereabouts is $2^{0.8} = 1.74$.
   
![alt text](./figs/dis_entropy.png)

2. The distribution of **radius of gyration** presents a right-skewed pattern. Based on this pattern, we are intuitive to give an assumption that **the predictability of individuals should aslo follows a right-skewed distribution, similar to radius of gyration.**
   
![distribution of gyration](./figs/dis_gyration.png)

3. The distribution of predictability did not show a right-skwed distribution, indicating that those with higher movement diversity keeps a similar predictability as well as common publics. The distribution mainly focus on 0.93, which means that for most of people, their next_step location predictability is around 93%

![alt text](./figs/dis_pred.png)

4. The relationships between individual predictability and his rygation is: predictability decrease with rygation increase at first(0-10km), then predictability independent, and converge to around 0.90+.

### Intersting points

1. use comparison to prove that data completeness not need to be perfect. (by measuring entropy difference for those with perfect data by mannually deleting some data)

### Discussion

1. the predictability of common public are around 93%
   
2. from the distribution, only considering locations are not effective(both random or with probability). Temporal relationships play a great role in location prediction taks.
   
3. The hypothesis is fail: Individuals with higher rg, the predictability is lower. They have relationships at first but converge with rg>10km.