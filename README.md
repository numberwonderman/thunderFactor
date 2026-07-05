# ⚡ THUNDER_FACTOR // V1.2.0 (The Daily Matrix)

A tactical, high-voltage math arcade game built with React. *Thunder Factor* combines a retro hacker aesthetic with a completely skill-based, shared daily competition. Every player worldwide receives the exact same matrix layout—your goal is to calculate the optimal mathematical path before your terminal resources run out.

---

## 🕹️ Game Mechanics & Rules

The terminal generates a **5x5 grid** filled with random two-digit integers, governed by a global, daily system **TARGET FACTOR** (e.g., 3, 4, 6, 7, 8, or 9).

### 1. Vector Linkage (Adjacent Movement)
* Chain together numbers that are completely divisible by the active target factor.
* Every number in your chain must be **physically adjacent** (horizontally, vertically, or diagonally) to the previous selection.
* Attempting to jump across the board triggers a `VECTOR DISCONNECTED` warning. Clicking a non-divisible number results in a `SYSTEM ERROR` and wipes out your current unexecuted path.

### 2. The 15-Move Core Limit
* **Energy is finite.** You are granted exactly **15 total moves (Slices)** per daily terminal session. 
* Once your 15 slices are executed, your matrix locks down, your terminal session ends, and your final score is locked in.

### 3. Synchronized Daily Seed (Deterministic RNG)
* No excuses, pure skill. The game utilizes a **Daily Seed Generator** tied directly to the current calendar date.
* Every single player worldwide gets the **exact same 5x5 starting grid** and the **exact same sequence of replacement numbers**. Your rank depends entirely on your strategy, pattern recognition, and mathematical efficiency.

---

## 📊 Scoring Matrix
Longer paths yield compounding, exponential rewards. Calculate your links carefully before executing a data slice to maximize your point yield per move:

$$\text{Score Reward} = \text{Chain Length} \times 100 \times \text{Chain Length}$$

| Chain Length | Points Awarded |
| :--- | :--- |
| **1 Tile** | 100 pts |
| **2 Tiles** | 400 pts |
| **3 Tiles** | 900 pts |
| **4 Tiles** | 1,600 pts |
| **5 Tiles** | 2,500 pts |

---

## 💻 Tech Stack
* **Frontend Core:** HTML5 / CSS3
* **UI Engine:** React 18 (Loaded via unpkg CDN)
* **Compiler:** Babel Standalone (In-browser JSX compilation)
* **Styling:** Inline JavaScript styles simulating a classic monochromatic green CRT terminal with responsive grid alignment and animated scanlines.

---

## 🚀 How to Play the Daily Challenge

1. Open the terminal link in your web browser.
2. Analyze the daily grid and the active target factor.
3. Trace your paths and click **EXECUTE SLICE [_ENTER]** to clear out the numbers.
4. Maximize your score within your **15 available slices**, then share your daily terminal breakdown with the community!
