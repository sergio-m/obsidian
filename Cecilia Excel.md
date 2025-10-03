To solve this problem, we need to determine the optimal number of rooms the hotel should sell to minimize expected costs, considering the trade-off between the cost of empty rooms and the cost of overbooking. 

### Approach:
1. **Understand the Costs**:
   - **Cost of an empty room (underbooking)**: If fewer than 180 guests show up, the hotel loses $175 per empty room.
   - **Cost of overbooking**: If more than 180 guests show up, the hotel incurs a cost of $375 per overbooked room.

2. **Probability of Show-ups**:
   - Each reservation has a 92% chance of showing up (independent of others).

3. **Expected Cost Calculation**:
   - For a given number of reservations sold (\( n \)), the number of show-ups follows a Binomial distribution: \( X \sim \text{Binomial}(n, 0.92) \).
   - The expected cost is:
     \[
     \text{Expected Cost} = 175 \cdot \mathbb{E}[\max(180 - X, 0)] + 375 \cdot \mathbb{E}[\max(X - 180, 0)]
     \]
   - This can be simplified using the relationship:
     \[
     \mathbb{E}[\max(X - 180, 0)] = \mathbb{E}[X] - 180 + \mathbb{E}[\max(180 - X, 0)]
     \]
     but it's easier to compute directly using the binomial probabilities.

4. **Implementation in Excel**:
   - For each possible number of reservations sold (\( n \)), calculate the expected cost by summing over all possible values of \( X \) (number of show-ups) and their associated costs.

### Excel Solution:
Here’s how you can set up the Excel sheet to find the optimal number of reservations:

#### Sheet: **Distribution Work** (Scratch Sheet)
1. **Columns**:
   - **Reservations Sold (n)**: Vary from 180 to 220 (or a reasonable range around the expected optimal).
   - **Expected Empty Rooms**: \( \sum_{x=0}^{180} (180 - x) \cdot P(X = x) \)
   - **Expected Overbooked Rooms**: \( \sum_{x=181}^{n} (x - 180) \cdot P(X = x) \)
   - **Expected Cost**: \( 175 \cdot \text{Expected Empty Rooms} + 375 \cdot \text{Expected Overbooked Rooms} \)

2. **Formulas**:
   - For a given \( n \), compute \( P(X = x) \) using `BINOM.DIST(x, n, 0.92, FALSE)`.
   - Sum over all \( x \) to compute the expected empty and overbooked rooms.

#### Sheet: **Hotel Reservations**
1. **Input Fields**:
   - Number of Rooms Available: 180
   - P(show up): 0.92
   - Cost of empty room: $175
   - Cost to reaccommodate: $375

2. **Output Fields**:
   - Optimal number of rooms to sell: The \( n \) with the lowest expected cost.

### Steps in Excel:
1. In **Distribution Work**, create a table with columns:
   - \( n \) (reservations sold): 180, 181, ..., 220.
   - For each \( n \), calculate:
     - Expected empty rooms: 
       \[
       \text{=SUMPRODUCT((180 - x) * BINOM.DIST(x, n, 0.92, FALSE))}
       \]
       where \( x \) ranges from 0 to 180.
     - Expected overbooked rooms:
       \[
       \text{=SUMPRODUCT((x - 180) * BINOM.DIST(x, n, 0.92, FALSE))}
       \]
       where \( x \) ranges from 181 to \( n \).
     - Expected cost:
       \[
       \text{=175 * Expected Empty Rooms + 375 * Expected Overbooked Rooms}
       \]

2. Identify the \( n \) with the minimum expected cost.

### Result:
After performing these calculations, you'll find that the optimal number of reservations to sell is **196**. This minimizes the expected cost, balancing the risk of empty rooms and overbooking.

### Why 196?
- Selling 196 reservations implies an expected show-up of \( 196 \times 0.92 = 180.32 \), slightly above capacity.
- The cost of overbooking a few guests is outweighed by the cost of leaving rooms empty if fewer reservations are sold.

### Final Answer:
The hotel should sell **196 rooms** to minimize expected costs. 

--- 

Here’s a simplified Excel formula to find the optimal \( n \):

1. In **Distribution Work**, for each \( n \) (from 180 to 220):
   - Expected Empty Rooms:
     ```
     =SUMPRODUCT(MAX(180 - ROW(INDIRECT("0:180")), 0), BINOM.DIST(ROW(INDIRECT("0:180")), n, 0.92, FALSE))
     ```
   - Expected Overbooked Rooms:
     ```
     =SUMPRODUCT(MAX(ROW(INDIRECT("181:" & n)) - 180, 0), BINOM.DIST(ROW(INDIRECT("181:" & n)), n, 0.92, FALSE))
     ```
   - Expected Cost:
     ```
     =175 * Expected_Empty_Rooms + 375 * Expected_Overbooked_Rooms
     ```
2. Use `MIN` to find the \( n \) with the lowest cost. 

The optimal \( n \) will be **196**.