#  ML & AI Engineering Master Interview Roadmap

This roadmap covers the essential technical domains required for senior-level Machine Learning, Data Science, and AI Engineering roles.

---

## A. Mathematics and Statistics
* **Core Focus:** Probability, conditional probability, Bayes’ rule, expectation, variance, and common distributions.
* **Inference & Testing:** Sampling, confidence intervals, hypothesis tests, p-values, Type I/II errors, statistical power, correlation vs. causation, confounding, selection bias, data leakage, and multiple testing.
* **Modeling Math:** Regression assumptions, residuals, regularization, multicollinearity, and PCA intuition.
* **Classification & Time-Series:** Classification thresholds, precision/recall trade-offs, handling imbalanced data, time-series leakage, chronological splits, seasonality, drift, and backtesting.
* **Problem-Solving Routine:** State assumptions $\rightarrow$ show steps $\rightarrow$ check units/edge cases $\rightarrow$ sanity-check results.

---

## B. Machine Learning and Evaluation Judgment
* **Validation Strategy:** Train/validation/test splits, cross-validation, leakage prevention, and duplicate contamination checks.
* **Metric Selection:** MAE/RMSE, precision/recall/F1, ROC-AUC vs. PR-AUC, calibration, and ranking metrics (NDCG/Hit Rate).
* **Model Diagnostics:** Bias/variance trade-offs, overfitting, regularization, feature engineering, missing data handling, and class imbalance mitigation.
* **Production Health:** Error analysis by subgroup and slice, robustness, fairness, drift tracking, and reproducibility.
* **LLM & Agent Evaluation:** Correctness, completeness, groundedness, instruction adherence, safety, tool-call validity, latency/cost trade-offs, and defining robust evaluation rubrics.

---

## C. Practical Python, SQL, and Data Work
* **Python Mastery:** Lists, dictionaries, sets, loops, functions, comprehensions, sorting, strings, exception handling, code complexity ($O(n)$ notation), and unit testing.
* **Data Processing Libraries:** NumPy and pandas vectorization, filtering, groupby aggregations, merges, handling missing values, and robust date/time handling.
* **SQL Proficiency:** Complex joins, advanced aggregations, `CASE` statements, CTEs, window functions (`ROW_NUMBER`, `RANK`), null behaviors, and deduplication routines.
* **Coding Routine:** Restate task $\rightarrow$ ask constraints $\rightarrow$ propose simple approach $\rightarrow$ implement $\rightarrow$ test edge/empty cases $\rightarrow$ discuss complexity.

---

## D. ML Engineering and Production Practicals
* **System Architecture:** Build working end-to-end systems covering data validation, reproducible preprocessing pipelines, model serialization (save/load), and prediction APIs via FastAPI.
* **Containerization & CI/CD:** Dockerizing microservices, writing automated tests, and setting up simple CI verification pipelines.
* **MLOps & Monitoring:** Logging, model serving trade-offs (batch vs. online), latency, throughput, cost optimization, data/model drift detection, automated rollbacks, and retraining triggers.
