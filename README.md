# A/B test simulator

An interactive page for comparing frequentist and Bayesian readouts of the same simulated A/B test.

**Live:** https://ziyi-zhu.github.io/ab-test-simulator/

Pick a metric (conversion, revenue, retention, ratio), set a baseline, true lift and sample size, then see:

- **Frequentist:** z-test, confidence interval, p-value, optional mSPRT sequential testing
- **Bayesian:** normal prior on relative lift, posterior, chance to beat, expected loss
- CUPED, winsorization, daily "peeking" reads, and a 2,000-run Monte Carlo of false-positive rate and power

The methods follow [Statsig's public docs](https://docs.statsig.com/). Data are simulated with normal approximations, so treat numbers as illustrative.

## Run locally

It's a single static file:

```sh
python3 -m http.server 8000
# open http://localhost:8000
```
