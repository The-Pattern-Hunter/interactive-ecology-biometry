# 📊 Unit 4: Biometry - Statistical Methods for Ecology

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/The-Pattern-Hunter/interactive-ecology-biometry/blob/main/unit-4-biometry/)

---

## 📖 Overview

Biometry applies statistical methods to biological questions. This unit covers probability distributions, descriptive statistics, sampling, hypothesis testing, experimental design, regression, and ANOVA through nine interactive notebooks. **The Pattern Hunter philosophy shines here**: students explore distributions visually before formulas, building statistical intuition through ecological examples.

**Core Innovation**: The **Stethoscope Analogy** - statistical distributions as diagnostic instruments, each detecting specific patterns in ecological data.

---

## 🎯 Learning Outcomes

By completing this unit, you will:

1. **Recognize and apply** 8 probability distributions to ecological data
2. **Calculate and interpret** measures of central tendency and dispersion
3. **Design sampling strategies** (random, stratified, systematic, cluster)
4. **Conduct hypothesis tests** (chi-square, t-tests, ANOVA)
5. **Design rigorous experiments** with proper controls and randomization
6. **Perform regression analysis** (linear, multiple, polynomial)
7. **Apply ANOVA** for comparing multiple groups
8. **Think statistically** using the Pattern Hunter approach

---

## 📚 Notebooks

### 1. Distributions Exploration 🔍

**The Foundation**: Interactive exploration of 8 probability distributions

**Distributions Covered**:
- **Binomial**: Success/failure trials (seed germination, survival)
- **Poisson**: Rare, independent events (species per quadrat)
- **Normal**: Continuous, symmetric (height, weight, measurement error)
- **Uniform**: Equal probability (random number generation)
- **Exponential**: Time between events, constant rate (radioactive decay, survival time)
- **Geometric**: Trials until first success (captures until recapture)
- **Negative Binomial**: Trials until r successes (overdispersed counts)
- **Log-Normal**: Skewed, positive (body mass, population size)

**The Stethoscope Analogy** 🩺:
```
Doctor's Tool          Ecologist's Tool
------------           ----------------
Stethoscope     ↔      Normal distribution (detect random variation)
Thermometer     ↔      Poisson distribution (detect rare events)
Blood pressure  ↔      Binomial distribution (detect success/failure)
X-ray           ↔      Exponential distribution (detect constant-rate processes)
```

**Interactive Features**:
- Parameter sliders (μ, σ, λ, p, etc.)
- Real-time shape changes
- Ecological examples for each
- Pattern recognition exercises

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/The-Pattern-Hunter/interactive-ecology-biometry/blob/main/unit-4-biometry/notebooks/01_distributions_exploration.ipynb)

**Pattern Hunter**: See distributions as SHAPES first (bell curve, J-curve, exponential decay), understand when to use each TOOL, then learn formulas.

**Learning Time**: ~2 hours

---

### 2. Central Tendency Analysis 📍

**Topics**: Mean, median, mode, geometric mean, trimmed mean, skewness, outliers

**Key Concepts**:
- **Mean (x̄)**: Average, sensitive to outliers
- **Median**: Middle value, robust to outliers
- **Mode**: Most frequent, useful for categorical
- **When to use which**: Depends on distribution shape
- **Skewness**: Right (positive), left (negative), symmetric

**Pattern Recognition**: 
- Symmetric → Mean ≈ Median ≈ Mode
- Right-skewed → Mean > Median > Mode
- Left-skewed → Mode > Median > Mean

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/The-Pattern-Hunter/interactive-ecology-biometry/blob/main/unit-4-biometry/notebooks/02_central_tendency_analysis.ipynb)

**Real Examples**: Tree heights, animal weights, species counts

**Learning Time**: ~1.5 hours

---

### 3. Dispersion Measures 📏

**Topics**: Range, variance, standard deviation, coefficient of variation, interquartile range

**Key Concepts**:
- **Range**: Max - Min (simple but sensitive to outliers)
- **Variance (s²)**: Average squared deviation from mean
- **Standard Deviation (SD)**: √variance (same units as data)
- **Coefficient of Variation (CV)**: SD/Mean × 100% (unitless comparison)
- **IQR**: Q₃ - Q₁ (robust to outliers)

**Pattern Recognition**:
- High dispersion = Spread out, high variability
- Low dispersion = Clustered, consistent
- CV allows comparing variability across different scales

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/The-Pattern-Hunter/interactive-ecology-biometry/blob/main/unit-4-biometry/notebooks/03_dispersion_measures.ipynb)

**Applications**: Population variability, measurement precision, comparing datasets

**Learning Time**: ~1.5 hours

---

### 4. Sampling Techniques 🎯

**Topics**: Random, stratified, systematic, cluster sampling, sample size determination

**Sampling Methods**:
- **Simple Random**: Every unit equal probability
- **Stratified**: Divide into groups, sample each proportionally
- **Systematic**: Every nth unit (transects)
- **Cluster**: Sample groups, then all within selected groups

**Key Concepts**:
- Sampling error vs bias
- Representative samples
- Sample size affects precision
- Trade-offs: accuracy vs cost

**Interactive Simulations**: Compare methods on simulated populations, see bias and variance

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/The-Pattern-Hunter/interactive-ecology-biometry/blob/main/unit-4-biometry/notebooks/04_sampling_techniques.ipynb)

**Real Applications**: Quadrat sampling, mark-recapture, transect surveys

**Learning Time**: ~1.5 hours

---

### 5. Hypothesis Testing 🧪

**Topics**: Chi-square, one-sample t-test, two-sample t-test, paired t-test, p-values

**Hypothesis Testing Framework**:
1. State H₀ (null) and H₁ (alternative)
2. Choose significance level (α = 0.05)
3. Calculate test statistic
4. Find p-value
5. Decision: Reject H₀ if p < α

**Tests Covered**:
- **Chi-square**: Categorical data (goodness-of-fit, independence)
- **One-sample t**: Does mean differ from hypothesized value?
- **Two-sample t**: Do two groups differ?
- **Paired t**: Do paired measurements differ?

**Pattern Recognition**: Test statistic distributions (chi-square, t) are our "stethoscopes" - each detects specific deviation from null hypothesis.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/The-Pattern-Hunter/interactive-ecology-biometry/blob/main/unit-4-biometry/notebooks/05_hypothesis_testing.ipynb)

**Real Examples**: Habitat preference (chi-square), fertilizer effects (t-test)

**Learning Time**: ~2 hours

---

### 6. Hypothesis Testing Fundamentals 🎓

**Topics**: Type I/II errors, power, confidence intervals, effect size, one-tailed vs two-tailed

**Critical Concepts**:
- **Type I error (α)**: False positive, reject true H₀
- **Type II error (β)**: False negative, fail to reject false H₀
- **Power (1-β)**: Probability of detecting real effect
- **Confidence Interval**: Range likely to contain true parameter
- **Effect size**: Magnitude of difference (practical significance)

**Decision Matrix**:
```
                H₀ True         H₀ False
Reject H₀       Type I Error    Correct (Power)
Fail to Reject  Correct (1-α)   Type II Error
```

**Interactive**: Adjust sample size, effect size, α - see power change

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/The-Pattern-Hunter/interactive-ecology-biometry/blob/main/unit-4-biometry/notebooks/06_hypothesis_testing_fundamentals.ipynb)

**Learning Time**: ~1.5 hours

---

### 7. Experimental Design 🔬

**Topics**: ANOVA basics, controls, randomization, replication, blocking, factorial designs

**Design Principles**:
- **Randomization**: Eliminates bias
- **Replication**: Estimates variability, increases power
- **Controls**: Baseline for comparison
- **Blocking**: Accounts for known variability

**Design Types**:
- **Completely Randomized Design (CRD)**: Random assignment to treatments
- **Randomized Complete Block Design (RCBD)**: Blocks account for spatial/temporal variation
- **Factorial Design**: Multiple factors, test interactions

**Pattern Recognition**: Good design = Less noise, clearer signal

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/The-Pattern-Hunter/interactive-ecology-biometry/blob/main/unit-4-biometry/notebooks/07_experimental_design.ipynb)

**Real Applications**: Field experiments, greenhouse trials, plot-based studies

**Learning Time**: ~1.5 hours

---

### 8. Regression Analysis 📈

**Topics**: Simple linear, multiple, polynomial regression, R², residuals, assumptions

**Regression Framework**:
- **Simple Linear**: y = β₀ + β₁x + ε (one predictor)
- **Multiple**: y = β₀ + β₁x₁ + β₂x₂ + ... + ε (multiple predictors)
- **Polynomial**: y = β₀ + β₁x + β₂x² + ... + ε (curved relationships)

**Key Concepts**:
- **R²**: Proportion of variance explained (0-1)
- **Slope (β₁)**: Change in y per unit x
- **Residuals**: Observed - Predicted (should be random)
- **Assumptions**: Linearity, independence, homoscedasticity, normality

**Diagnostics**:
- Residual plots (detect patterns)
- Q-Q plots (check normality)
- Leverage/influence (outliers)

**Interactive**: Fit models to real ecological data, examine diagnostics

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/The-Pattern-Hunter/interactive-ecology-biometry/blob/main/unit-4-biometry/notebooks/08_regression_analysis.ipynb)

**Real Examples**: Height-diameter relationships, species-area curves, temperature-metabolism

**Learning Time**: ~2 hours

---

### 9. ANOVA (Analysis of Variance) 📊

**Topics**: One-way ANOVA, two-way ANOVA, post-hoc tests (Tukey HSD), assumptions

**ANOVA Framework**:
- **Question**: Do means differ among 3+ groups?
- **Null (H₀)**: All group means equal
- **Alternative (H₁)**: At least one differs
- **F-statistic**: Variance between groups / Variance within groups

**ANOVA Types**:
- **One-way**: One factor (e.g., 4 fertilizer treatments)
- **Two-way**: Two factors (e.g., fertilizer × watering)
  - Main effects (fertilizer effect, watering effect)
  - Interaction (does fertilizer effect depend on watering?)

**Post-hoc Tests**:
- ANOVA says "differences exist" but not WHERE
- Tukey HSD: Pairwise comparisons (controls family-wise error rate)

**Assumptions**:
- Independence
- Normality (within groups)
- Homogeneity of variance (equal variances)

**Pattern Recognition**: Large F = Groups differ more than expected by chance

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/The-Pattern-Hunter/interactive-ecology-biometry/blob/main/unit-4-biometry/notebooks/09_anova.ipynb)

**Real Examples**: Fertilizer trials, habitat comparisons, treatment effects

**Learning Time**: ~2 hours

---

## 🎨 The Pattern Hunter Philosophy in Unit 4

### The Stethoscope Analogy 🩺

**Traditional Statistics**: "Here's the formula for normal distribution: f(x) = (1/√(2πσ²))e^(-(x-μ)²/(2σ²))"  
→ Students memorize, forget, fear statistics

**Pattern Hunter**: "The normal distribution is your 'stethoscope' for detecting random variation around a mean. Adjust μ and σ with sliders, SEE the bell curve shift and spread. NOW the formula makes sense - it describes what you already understand visually."

### Pattern-First Learning Journey:

**Traditional Path**:
```
Formula → Definition → Example → Confusion → Memorize → Forget
```

**Pattern Hunter Path**:
```
Interactive Visualization → Pattern Recognition → Ecological Context → 
Intuition Built → Formula (as description) → Deep Understanding → Retention
```

### Concrete Examples:

1. **Distributions**: See shapes (bell, J, exponential) BEFORE probabilities
2. **Central Tendency**: Observe mean/median positions on histograms BEFORE calculations
3. **Hypothesis Tests**: Visualize test statistic distributions BEFORE p-values
4. **Regression**: Plot scatterplots, see trend lines BEFORE least squares
5. **ANOVA**: Box plots show group differences BEFORE F-statistics

**Result**: Statistics becomes pattern recognition, not formula manipulation.

---

## 🔗 Connections

**From Units 1-3**: 
- Energy pyramids → Data visualization
- Exponential decay → Exponential distribution
- Population growth → Regression models
- Species-area → Log-log regression

**Applications**: Every ecological question requires statistics. This unit provides the toolkit.

---

## 📊 Interactive Features

✅ **Parameter sliders** for all distributions  
✅ **Real-time visualizations** (curves update instantly)  
✅ **Ecological examples** throughout  
✅ **Hypothesis test simulators** (interactive p-values)  
✅ **Regression diagnostics** (residual plots, Q-Q plots)  
✅ **ANOVA calculators** with post-hoc tests  
✅ **Pattern recognition exercises** ("Which distribution fits?")  
✅ **Comprehensive code comments** (learn by reading)

---

## 🎓 Skills Developed

### Statistical Thinking:
- Recognizing distributional patterns
- Selecting appropriate tests
- Interpreting p-values correctly
- Understanding Type I/II errors

### Analytical:
- Hypothesis formulation
- Experimental design
- Model fitting and diagnostics
- Effect size vs statistical significance

### Computational:
- Python for statistics (SciPy, statsmodels)
- Creating professional visualizations
- Running simulations
- Reproducible analysis

### Communication:
- Presenting statistical results
- Visual communication (plots)
- Interpreting for non-statisticians

---

## 📖 Recommended Reading

### Statistics Foundations:
- Zar, J. H. (2010). *Biostatistical Analysis*. 5th edition.
- Sokal, R. R., & Rohlf, F. J. (2012). *Biometry*. 4th edition.
- Quinn, G. P., & Keough, M. J. (2002). *Experimental Design and Data Analysis for Biologists*.

### Pattern Hunter Philosophy:
- Patel, A. & Kar, S. (2024). Interactive Ecology and Biometry. DOI: 10.5281/zenodo.14463277

### Accessible Introductions:
- Whitlock, M. C., & Schluter, D. (2020). *The Analysis of Biological Data*. 3rd edition.

---

## 💡 Teaching & Learning Tips

### For Instructors:
1. **Always start with visualization**: Show distribution shapes, let students explore
2. **Use ecological examples**: "Does fertilizer work?" not "Is μ₁ ≠ μ₂?"
3. **Emphasize interpretation**: p-value means what? Effect size matters!
4. **Encourage exploration**: Sliders build intuition faster than lectures
5. **Connect to research**: How do real ecologists use these tools?

### For Students:
1. **Play with sliders FIRST**: See patterns before formulas
2. **Ask "Which stethoscope?"**: Match distribution to data type
3. **Visualize data always**: Plot before testing
4. **Check assumptions**: Tests fail if assumptions violated
5. **Interpret, don't just calculate**: What does result MEAN biologically?

---

## 🌍 Real-World Applications

- **Ecology**: Population comparisons, diversity analysis, growth models
- **Conservation**: Monitoring programs, impact assessments, A/B testing
- **Agriculture**: Fertilizer trials, cultivar comparisons, yield optimization
- **Medicine**: Clinical trials, epidemiology, dose-response
- **Environmental Science**: Pollution assessment, climate analysis

---

## 🛠️ Technical Requirements

**Auto-installed**: Python 3.8+, NumPy, Pandas, SciPy, statsmodels, Plotly, Matplotlib  
**Platform**: Google Colab (recommended) or local Jupyter  
**Prerequisites**: Basic algebra; curiosity essential; fear of statistics optional (we'll fix that!)

---

## 📧 Support

📧 aloksu@gmail.com | 💬 [GitHub Issues](https://github.com/The-Pattern-Hunter/interactive-ecology-biometry/issues) | 📚 [Main README](../)

---

## 📜 License

**MIT License** - Free to use, modify, distribute with attribution.

Copyright © 2024 Susama Kar & Dr. Alok Patel

---

<div align="center">

**📊 Unit 4: Biometry - Statistics with the Pattern Hunter Philosophy 📊**

**9 Interactive Notebooks • Distributions • Descriptive Stats • Sampling • Hypothesis Tests • Design • Regression • ANOVA**

**The Stethoscope Analogy: Statistical Distributions as Diagnostic Instruments**

[📓 Previous: Unit 3](../unit-3-community/) | [🏠 Home](../)

**Made with 💚 by Dr. Alok Patel & Ms. Susama Kar**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.14463277.svg)](https://doi.org/10.5281/zenodo.14463277)

</div>
