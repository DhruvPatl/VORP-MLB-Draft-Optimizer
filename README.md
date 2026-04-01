# DiamondLogic: MLB Draft Optimizer
DiamondLogic is a Python-based valuation engine for fantasy baseball points leagues. It moves beyond basic "total points" projections by calculating VORP (Value Over Replacement Player) and Positional Tier Drops to identify the most mathematically optimal picks in real-time.

## 🔑 Key Features

- Positional Scarcity Mapping: Automatically accounts for the "cliff" at thin positions like SS and 2B.

- Live VORP Calculation: Re-evaluates player value against a dynamic 10-team replacement baseline.

- Tier Drop Alerts: Highlights the point-loss penalty if you pass on a top-tier player at a specific position.

- Fuzzy Search Console: Draft-day optimized input that handles partial names, typos, and accents (e.g., typing "diaz" correctly removes "Edwin Díaz").

- Ohtani Logic: Includes custom filtering to handle dual-eligibility data conflicts.



## The Math 📈 Why VORP?

In a points league, a player scoring 700 points isn't always better than a player scoring 600 points. $$VORP = \text{Player's Projected Points} - \text{Points of the 10th-ranked player at that POS}$$ If the "Replacement Level" Shortstop is weak, an elite Shortstop's VORP will skyrocket, making them a higher priority than an Outfielder with more total points but a deeper talent pool.
