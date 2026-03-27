Language: Python 3
Environment: Jupyter Notebook (IPython)

⚙️ Dependencies
pip install matplotlib numpy

Other libraries used (math, random, collections, datetime) are part of Python’s standard library.

🧩 Q10 — Hill Climbing

Maximizing the function:

f(x) = -(x - 3)^2 + 9

(Global maximum at x = 3, f(x) = 9)

Implementations

Simple Hill Climbing

Moves to the first improving neighbor

Steepest-Ascent Hill Climbing 

Evaluates both neighbors and chooses the best

Random-Restart Hill Climbing

Runs hill climbing multiple times from random starting points

Key Insight

Random restart is not always useful. For unimodal functions, it adds unnecessary computation.

🧳 Q11 — Simulated Annealing (TSP)

Solved a 10-city Travelling Salesman Problem using Simulated Annealing.

Setup

Cities represented as coordinates

State: permutation of cities

Neighbor: swap two cities

Acceptance probability: P = e^(-ΔE / T)

Parameters

Initial Temperature: 1000

Cooling Rate: 0.995

Iterations: 10,000

Cooling Schedules

Geometric Cooling → better exploration & results

Linear Cooling → faster but may converge early

Key Insight

Geometric cooling generally produces better solutions than linear cooling.

♛ Q12 — 8-Queens (Beam Search)

Placed 8 queens on an 8×8 board such that none attack each other.

Representation

State: list of queen row positions

Heuristic: number of non-attacking pairs

Goal: 28

Algorithms

Local Beam Search (LBS)

Keeps top k = 5 states but may lose diversity

Stochastic Beam Search (SBS)

Uses probability to maintain diversity and avoid local traps

Key Insights

LBS suffers from plateau problem

SBS performs better due to diversity

SBS may take slightly more iterations

📂 File Structure

23F-0855_6C_A3.ipynb → Main notebook

▶️ How to Run

Install dependencies

pip install matplotlib numpy

Open notebook

jupyter notebook 23F-0855_6C_A3.ipynb

Run all cells (Restart & Run All)
