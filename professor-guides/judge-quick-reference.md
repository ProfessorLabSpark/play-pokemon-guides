# 🧭 Play! Pokémon Judge Quick Reference (Complete Edition)
A practical, scalable cheat sheet for Challenges, Cups, and mixed‑age League events.

---

# 1. Age Divisions Always Exist (Even in One Pod)
Even in a unified pod, TOM still treats:
- **Juniors**
- **Seniors**
- **Masters**

…as **separate divisions** for:
- Round count  
- Standings  
- Prizing  
- Championship Points  

Pairings may cross divisions; standings and prizing never do.

---

# 2. Swiss Rounds Are Based on the Largest Division (with ≥2 players)

| Players in a division | Swiss Rounds |
|----------------------|--------------|
| 1                    | 0 (auto‑1st) |
| 2–3                  | 2 |
| 4–8                  | 3 |
| 9–16                 | 4 |
| 17–32                | 5 |
| 33–64                | 6 |
| 65–128               | 7 |

**Round count = the highest number required by any division with ≥2 players.**

Example:  
2 Masters → 2 rounds  
8 Seniors → 3 rounds  
14 Juniors → 4 rounds  
**Event runs 4 rounds** (largest division = Juniors)

---

# 3. Drops Do NOT Change Round Count
Once Round 1 begins:
- Round count is **locked**
- Drops do not reduce rounds

---

# 4. TOM’s Real Tiebreaker Math (Not the Handbook Version)

## MW% (Match‑Win Percentage)
TOM uses **per‑round scoring**, not match points.

- Win → **1.0**  
- Tie → **0.5**  
- Loss → **0.0**  
- Bye → **ignored**



\[
\text{MW\%} = \text{average of per‑round values}
\]



Then:
- **Floor at 25%**
- **Internal rounding**

---

## OMW% (Opponents’ MW%)


\[
\text{OMW\%} = \text{average of opponents’ MW\%}
\]



Notes:
- Use **their** MW% (with 1/0.5/0 system)  
- Apply **25% floor** to each opponent  
- Ignore byes  

---

## OOWP (Opponents’ Opponents’ Win Percentage)


\[
\text{OOWP} = \text{average of opponents’ OMW\%}
\]



---

# 5. Mental Shortcut (Fastest Way to Check TOM)
Think of each round as:
- Win = **1**
- Tie = **0.5**
- Loss = **0**

Then:
- MW% = your average  
- OMW% = average of your opponents’ averages  
- OOWP = average of *their* opponents’ averages  

---

# 6. Prizing Rules (Division‑Based)

## Prize Pool Per Division


\[
\text{Prize Pool} = \text{Players in Division} \times \text{Packs per Player}
\]



Example (24‑player event, 2 packs each):
- Masters (2) → 4 packs  
- Seniors (8) → 16 packs  
- Juniors (14) → 28 packs  

---

# 7. Two Legal Prize Distribution Models

## **Method A — Participation + Top Cut (“Nice Method”)**
- Every player receives **1 guaranteed pack**
- Remaining packs go to top finishers

## **Method B — Pure Top Cut (“Typical Method”)**
- All packs go to top finishers  
- No guaranteed participation packs

Both are legal if:
- Announced before Round 1  
- Consistent within the division  
- Not based on age  

---

# 8. Proportional Prize Distribution Algorithms

These models scale cleanly and always sum to 100%.

---

## ⭐ Top 4 Prize Model (Sums to 100%)

| Place | Fraction |
|-------|----------|
| 1st   | 1/2 (50%) |
| 2nd   | 1/4 (25%) |
| 3rd   | 1/8 (12.5%) |
| 4th   | 1/8 (12.5%) |

Perfect for divisions of **4–16 players**.

---

## ⭐ Top 8 Prize Model (Corrected, Sums to 100%)

| Place | Fraction |
|-------|----------|
| 1st   | 32% |
| 2nd   | 20% |
| 3rd   | 12% |
| 4th   | 12% |
| 5th   | 6% |
| 6th   | 6% |
| 7th   | 6% |
| 8th   | 6% |

This is ideal for divisions of **17–32 players**.

---

# 9. Participation + Proportional Top Cut (Hybrid Method)
If using the Nice Method:

1. Give every player **1 pack**  
2. Put remaining packs into a pool  
3. Apply the proportional distribution to the remaining pool  

---

# 10. FULL WORKED EXAMPLE — 24‑Player Event

## Division Breakdown
- **Masters: 2 players → 4 packs**
- **Seniors: 8 players → 16 packs**
- **Juniors: 14 players → 28 packs**

---

## A. Masters (2 players → 4 packs)
Top cut = 1  
Participation = 2 packs  
Remaining = 2 packs  

Distribution:
- 1st → 2 remaining  
- 2nd → 0 remaining  
- Everyone → 1 participation  

**Final:**
- 1st: 3 packs  
- 2nd: 1 pack  

---

## B. Seniors (8 players → 16 packs)
Top cut = 4  
Participation = 8 packs  
Remaining = 8 packs  

Top 4 distribution of remaining 8:
- 1st → 4  
- 2nd → 2  
- 3rd → 1  
- 4th → 1  

Add participation:
- 1st → 5  
- 2nd → 3  
- 3rd → 2  
- 4th → 2  
- 5th–8th → 1 each  

---

## C. Juniors (14 players → 28 packs)
Top cut = 4 (since <17 players)  
Participation = 14 packs  
Remaining = 14 packs  

Top 4 distribution of remaining 14:
- 1st → 7  
- 2nd → 3.5 → **4**  
- 3rd → 1.75 → **2**  
- 4th → 1.75 → **2**  

Add participation:
- 1st → 8  
- 2nd → 5  
- 3rd → 3  
- 4th → 3  
- 5th–14th → 1 each  

---

# 11. One‑Line Summary
**Divisions determine rounds and prizing; TOM determines tiebreakers; unified pods only affect pairings.  
Prize pools are per division, and proportional top‑cut distribution scales cleanly for Top 4 and Top 8.**
