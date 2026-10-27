# Discrete Probability Distribution Calculator

An interactive web application for exploring discrete probability
distributions. It helps users calculate probabilities, understand
distribution parameters, and visualize probability patterns through
charts.

## Features

### 1. Binomial Distribution

-   Calculate the probability of getting exactly `k` successes in `n`
    independent trials.
-   Configure the number of trials and the probability of success.
-   View probability results across possible outcomes using a chart.

### 2. Poisson Distribution

-   Calculate the probability of observing exactly `k` events for a
    given average event rate (`λ`).
-   Enter the event count and the average rate.
-   Visualize the probability distribution across event counts.

### 3. Geometric Distribution

-   Calculate the probability that the first success occurs on trial
    `k`.
-   Set the probability of success for each independent trial.
-   View probabilities for possible trial numbers in a chart.

## Purpose

The project is designed as a learning tool for discrete probability
distributions. It combines probability calculations with visual
representations so students can explore how changing parameters affects
the results.

## Probability Formulas

### Binomial Distribution

For `X ~ Binomial(n, p)`:

\[ P(X = k) = `\binom{n}{k}`{=tex} p\^k (1-p)\^{n-k} \]

Where: - `n` is the number of independent trials. - `k` is the number of
successes. - `p` is the probability of success in each trial.

### Poisson Distribution

For `X ~ Poisson(λ)`:

\[ P(X = k) = `\frac{e^{-λ} λ^k}{k!}`{=tex} \]

Where: - `λ` is the average number of events in the interval. - `k` is
the number of events observed.

### Geometric Distribution

For `X ~ Geometric(p)`, where `X` counts the trial on which the first
success occurs:

\[ P(X = k) = (1-p)\^{k-1}p \]

Where: - `p` is the probability of success on each trial. - `k` is the
trial number of the first success, starting from 1.

## Getting Started

1.  Clone or download this repository.
2.  Open the project folder in your code editor.
3.  Install any dependencies required by the project, if applicable.
4.  Run the application using the development command configured in
    `package.json`, or open the HTML file directly if it is a standalone
    page.

> The exact run command depends on the tools and framework used in this
> project. Check `package.json` for the available scripts.

## How to Use

1.  Open the application.
2.  Select the distribution you want to explore.
3.  Enter the required parameters.
4.  Calculate the probability.
5.  Review the result and chart.
6.  Adjust the inputs to see how the distribution changes.

## Input Validation

Use valid parameter values: - Probabilities must be between `0` and
`1`. - The number of trials and event counts must be non-negative
integers where required. - For the geometric distribution, the trial
number `k` starts at `1`. - The Poisson rate `λ` must be non-negative.

## Technologies

Update this section to match the actual implementation: - HTML, CSS, and
JavaScript - Charting library (if used)

## Future Improvements

-   Add cumulative probability calculations.
-   Display expected value and variance for each distribution.
-   Add explanations and worked examples for common probability
    questions.
-   Improve accessibility and mobile responsiveness.
-   Add automated tests for probability calculations and input
    validation.

## Academic Use

This project is intended for educational and demonstration purposes.
Verify calculations and assumptions against your course materials when
using it for assignments.

## License

No license has been specified yet. Add a `LICENSE` file if you intend to
distribute the project publicly.
