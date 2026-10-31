# Dice Game Risk Analysis

How does session length affect the probability of losing money in
a game with positive expected profit?

This project studies a two-dice game: pay $4, roll two fair six-sided
dice, and receive the higher number in dollars.

## Methods

- Derive the expected profit mathematically.
- Estimate loss probabilities using Monte Carlo simulation.
- Calculate exact loss probabilities using dynamic programming.
- Compare a continuity-corrected normal approximation with exact results.
- Measure simulation uncertainty using standard errors.

## Main findings

Expected profit is approximately $0.47 per game, but losses remain
possible. For the session lengths tested, exact loss probability
fell from 25% for one game to approximately 0.0473% for 100 games.

The normal approximation underestimated the 100-game loss probability
by 28.42% relative to the exact result. Simulation also becomes less
precise relative to the probability when losses are rare.

## Run the notebook

Requires Python 3, Jupyter, and Matplotlib.

Install the dependencies:

```sh
python -m pip install notebook matplotlib