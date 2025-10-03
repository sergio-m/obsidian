We produce electronic chips that are used as an input in automobiles. We have acquired a new contract and need to increase our hourly production to produce 150 chips per hour. We would like you to decide how we allocate our capital and labor.

To produce a chip, we estimate our hourly production function to be Q = 5*(0.5*K1)(0.5*L1), where K is capital units that have

an hourly cost of $90 and L is labor units that we pay an hourly wage of $10. We currently charge our customers $50 per chip.

It has been awhile since I took my MBA Managerial Economics course, so I am struggling to determine the optimal allocation of labor (L) and capital (K) units per hour that are needed to minimize the cost of producing 150 chips per hour.

Can you please help us determine this optimal allociation of iniputs? Thank you!

If you don't mind, can you provide me with the following analysis:

1. ﻿﻿﻿How many capital units per hour should we plan to use to produce the needed 150 chips per hour?
2. ﻿﻿﻿How many labor units per hour should we plan to use to produce the needed 150 chips per hour?
3. ﻿﻿﻿What is our hourly profit for producing 150 chips per hour?


----

To determine the optimal allocation of labor (L) and capital (K) to produce 150 chips per hour at minimal cost, we can follow these steps:

### Given:
- **Production function**: \( Q = 5 \times (0.5 K)^{0.5} \times (0.5 L)^{0.5} \)
- **Simplify the production function**:
  \[
  Q = 5 \times (0.5 K)^{0.5} \times (0.5 L)^{0.5} = 5 \times 0.5^{0.5} K^{0.5} \times 0.5^{0.5} L^{0.5} = 5 \times 0.5 \times K^{0.5} L^{0.5} = 2.5 K^{0.5} L^{0.5}
  \]
  So, the simplified production function is:
  \[
  Q = 2.5 K^{0.5} L^{0.5}
  \]
- **Target output**: \( Q = 150 \) chips/hour
- **Cost of capital (K)**: $90 per unit per hour
- **Cost of labor (L)**: $10 per unit per hour
- **Price per chip**: $50

### Step 1: Solve for the relationship between K and L to produce Q = 150
Set \( Q = 150 \):
\[
2.5 K^{0.5} L^{0.5} = 150 \\
K^{0.5} L^{0.5} = 60 \\
(K L)^{0.5} = 60 \\
K L = 3600 \\
L = \frac{3600}{K}
\]

### Step 2: Minimize the cost function
The total cost (C) is:
\[
C = 90 K + 10 L
\]
Substitute \( L = \frac{3600}{K} \) into the cost function:
\[
C = 90 K + 10 \left( \frac{3600}{K} \right) = 90 K + \frac{36000}{K}
\]

To minimize cost, take the derivative of \( C \) with respect to \( K \) and set it to zero:
\[
\frac{dC}{dK} = 90 - \frac{36000}{K^2} = 0 \\
90 = \frac{36000}{K^2} \\
K^2 = \frac{36000}{90} = 400 \\
K = \sqrt{400} = 20
\]

Now, solve for \( L \):
\[
L = \frac{3600}{K} = \frac{3600}{20} = 180
\]

### Step 3: Verify production with \( K = 20 \) and \( L = 180 \)
\[
Q = 2.5 \times (20)^{0.5} \times (180)^{0.5} = 2.5 \times \sqrt{20 \times 180} = 2.5 \times \sqrt{3600} = 2.5 \times 60 = 150
\]
This confirms the solution satisfies the production target.

### Step 4: Calculate hourly profit
- **Revenue**: \( 150 \text{ chips} \times \$50/\text{chip} = \$7500 \)
- **Cost**: \( 90 \times 20 + 10 \times 180 = 1800 + 1800 = \$3600 \)
- **Profit**: \( \$7500 - \$3600 = \$3900 \)

### Answers:
1. **Capital units per hour (K)**: 20
2. **Labor units per hour (L)**: 180
3. **Hourly profit**: \$3,900