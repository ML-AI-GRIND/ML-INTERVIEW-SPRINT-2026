#  Week 4 Sprint: Power, Multiple Testing & A/B Testing

Welcome to Week 4 of the **ML/AI GRIND** weekly sprint! Last week we learned how to build confidence intervals and run hypothesis tests. This week we go one level deeper into what makes those tests trustworthy in practice: **Statistical Power, Sample Size, Multiple Testing, and the A/B Testing Pitfalls** that trip up even experienced engineers.

---

###  Weekly Learning Objectives
1. Understand statistical power, effect size, and how α, power, effect size, and sample size trade off against each other. Be able to plan a sample size before an experiment.
2. Understand the multiple testing problem and how to correct for it (Bonferroni for family-wise error, Benjamini-Hochberg for false discovery rate).
3. Spot the common experiment pitfalls: peeking and early stopping, statistical vs. practical significance, and results that are really driven by confounding, selection bias, or data leakage rather than a true effect.

---

###  Curated Resources for Week 4
* **[Devinterview Statistics Interview Questions](https://github.com/Devinterview-io/statistics-interview-questions)** — Revisit the questions on statistical power, α, and confidence intervals (which also touches multiple comparisons), and work through the rest of the list.
* **[StatQuest: Statistical Power, Clearly Explained](https://www.youtube.com/watch?v=Rsc5znwR5FA)** — Why underpowered tests miss real effects and what drives power.
* **[StatQuest: False Discovery Rates (FDR)](https://www.youtube.com/watch?v=K8LQSvtjcEo)** — The multiple testing problem and why we correct for it.
* **[Evan Miller's A/B Test Sample Size Calculator](https://www.evanmiller.org/ab-testing/sample-size.html)** — Play with baseline rate, minimum detectable effect, α, and power to see how the required sample size changes.
* **[Think Stats 2e (Allen Downey, free online)](https://greenteapress.com/thinkstats2/html/index.html)** — Read the **Hypothesis testing** chapter again with power in mind. Python-first and simulation-based.
* **[Statsmodels Stats Reference](https://www.statsmodels.org/stable/stats.html)** — `TTestIndPower` / `NormalIndPower` for power and sample size, and `multipletests` for Bonferroni and FDR corrections.
* **[Scipy: false_discovery_control](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.false_discovery_control.html)** — Benjamini-Hochberg and Benjamini-Yekutieli adjustment of p-values.

---

###  Practical Group Task
* Write a Python script using `numpy`, `scipy.stats`, and `statsmodels` that explores power and multiple testing by simulation. Include both parts:
  1. **Power:** Give one group a true effect (Cohen's d = 0.5, n = 100 per group). Estimate power by simulation and compare it with the analytic answer from `TTestIndPower`. Then solve for the sample size per group needed to reach 80% power.
  2. **Multiple testing:** Run 20 tests where every null is true. Show the chance of at least one false positive (about 64% theoretically, since 1 − 0.95²⁰). Then apply Bonferroni and Benjamini-Hochberg and show the rate drops back near 5%.
* Focus on checking simulation results against theory, and being able to explain *why* correction methods trade power for fewer false positives.

---

###  Weekend Mock Interview Guide & Format
Over this coming Saturday and Sunday, we will conduct our peer mock interviews based on the rotation tracked in the [October Mock Interview Tracker](https://docs.google.com/spreadsheets/d/10fksoU7Ws7NrxaoaqcJ5gni_97uiE9UDyP50sxTdnZU/edit?usp=sharing).

#### How the Mock Interview Works (30–45 mins per session):
1. **The Question (10 mins):** The Interviewer presents a scenario involving power, sample size, multiple comparisons, or experiment design. Examples:
   * "How many users do we need per arm to detect a lift from 10.0% to 10.4% in click-through? What do you need to ask me first?"
   * "A teammate checks the A/B test every day and stops the moment p < 0.05. What is wrong with that?"
   * "You test 20 features for correlation with churn and one is significant at p = 0.03. Do you trust it?"
   * "Users who got the new feature spend more. Does the feature cause that? What could confound it?"
2. **The Walkthrough (15 mins):** The Interviewee restates the problem, states assumptions, sets up the calculation or the experiment design, and discusses power, corrections, and practical significance. Bonus points for naming confounding, selection bias, or leakage when the scenario hints at it.
3. **Feedback & Discussion (10 mins):** Constructive feedback on clarity, statistical rigor, and whether the interviewee gave a clear recommendation at the end.

---

###  Goodluck Message
Two weeks of inference done after this one. Power and multiple testing are where strong candidates separate themselves, because they show you understand how experiments fail in the real world. Run the simulations, challenge each other's designs, and let's keep cooking! 🚀🔥

## feel free to add your own resource that could help the team
