# Limits of Predictability in Human Mobility

> Under constrcution... 04.22/2024

### Research Problem:

To what extent human mobility is predictable?
(Note: )

### Research Method:

**Entropy Measurement**

1. The random Entropy: $S^{rand}_{i} = log_2{N_i}$, where N represents the number of distinct locations for a user.
2. The Temporal unrelatted Entropy: $S^{unc}_i = -\sum^{N_i}_j{p_i(j)}*log_2{p_i(j)}$, where $p(j)$ represents the probability of j in previous visitation by user i.
3. The actural Entropy: $S_i =-\sum^{Num_{T_i}}_1{P_i(T_
i)}*log_2{P_i(T_i)}$, where $T_i$ represents a consecutive temporal location pair in form of {$X_1,X_2$} for user i. And $P_i$ represents the probability of this pair.

**radius of gyration**

回旋半径，测度一个人的活动范围大小

**generally speaking, for each user, $S_i \leq S^{unc}_i \leq S^{rand}_{i}$** (larger diversity cause larger entropy)

### Findings

1. Real uncertainty for a typical user's next-step whereabouts is $2^{0.8} = 1.74$.
2. The distribution of **radius of gyration** presents a right-skewed pattern. Based on this pattern, we are intuitive to give an assumption that **the predictability of individuals should aslo follows a right-skewed distribution, similar to radius of gyration.**
3.

### Intersting points

1. use comparison to prove that data completeness not need to be perfect. (by measuring entropy difference for those with perfect data by mannually deleting some data)

2.
