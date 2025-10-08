
import random
n = 1000
rolls = [random.randint(1, 6) for _ in range(n)]
even_count = sum(1 for r in rolls if r % 2 == 0)
# experimental probability
experimental_prob = even_count / n
# theoretical probability
theoretical_prob = 0.5
print("Number of rolls:", n)
print("Even numbers rolled:", even_count)
print(f"Experimental Probability: {experimental_prob:.3f}")
print(f"Theoretical Probability:  {theoretical_prob:.3f}")
print(f"Difference: {abs(experimental_prob - theoretical_prob):.3f}")
