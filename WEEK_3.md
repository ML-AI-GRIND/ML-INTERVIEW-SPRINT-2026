#  Week 3 Sprint: Statistical Inference & Hypothesis Testing

Welcome to Week 3 of the **ML/AI GRIND** weekly sprint! Week 1 gave us probability and Bayes' rule. Week 2 gave us random variables, distributions, and the CLT. This week we use all of it to answer the question every ML team asks: **"Is this result real, or is it just noise?"** We are covering **Sampling, Confidence Intervals, Hypothesis Tests, p-values, Type I/II Errors, Power, and Multiple Testing**.

---

###  Weekly Learning Objectives
1. Understand sampling distributions and standard error, and build and interpret confidence intervals correctly (what "95%" actually means, and what it does not mean).
2. Master the hypothesis testing framework: null vs. alternative, test statistics, p-values, significance level (α), Type I/II errors, and statistical power. Know the common p-value misreadings and be able to explain them out loud.
3. Handle real-world pitfalls: multiple testing (Bonferroni, Benjamini-Hochberg), sample size planning, peeking in A/B tests, and statistical vs. practical significance.

---

###  Curated Resources for Week 3
* **[Devinterview Statistics Interview Questions](https://github.com/Devinterview-io/statistics-interview-questions)** — 75 statistics Q&As for ML and data science roles. Focus on the questions about hypothesis testing, p-values, Type I/II errors, power, α, and confidence intervals. (Heads up: its SciPy p-value example uses `binom_test`, which is deprecated. Use `scipy.stats.binomtest` instead.)
* **[StatQuest: Hypothesis Testing and The Null Hypothesis](https://www.youtube.com/watch?v=0oc49DyA3hU)** — Visual walkthrough of the null hypothesis and how a test decision is made.
* **[StatQuest: Confidence Intervals, Clearly Explained](https://www.youtube.com/watch?v=TqOeMYtOc1w)** — Builds intuition for what a confidence interval is and how to read it.
* **[StatQuest: Statistical Power, Clearly Explained](https://www.youtube.com/watch?v=Rsc5znwR5FA)** — Why underpowered tests miss real effects and what drives power.
* **[StatQuest: Bootstrapping Main Ideas](https://www.youtube.com/watch?v=Xz0x-8-cgaQ)** — Resampling to estimate uncertainty when a closed-form formula is not available.
* **[StatQuest: False Discovery Rates (FDR)](https://www.youtube.com/watch?v=K8LQSvtjcEo)** — The multiple testing problem and why we correct for it.
* **[Think Stats 2e (Allen Downey, free online)](https://greenteapress.com/thinkstats2/html/index.html)** — Read the **Estimation** and **Hypothesis testing** chapters. Python-first, simulation-based, and very interview friendly.
* **[There Is Only One Test (Allen Downey)](https://allendowney.blogspot.com/2011/05/there-is-only-one-test.html)** — Short read. Every test is "simulate the null, count how often you see something this extreme." This makes the whole topic click.
* **[Seeing Theory: Frequentist Inference](https://seeing-theory.brown.edu/frequentist-inference/index.html)** — Interactive simulations for confidence intervals and the bootstrap. (It does not cover hypothesis testing, so pair it with the resources above.)
* **[Evan Miller's A/B Test Sample Size Calculator](https://www.evanmiller.org/ab-testing/sample-size.html)** — Play with baseline rate, minimum detectable effect, α, and power to see how sample size changes.
* **[Scipy.stats Documentation Reference](https://docs.scipy.org/doc/scipy/reference/stats.html)** — `ttest_ind`, `ttest_1samp`, `chi2_contingency`, `bootstrap`, and `false_discovery_control` (Benjamini-Hochberg).
* **[Statsmodels Stats Reference](https://www.statsmodels.org/stable/stats.html)** — `TTestIndPower` / `NormalIndPower` for power and sample size, and `multipletests` for Bonferroni and FDR corrections.

---

###  Practical Group Task
* Write a Python script using `numpy` and `scipy.stats` (add `statsmodels` for the power part) that tests our hypothesis testing intuition by simulation. Build on last week's CLT script. Include all four parts:
  1. **A/A test:** Draw two groups from the *same* Normal distribution 5,000 times and run a t-test each time. Verify that the false positive rate is about α = 0.05.
  2. **Power:** Now give one group a true effect (Cohen's d = 0.5, n = 100 per group). Estimate power by simulation and compare it with the analytic answer from `TTestIndPower`.
  3. **Multiple testing:** Run 20 tests where every null is true. Show the chance of at least one false positive (about 64% theoretically, since 1 − 0.95²⁰). Then apply Bonferroni and Benjamini-Hochberg and show the rate drops back near 5%.
  4. **Bootstrap vs. t-interval:** Take a skewed sample (for example, exponential, n = 60). Compare a bootstrap 95% CI for the mean with the classic t-based CI.
* Focus on stating hypotheses and assumptions clearly, checking the numbers against theory, and being able to explain *why* each result comes out the way it does.

---

###  Weekend Mock Interview Guide & Format
Over this coming Saturday and Sunday, we will conduct our peer mock interviews based on the rotation tracked in the [October Mock Interview Tracker](https://docs.google.com/spreadsheets/d/10fksoU7Ws7NrxaoaqcJ5gni_97uiE9UDyP50sxTdnZU/edit?usp=sharing).

#### How the Mock Interview Works (30–45 mins per session):
1. **The Question (10 mins):** The Interviewer presents a scenario involving confidence intervals, hypothesis tests, p-values, power, or A/B testing. Examples:
   * "Explain a p-value to a product manager. What does it *not* tell us?"
   * "Our new model lifts click-through from 10.0% to 10.4% on 5,000 users per arm. Do we ship it?"
   * "You test 20 features for correlation with churn and one is significant at p = 0.03. Do you trust it?"
   * "How many users do we need for this experiment, and what happens if we stop early when we see a significant result?"
2. **The Walkthrough (15 mins):** The Interviewee restates the problem, defines the null and alternative hypotheses, picks a test and justifies its assumptions, computes or sets up the calculation, and discusses Type I/II errors, power, and practical significance.
3. **Feedback & Discussion (10 mins):** Constructive feedback on clarity, statistical rigor, and whether the interviewee gave a clear business decision at the end.

---

###  Goodluck Message
Two weeks of foundations are about to pay off. Inference is where probability meets real decisions, and it is one of the most common topics in DS and ML interviews. Run the simulations, argue with your partners about what a p-value really means, and let's keep cooking! 🚀🔥

## feel free to add your own resource that could help the team
