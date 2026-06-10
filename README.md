# myFirstRepo

A collection of statistical exercises and code from my summer bootcamp, where I'm learning R and GitHub.

---

## Sampling Distribution of the Mean

**File:** `sampling_distribution.Rmd` / `sampling_distribution.nb.html`

This R notebook is an interactive simulation exploring one of the most important ideas in statistics: the **sampling distribution of the mean** and the **Central Limit Theorem (CLT)**.

### What it does

1. **Builds a skewed population** — generates 100,000 values from an exponential distribution, which is heavily right-skewed and looks nothing like a normal curve.

2. **Simulates sampling** — draws 1,000 random samples from that population at three different sample sizes:
   - Small: n = 5
   - Medium: n = 30
   - Large: n = 100

3. **Plots the sampling distributions** — visualises how the distribution of sample means changes shape and spread as sample size grows.

4. **Demonstrates the CLT** — even though the population is skewed, the sample means become approximately normally distributed as n increases.

5. **Verifies the standard error formula** — compares the observed spread of sample means against the theoretical prediction σ/√n.

### Key takeaways

- The sample mean is an **unbiased estimator** — it centres on the true population mean regardless of sample size.
- **Larger samples produce narrower distributions** — you get more precise estimates with more data.
- The **standard error shrinks as √n**, meaning there are diminishing returns to increasing sample size.

### How to run

Open `sampling_distribution.Rmd` in RStudio and click **Knit**, or run in R:

```r
rmarkdown::render("sampling_distribution.Rmd")
```

**Required packages:** `ggplot2`, `dplyr`, `tidyr`, `rmarkdown`

---

## Other files

- `analysis.R` — arithmetic exercises from early in the bootcamp
