Family of Distributions in Input Data Modeling
This document summarizes key statistical distributions used in input data modeling, including their formulas and example problems.

Exponential Distribution
Used to model the time between events in a process where events happen continuously and independently.

Formula: f(x) = λe^(-λx), x ≥ 0

Example:

A service receives 3 calls/hour. Find P(next call > 15 min).
Convert 15 min = 0.25 hour
P(X > 0.25) = e^(-3×0.25) ≈ 0.4724


Normal Distribution
Used to model symmetric data centered around a mean (e.g., exam scores, heights).

Formula: f(x) = 1 / (σ√(2π)) * e^(-(x - μ)^2 / 2σ^2)

Example:

IQ with μ = 100, σ = 15. Find P(X < 115).
Z = (115 - 100)/15 = 1 → P(Z < 1) ≈ 0.8413


Poisson Distribution
Explanation: Used to count the number of events in a fixed time interval.

Formula: P(X = k) = (λ^k * e^(-λ)) / k!

Example:
λ = 5, k = 3 → P(3) = (125 * e^-5) / 6 ≈ 0.1404


Binomial Distribution
Models number of successes in fixed trials (like coin flips).

Formula: P(X = k) = C(n, k) * p^k * (1-p)^(n-k)

Example:

n = 6, k = 4, p = 0.5 → P = 15 * 0.0625 * 0.25 = 0.2344


Triangular Distribution
Used when only the minimum, maximum, and most likely values are known.

Formula: Piecewise: f(x) depends on whether x is ≤ or > the mode.

Example:

a = 2, b = 6, c = 4, x = 3 → f(3) = 2(3 - 2) / (4×2) = 0.25


Lognormal Distribution
Used when log(X) is normally distributed.

Formula: f(x) = 1 / (xσ√(2π)) * e^(-(ln x - μ)^2 / 2σ^2)


Example:
μ = 0, σ = 0.25, x = 1 → f(1) ≈ 1.596


Gamma Distribution
Models time until multiple events happen.

Formula: f(x) = β^α * x^(α-1) * e^(-βx) / Γ(α)

Example:

α = 2, β = 1, x = 3 → f(3) = 3 * e^-3 ≈ 0.1494


Beta Distribution
Used for modeling random variables between 0 and 1.

Formula:f(x) = x^(α - 1) * (1 - x)^(β - 1) / B(α, β)

Example:

α = 2, β = 3, x = 0.5 → f(0.5) = 0.125 / (1/12) = 1.5


Weibull Distribution
Used to model life data and failure rates.

Formula:f(x) = (k/λ) * (x/λ)^(k - 1) * e^(-(x/λ)^k)

Example:
k = 2, λ = 5, x = 4 → f(4) ≈ 0.1686


Uniform Distribution
All values between a and b are equally likely.

Formula: f(x) = 1 / (b - a)

Example:

a = 2, b = 6 → f(x) = 1 / 4 = 0.25


