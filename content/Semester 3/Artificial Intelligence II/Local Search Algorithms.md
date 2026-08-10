- Local Search (AKA Iterative Improvement) Algorithms are optimization techniques that improve a solution by repeatedly moving to a better neighbouring state

# Hill Climbing

1. Choose an initial state
	- Usually random (but not necessarily)
2. Find neighbouring states
3. Compare neighbouring states
	- If a better neigbouring state exists, replace current state with it
4. Repeat until no better neighbours exist or until a certain number of iterations

---

- Depending on initial state the algorithm can get stuck on a local optima
- The following algorithms are variants of hill climbing that prevent this

## Random Restart Hill Climbing

- Works by jumping to a random new position after a fixed number of iterations
	- This is what prevents the algorithm getting stuck on a local optima
- Keep the current best state as you go

## Simulated Annealing

- Start with a temperature set very high
	- Gradually decrease the temperature with each iteration
- When comparing neighbouring states, there is a chance that the current state is replaced by a worse state
	- This probablity is based on the current temperature and how much worse the new state is