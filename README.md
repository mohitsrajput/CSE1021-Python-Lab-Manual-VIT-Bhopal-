This repository contains all 34 assignment questions along with their corresponding Python code and detailed reports.

Q2) Digital Root Function

Rephrased Explanation

Task: Write a function digital_root(n) that repeatedly sums the digits of a number until a single-digit value is obtained.

What We Did: We implemented a Python function digital_root(n) that computes the digital root of a non-negative integer. Instead of using repeated digit-sum loops, the implementation takes advantage of a mathematical property that allows the result to be computed in constant time.

What We Learned: While the iterative method of summing digits is simple, the formula

(n - 1) % 9 + 1

How It Helps Others:

Checksum Validation: Digital roots can be used in basic error-detection systems.

Algorithm Optimization: The constant-time formula is faster than iterative digit processing, especially for large values or repeated operations.

Educational Value: The function clearly illustrates how number theory can simplify common programming tasks.

Q6) Deficient Number Checker

Rephrased Explanation

Task: Write a function is_deficient(n) that returns True if the sum of proper divisors of n is less than n.

What We Did: We created a function that computes all proper divisors of a positive integer and checks whether their sum is less than the number itself. The implementation uses an optimized divisor-finding technique by iterating only up to the square root of n.

What We Learned:

Understanding Deficient Numbers: A number is deficient if the sum of its proper divisors is smaller than the number.

Efficient Divisor Calculation: Looping up to √n greatly reduces computational cost.

Early Exit Optimization: The function stops early if the divisor sum already exceeds or equals n.

How It Helps Others:

Educational Insight: Demonstrates classification of numbers into deficient, perfect, or abundant.

Performance Optimization: Shows best practices for handling divisor-based computations.

Research Applications: Useful for exploring divisor properties and integer sequences.

Q12) Prime Power Checker

Rephrased Explanation

Task: Write a function is_prime_power(n) that determines whether a number can be written as , where is prime and .

What We Did: We implemented a function that factorizes the number using optimized trial division and checks whether exactly one distinct prime factor exists. If so, the number is a prime power.

What We Learned:

Prime Powers: A prime-power number contains only one unique prime factor.

Efficient Factorization: Limiting division to √n and early termination improves performance.

Fundamental Theorem of Arithmetic: The solution relies on the unique factorization property of integers.

How It Helps Others:

Cryptography: Prime powers appear in algorithms and cryptographic structures.

Algorithmic Thinking: Shows how theoretical math concepts guide efficient coding.

Code Optimization: Demonstrates techniques like early exit and reduced iteration ranges.

Q16) Aliquot Sum Function

Rephrased Explanation

Task: Write a function aliquot_sum(n) that returns the sum of all proper divisors of n.

What We Did: We developed a function that calculates the aliquot sum efficiently by finding divisor pairs using iteration only up to the square root. Special cases such as perfect squares and were properly handled.

What We Learned:

Aliquot Sum Definition: The sum of divisors excluding the number itself.

Performance Optimization: Using divisor pairs dramatically reduces computation time.

Edge Case Handling: Perfect squares and the value 1 require special treatment.

How It Helps Others:

Number Classification: Helps determine whether numbers are deficient, perfect, or abundant.

Sequence Generation: Useful in generating aliquot sequences for mathematical studies.

Algorithm Training: Demonstrates optimization techniques commonly used in divisor-related problems.

Q21) Modular Multiplicative Inverse

Rephrased Explanation

Task: Implement mod_inverse(a, m) to find x such that

(a \cdot x) \equiv 1 \pmod{m}.

What We Did: We wrote a function that uses the Extended Euclidean Algorithm to compute the modular inverse when a and m are coprime.

What We Learned:

Modular Inverse Concept: Exists only if gcd(a, m) = 1.

Extended Euclidean Algorithm: Computes coefficients satisfying Bézout’s identity and produces the modular inverse.

Algorithm Mechanics: Uses iterative reduction similar to the Euclidean GCD computation.

How It Helps Others:

Cryptography: Essential in RSA decryption key generation.

Error-Checking Systems: Used in standards like ISBN and IBAN.

Algorithm Efficiency: Converts division into multiplication in modular arithmetic for faster computation.

Q30) Carmichael Number Checker

Rephrased Explanation

Task: Write is_carmichael(n) to check whether a composite number satisfies

a^{n-1} \equiv 1 \pmod{n}

What We Did: We implemented the Carmichael number test using Korselt’s Criterion, supported by helper functions for primality testing and prime factor extraction.

What We Learned:

Korselt’s Criterion: A composite number is Carmichael if:

It is square-free.

For every prime divisor , divides .

Example: The smallest Carmichael number is 561 (3 × 11 × 17).

Efficiency: Korselt’s rule avoids checking all coprime bases, saving enormous computation.

How It Helps Others:

Primality Testing Education: Demonstrates limits of Fermat primality testing.

Efficient Algorithms: Shows how theoretical criteria outperform naive testing.

Cryptography Insight: Understanding Carmichael numbers is crucial for secure key generation.

Q31) Miller–Rabin Primality Test

Rephrased Explanation

Task: Implement the probabilistic Miller–Rabin primality test is_prime_miller_rabin(n, k).

What We Did: We implemented the Miller–Rabin algorithm using repeated randomized checks. Efficient modular exponentiation (pow()) was used to handle large integers.

What We Learned:

Probabilistic Primality: Deterministic tests are slow; Miller–Rabin is fast with extremely low error.

Algorithm Mechanics:

Decompose .

Test whether a randomly chosen base reveals compositeness.

Error Reduction: Each round reduces error probability to .

How It Helps Others:

Cryptography: Widely used for generating large primes in RSA and Diffie–Hellman.

Fast Prime Generation: Essential for handling numbers with hundreds or thousands of digits.

Computer Science Education: A strong example of practical randomized algorithms.
