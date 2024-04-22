# Limits of Predictability in Human Mobility

> Under construction... 04/22/2024

## Research Problem

To what extent is human mobility predictable?

## Research Method

### Entropy Measurement

1. **Random Entropy**: \( S^{rand}\_{i} = \log_2{N_i} \), where \( N \) represents the number of distinct locations for a user.

2. **Temporal Unrelated Entropy**: \( S^{unc}\_i = -\sum^{N_i}\_j{p_i(j) \cdot \log_2{p_i(j)}} \), where \( p(j) \) represents the probability of \( j \) in previous visitation by user \( i \).

3. **Actual Entropy**: \( S*i = -\sum^{Num*{T_i}}\_1{P_i(T_i) \cdot \log_2{P_i(T_i)}} \), where \( T_i \) represents a consecutive temporal location pair in the form of \( \{X_1, X_2\} \) for user \( i \). And \( P_i \) represents the probability of this pair.

Generally speaking, for each user, \( S*i \leq S^{unc}\_i \leq S^{rand}*{i} \) (larger diversity causes larger entropy)

### Radius of Gyration

Radius of gyration measures the extent of a person's mobility range.

### Π: Measurement of Predictability

> Cannot fully understand the mathematic inference for this index

\( Π \) measures the limits of predictability of a user based on historical information.
\( Π\_{max} \) shows the limit of the predictability of a user.

## Findings

1. Real uncertainty for a typical user's next-step whereabouts is \( 2^{0.8} = 1.74 \).

   ![Figure: Entropy Distribution](./figs/dis_entropy.png)

2. The distribution of the **radius of gyration** presents a right-skewed pattern. Based on this pattern, we intuitively assume that **the predictability of individuals should also follow a right-skewed distribution, similar to the radius of gyration**.

   ![Figure: Distribution of Gyration](./figs/dis_gyration.png)

3. The distribution of predictability does not show a right-skewed distribution, indicating that those with higher movement diversity maintain similar predictability as the general public. The distribution mainly focuses around 0.93, which means that for most people, their next-step location predictability is around 93%.

   ![Figure: Predictability Distribution](./figs/dis_pred.png)

4. The relationship between individual predictability and their radius of gyration is: predictability decreases with an increase in radius of gyration at first (0-10 km), then becomes independent, and converges to around 0.90+.

## Interesting Points

1. Use a comparison to prove that data completeness does not need to be perfect (by measuring the entropy difference for those with perfect data by manually deleting some data).

## Discussion

1. The predictability of the general public is around 93%.

2. From the distribution, it's evident that considering locations alone is not effective (both random or with probability). Temporal relationships play a significant role in location prediction tasks.

3. The hypothesis fails: Individuals with higher radius of gyration do not necessarily have lower predictability. They show a relationship at first but converge with a radius of gyration greater than 10 km.
