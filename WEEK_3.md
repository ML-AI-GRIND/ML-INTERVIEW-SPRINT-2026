#  Week 3 Sprint: Estimation, Confidence Intervals & Hypothesis Testing

Welcome to Week 3 of the **ML/AI GRIND** weekly sprint! Week 1 gave us probability and Bayes' rule. Week 2 gave us random variables, distributions, and the CLT. This week we use all of it to answer the question every ML team asks: **"Is this result real, or is it just noise?"** We are covering **Sampling, Standard Error, Confidence Intervals, the Hypothesis Testing Framework, p-values, and Type I/II Errors**. Next week (Week 4) we build on this with power, sample size, multiple testing, and A/B testing.

---

###  Weekly Learning Objectives
1. Understand sampling distributions and standard error, and build and interpret confidence intervals correctly (what "95%" actually means, and what it does not mean).
2. Master the hypothesis testing framework: null vs. alternative, test statistics, p-values, and the significance level (α).
3. Understand Type I and Type II errors, and be able to explain the common p-value misreadings out loud in plain language.

---

###  Curated Resources for Week 3
* **[Devinterview Statistics Interview Questions](https://github.com/Devinterview-io/statistics-interview-questions)** — 75 statistics Q&As for ML and data science roles. Focus on the questions about hypothesis testing, p-values, Type I/II errors, α, and confidence intervals. (Heads up: its SciPy p-value example uses `binom_test`, which is deprecated. Use `scipy.stats.binomtest` instead.)
* **[StatQuest: Hypothesis Testing and The Null Hypothesis](https://www.youtube.com/watch?v=0oc49DyA3hU)** — Visual walkthrough of the null hypothesis and how a test decision is made.
* **[StatQuest: Confidence Intervals, Clearly Explained](https://www.youtube.com/watch?v=TqOeMYtOc1w)** — Builds intuition for what a confidence interval is and how to read it.
* **[There Is Only One Test (Allen Downey)](https://allendowney.blogspot.com/2011/05/there-is-only-one-test.html)** — Short read. Every test is "simulate the null, count how often you see something this extreme." This makes the whole topic click.
* **[Seeing Theory: Frequentist Inference](https://seeing-theory.brown.edu/frequentist-inference/index.html)** — Interactive simulations for confidence intervals and the bootstrap. (It does not cover hypothesis testing, so pair it with the resources above.)
* **[Scipy.stats Documentation Reference](https://docs.scipy.org/doc/scipy/reference/stats.html)** — `ttest_ind`, `ttest_1samp`, `binomtest`, and `bootstrap` for the practical task.

---

###  Practical Group Task
* Write a Python script using `numpy` and `scipy.stats` that tests our inference intuition by simulation. Build on last week's CLT script. Include both parts:
  1. **A/A test:** Draw two groups from the *same* Normal distribution 5,000 times and run a t-test each time. Verify that the false positive rate is about α = 0.05. Be ready to explain why it lands there.
  2. **Bootstrap vs. t-interval:** Take a skewed sample (for example, exponential, n = 60). Compare a bootstrap 95% CI for the mean with the classic t-based CI. Discuss when and why they differ.
* Focus on stating the null and alternative hypotheses clearly, checking your numbers against theory, and being able to explain *why* each result comes out the way it does.

---

###  Weekend Mock Interview Guide & Format
Over this coming Saturday and Sunday, we will conduct our peer mock interviews based on the rotation tracked in the [October Mock Interview Tracker](https://docs.google.com/spreadsheets/d/10fksoU7Ws7NrxaoaqcJ5gni_97uiE9UDyP50sxTdnZU/edit?usp=sharing).

#### How the Mock Interview Works (30–45 mins per session):
1. **The Question (10 mins):** The Interviewer presents a scenario involving confidence intervals, hypothesis tests, or p-values. Examples:
   * "Explain a p-value to a product manager. What does it *not* tell us?"
   * "What does a 95% confidence interval actually mean? Is there a 95% chance the true mean is inside this one?"
   * "Our new model lifts click-through from 10.0% to 10.4% on 5,000 users per arm. Is the lift real?"
   * "What is the difference between a Type I and a Type II error? Which one is worse for a fraud detection model?"
2. **The Walkthrough (15 mins):** The Interviewee restates the problem, defines the null and alternative hypotheses, picks a test and justifies its assumptions, computes or sets up the calculation, and explains what the result means in plain language.
3. **Feedback & Discussion (10 mins):** Constructive feedback on clarity, statistical rigor, and whether the interviewee avoided the classic p-value and confidence interval misinterpretations.

---

###  Goodluck Message
Inference is where probability meets real decisions, and it shows up in almost every DS and ML interview. Run the simulations, argue with your partners about what a p-value really means, and let's keep cooking! 🚀🔥

## feel free to add your own resource that could help the team
