# Continuous Probability Distributions: Industry Applications

A beginner-friendly, responsive educational web application for undergraduate AIML students. The project demonstrates how continuous probability distributions are used to reason about manufacturing quality, cloud request arrivals, and warehouse operations.

## Learning modules

### 1. Normal Distribution — Manufacturing Quality Control

- Illustrative shaft target diameter: 10 mm.
- Editable mean (μ), standard deviation (σ), lower specification limit (LSL), upper specification limit (USL), and selected diameter (x).
- Calculates the probability density at x, probability within specification limits, probability below LSL, probability above USL, expected defective percentage, and expected yield.
- Uses the normal probability density function and normal cumulative distribution function.
- Dynamically plots the bell curve, highlighting acceptable and defective regions.
- Validates positive standard deviation and LSL < USL; updates results as inputs change.

### 2. Exponential Distribution — Cloud Request Inter-arrival Time

- Illustrative arrival rate: λ = 12 requests per minute.
- Editable arrival rate (requests/minute) and two time thresholds (seconds).
- Converts the arrival rate to requests/second before calculating time-based quantities.
- Calculates mean inter-arrival time, variance, P(T ≤ t₁), P(T > t₁), and P(T > t₂ | T > t₁).
- Dynamically plots the exponential density curve and shades the probability regions.
- Explains the memoryless property in plain language and validates the rate, non-negative thresholds, and t₂ ≥ t₁.
- Clearly assumes a homogeneous, constant-rate Poisson arrival process. Inter-arrival time is the gap between incoming requests; it is not server response time.

### 3. Central Limit Theorem — Warehouse Processing Time

- Illustrative population mean: μ = 18 minutes; population standard deviation: σ = 6 minutes.
- Editable population mean (μ), population standard deviation (σ), sample size (n), and sample-mean threshold (x̄).
- Calculates the expected sample mean E(X̄) = μ, variance Var(X̄) = σ²/n, standard error σ/√n, z-score, P(X̄ ≤ x̄), P(X̄ > x̄), and the approximate central 95% range.
- Dynamically plots the sampling distribution of sample means with the left and right probability areas shaded. A dashed population curve is included to compare individual processing-time variation with the narrower distribution of sample averages.
- Explains how increasing sample size reduces standard error while the expected sample mean remains at μ.
- Validates finite numeric inputs, σ > 0, and a positive integer sample size (1–100,000).
- Uses a normal approximation to the sampling distribution. It is exact for every sample size if the population is normal; for other populations, the approximation generally improves as sample size increases, assuming independent random sampling and finite variance.

## Run locally

No dependencies, package installation, build step, or server are required.

1. Download and extract the project ZIP.
2. Open `index.html` in a modern web browser.
3. Select a module from the top navigation or the home-page cards.
4. Edit the inputs to explore the calculations and graphs. Use each module's reset button to restore its illustrative example.

## Technology

- HTML5 and CSS3
- Vanilla JavaScript
- Inline SVG charts
- No external libraries or runtime dependencies

The Normal and CLT modules use a JavaScript error-function approximation for the standard normal CDF. The Exponential module uses JavaScript's exponential functions and explicitly converts requests/minute to requests/second.

## Important modelling notes

These modules are educational probability models. Their outputs depend on the stated distributional assumptions and should not be treated as guarantees about a real production batch, live cloud traffic, or a specific warehouse operation. Check whether the assumptions are reasonable before applying the models to operational decisions.
