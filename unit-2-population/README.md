# 👥 Unit 2: Population Ecology

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/The-Pattern-Hunter/interactive-ecology-biometry/blob/main/unit-2-population/)

---

## 📖 Overview

This unit explores how populations grow, decline, and persist over time and space. Through five interactive notebooks, students investigate mathematical models of population growth, analyze survival patterns across life stages, examine age structure and demographic transitions, understand mechanisms of population regulation, and discover how spatially-separated populations connect through metapopulation dynamics.

**Philosophy:** Population ecology is inherently quantitative, yet students discover **growth curve patterns visually** before encountering differential equations. Real demographic data (human populations, Dall sheep, Kaibab deer) grounds every concept in ecological reality.

---

## 🎯 Unit Learning Outcomes

By completing this unit, you will be able to:

1. **Model population growth** using exponential and logistic equations
2. **Construct and interpret life tables** and survivorship curves
3. **Analyze age structure** and predict demographic transitions
4. **Explain population regulation** mechanisms (density-dependent and independent)
5. **Apply metapopulation theory** to fragmented habitats
6. **Distinguish r-selection from K-selection** life history strategies
7. **Use real demographic data** to calculate vital rates and project populations
8. **Connect mathematical models** to observable patterns in nature

---

## 📚 Notebooks

### 1. Population Growth Models 📈

**Topics**: Exponential growth, logistic growth, r vs K selection, carrying capacity, growth rate parameters

**Key Concepts**:

**Exponential Growth**:
- **Model**: dN/dt = rN  or  N(t) = N₀e^(rt)
- **Assumptions**: Unlimited resources, no competition, constant birth/death rates
- **Pattern**: J-shaped curve, accelerating growth
- **Parameter r**: Intrinsic rate of increase (per capita growth rate)
  - r > 0: Population grows
  - r = 0: Stable population
  - r < 0: Population declines
- **Doubling time**: t_d = ln(2) / r ≈ 0.693 / r
- **When realistic**: Invasive species, bacterial growth, recovering populations

**Logistic Growth**:
- **Model**: dN/dt = rN(1 - N/K)  or  N(t) = K / (1 + ((K-N₀)/N₀)e^(-rt))
- **Assumptions**: Limited resources, intraspecific competition, density-dependent regulation
- **Pattern**: S-shaped curve, levels off at carrying capacity
- **Parameter K**: Carrying capacity (maximum sustainable population)
- **Parameter r**: Still intrinsic growth rate, but now modulated by (1-N/K)
- **Inflection point**: At N = K/2 (maximum growth rate)
- **When realistic**: Most populations in stable environments

**Comparing Models**:
```
EXPONENTIAL                    LOGISTIC
-----------                    ---------
Unlimited growth               Levels off at K
J-curve                        S-curve
Never stops                    Equilibrium at K
Unrealistic long-term          More realistic
r controls everything          Both r and K matter
```

**r vs K Selection**:
- **r-selected species**: 
  - High r, low K
  - Many small offspring, minimal parental care
  - Short-lived, early maturity
  - Opportunistic, colonizers
  - Examples: Insects, weeds, bacteria
  
- **K-selected species**:
  - Low r, high K
  - Few large offspring, extensive parental care
  - Long-lived, delayed maturity
  - Competitive, stable environments
  - Examples: Elephants, whales, trees, humans

**Interactive Visualizations**:
- Growth curve explorer (adjust r, K, N₀)
- Exponential vs logistic comparison
- Doubling time calculator
- r-K selection strategy spectrum
- Real population data fitting (bacteria, human, deer)

**Pattern Recognition**: Population growth curves have **recognizable shapes** (J vs S). The shape reveals the underlying process (unlimited vs limited resources). Parameters r and K define the entire curve - understand them visually before formulas.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/The-Pattern-Hunter/interactive-ecology-biometry/blob/main/unit-2-population/notebooks/01_population_growth_models.ipynb)

**Learning Time**: ~2 hours

**Real Data**: 
- Human population growth (1 CE - 2050)
- Bacterial growth in culture
- Reindeer on St. Paul Island (overshoot and crash)
- Kaibab deer population (1906-1939)

---

### 2. Life Tables & Survivorship 📊

**Topics**: Life table construction, survivorship curves (Type I/II/III), age-specific mortality, life expectancy

**Key Concepts**:

**Life Table Components**:
- **x**: Age class
- **n_x**: Number alive at start of age x
- **d_x**: Number dying during age x
- **q_x**: Age-specific mortality rate = d_x / n_x
- **l_x**: Proportion surviving to age x = n_x / n₀
- **e_x**: Life expectancy at age x (average years remaining)

**Life Table Types**:
- **Cohort (horizontal)**: Follow one cohort from birth to death (ideal but difficult)
- **Static (vertical)**: Snapshot of all ages at one time (practical)
- **Assumptions**: Stable age distribution, constant vital rates

**Survivorship Curves**:

**Type I** (Convex):
- High survival through youth and middle age
- Most mortality in old age
- Heavy parental investment
- Examples: Humans, elephants, large mammals
- Pattern: l_x stays high, drops steeply at end

**Type II** (Linear):
- Constant mortality rate across ages
- Equal chance of dying at any age
- Moderate parental care
- Examples: Birds, rodents, some reptiles
- Pattern: l_x declines steadily, straight line on log scale

**Type III** (Concave):
- High mortality in early life
- Survivors live long
- Little parental care, many offspring
- Examples: Fish, marine invertebrates, plants
- Examples: Most eggs/seeds die, few reach adulthood
- Pattern: l_x drops sharply early, flattens later

**Survival vs Mortality**:
- Survivorship: l_x (proportion alive)
- Mortality: q_x (proportion dying)
- Complementary patterns: high early mortality → Type III

**Life Expectancy**:
- e_x = Average years remaining at age x
- Often decreases with age (not always!)
- e₀ = Life expectancy at birth (key demographic parameter)

**Interactive Visualizations**:
- Life table calculator (input data, auto-compute all columns)
- Survivorship curve plotter (log scale)
- Type I/II/III comparison
- Real Dall sheep life table (classic dataset)
- Human life table explorer (country/year comparisons)

**Pattern Recognition**: **Survivorship curves reveal life history strategies** visually. Type I = invest heavily in few offspring. Type III = produce many, invest little. Type II = intermediate. The curve SHAPE tells the story - no formula memorization needed first.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/The-Pattern-Hunter/interactive-ecology-biometry/blob/main/unit-2-population/notebooks/02_life_tables_survivorship.ipynb)

**Learning Time**: ~1.5-2 hours

**Real Data**:
- Dall mountain sheep (Murie, 1944) - classic Type I
- Hydra (lab organism) - Type II
- Oyster larvae - Type III
- Human life tables (USA, Nigeria, Japan)

---

### 3. Age Structure & Demography 🏛️

**Topics**: Age pyramids, demographic transition, population momentum, dependency ratios

**Key Concepts**:

**Age Structure Diagrams (Population Pyramids)**:
- **X-axis**: Number or % of population
- **Y-axis**: Age classes (0-4, 5-9, ..., 85+)
- **Split by sex**: Males left, females right
- **Shape reveals demographic status**:

**Pyramid Shapes**:

**Expanding (Triangle)**:
- Wide base, narrow top
- High birth rate, high death rate
- Young population, rapid growth
- Characteristic of developing countries
- Example: Nigeria, Kenya
- **Momentum**: Will grow even if birth rate drops (many reproductive-age individuals)

**Stationary (Column)**:
- Relatively equal width across ages
- Low birth rate, low death rate
- Stable population (r ≈ 0)
- Characteristic of developed countries
- Example: USA, Canada

**Contracting (Inverted)**:
- Narrow base, wide middle
- Very low birth rate, low death rate
- Aging population, declining
- Characteristic of post-industrial countries
- Example: Japan, Italy, Germany
- **Challenges**: Fewer workers supporting more retirees

**Demographic Transition Model**:

**Stage 1** (Pre-transition):
- High birth rate, high death rate
- Stable population, low life expectancy
- Pre-industrial societies

**Stage 2** (Early transition):
- High birth rate, declining death rate
- Rapid population growth
- Better healthcare, nutrition
- Example: Most of 1800s Europe

**Stage 3** (Late transition):
- Declining birth rate, low death rate
- Slowing growth
- Urbanization, education, contraception
- Example: Mexico, Brazil

**Stage 4** (Post-transition):
- Low birth rate, low death rate
- Stable or declining population
- High life expectancy, aging
- Example: Most of Europe, Japan

**Stage 5** (Possible):
- Very low birth rate (below replacement)
- Population decline
- Severe aging
- Example: Japan, Italy

**Dependency Ratios**:
- **Youth dependency**: (age 0-14) / (age 15-64)
- **Old-age dependency**: (age 65+) / (age 15-64)
- **Total dependency**: (0-14 + 65+) / (15-64)
- High ratios = fewer workers per dependent

**Population Momentum**:
- Even if fertility drops to replacement (2.1 children/woman), population continues growing
- Why? Large cohorts of reproductive-age individuals
- Can take 50-70 years to stabilize
- Important for projections

**Interactive Visualizations**:
- Age pyramid builder (adjust birth/death rates)
- Country comparisons (Nigeria vs Japan vs USA)
- Demographic transition animation (1800-2100)
- Dependency ratio calculator
- Population projection simulator

**Pattern Recognition**: **Pyramid SHAPE predicts future** without calculations. Triangle = growth, Column = stable, Inverted = decline. Demographic transition follows predictable pattern across countries - timing varies but sequence is consistent.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/The-Pattern-Hunter/interactive-ecology-biometry/blob/main/unit-2-population/notebooks/03_age_structure_demography.ipynb)

**Learning Time**: ~1.5-2 hours

**Real Data**:
- Human age pyramids (200+ countries, 1950-2100)
- UN Population Division projections
- Historical demographic transitions (Sweden, Japan)
- COVID-19 impacts on age structure

---

### 4. Population Regulation 🎚️

**Topics**: Density-dependent factors, density-independent factors, predator-prey cycles, competition

**Key Concepts**:

**Density-Dependent Factors**:
- Effect **strengthens** as population density increases
- Provide negative feedback (regulate population)
- **Types**:
  - **Competition** (intraspecific): For food, space, mates
  - **Predation**: More prey attracts more predators
  - **Disease**: Spreads faster in dense populations
  - **Parasitism**: Transmission increases with density
  - **Territoriality**: Limited territories cap population
  - **Waste accumulation**: Toxic at high density

- **How they work**: As N increases → per capita resources decrease → birth rate falls and/or death rate rises → N levels off
- **Result**: Population oscillates around K (carrying capacity)

**Density-Independent Factors**:
- Effect **same** regardless of population density
- No feedback, can't regulate (but can limit)
- **Types**:
  - **Weather**: Droughts, floods, heat waves, cold snaps
  - **Natural disasters**: Fires, hurricanes, earthquakes, volcanic eruptions
  - **Seasonal changes**: Winter kill regardless of density
  - **Habitat destruction**: Human-caused, non-selective

- **How they work**: Random mortality events, no relationship to N
- **Result**: Population crashes, then may recover (if survivors remain)

**Predator-Prey Dynamics (Lotka-Volterra Model)**:

**Equations**:
```
Prey:     dN/dt = rN - aNP
Predator: dP/dt = baNP - mP
```

Where:
- N = Prey population
- P = Predator population
- r = Prey growth rate
- a = Attack rate (predation efficiency)
- b = Conversion efficiency (prey → predator biomass)
- m = Predator mortality rate

**Predicted Pattern**:
- Coupled oscillations
- Prey peaks BEFORE predator peaks (time lag)
- Predator increase drives prey decrease
- Prey decrease causes predator decrease
- Cycle repeats indefinitely (in model)

**Real-world modifications**:
- Cycles dampen (not perpetual)
- Prey refuges stabilize
- Alternative prey buffers
- Environmental variation adds noise

**Classic Example: Hare-Lynx Cycles**:
- Hudson Bay Company fur records (1845-1935)
- ~10-year cycles
- Lynx tracks hare with ~2-year lag
- One of ecology's most famous datasets

**Competition**:

**Intraspecific** (within species):
- Scramble: All get less (interference)
- Contest: Some get all, others nothing (territoriality)
- Both are density-dependent

**Interspecific** (between species):
- Competitive exclusion (Gause's principle)
- Niche partitioning (coexistence)
- Covered more in Unit 3

**Allee Effects**:
- Positive density dependence at LOW densities
- Too few individuals → problems:
  - Difficulty finding mates
  - Reduced genetic diversity
  - Inability to defend against predators
  - Loss of social structure
- Creates minimum viable population size
- Important for conservation (small populations vulnerable)

**Interactive Visualizations**:
- Density-dependent vs independent comparison
- Lotka-Volterra simulator (adjust parameters, watch cycles)
- Hare-lynx historical data plotter
- Competition outcome predictor
- Allee effect threshold explorer

**Pattern Recognition**: **Density-dependent factors create oscillations** around K. Predator-prey systems show predictable phase-shifted cycles. Density-independent factors cause irregular crashes. The PATTERN of population change reveals the regulatory mechanism.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/The-Pattern-Hunter/interactive-ecology-biometry/blob/main/unit-2-population/notebooks/04_population_regulation.ipynb)

**Learning Time**: ~2 hours

**Real Data**:
- Hare-lynx cycles (Hudson Bay, 1845-1935)
- Kaibab deer irruption and crash (1906-1939)
- Reindeer on St. Paul Island (overshoot)
- Lemming population cycles (Norway)

---

### 5. Metapopulations 🗺️

**Topics**: Metapopulation concept, source-sink dynamics, extinction-colonization balance, fragmented habitats

**Key Concepts**:

**Metapopulation Definition**:
- "Population of populations"
- Set of local populations connected by dispersal
- Each patch can go extinct and be recolonized
- Persistence depends on regional dynamics, not just local

**Why Metapopulations Matter**:
- Habitat fragmentation (human-caused)
- Many species now exist as metapopulations
- Conservation requires landscape-scale thinking
- Corridors connect patches
- Rescue effect can prevent local extinction

**Levins Metapopulation Model**:

**Equation**:
```
dp/dt = cp(1-p) - ep
```

Where:
- p = Proportion of patches occupied
- c = Colonization rate
- e = Extinction rate
- cp(1-p) = Colonization (more occupied → more colonizers, more empty → more targets)
- ep = Extinction (more occupied → more go extinct)

**Equilibrium**:
```
p* = 1 - (e/c)
```

**Metapopulation persists if**: c > e (colonization exceeds extinction)

**Predictions**:
- If c > e: Metapopulation persists at equilibrium p*
- If c < e: All patches eventually go extinct (doomed)
- If c = e: Critical threshold (unstable)

**Assumptions** (often violated in reality):
- All patches equal quality
- All equally connected
- Patch dynamics independent
- No rescue effect

**Source-Sink Dynamics**:

**Source populations**:
- Birth rate > Death rate (b > d)
- Produces surplus individuals
- Emigrants colonize other patches
- Self-sustaining

**Sink populations**:
- Death rate > Birth rate (d > b)
- Requires immigration to persist
- Cannot sustain without source
- May occupy marginal habitat

**Why sinks exist**:
- Habitat quality varies
- Individuals disperse randomly
- Some land in poor habitat
- Maintained by immigration

**Conservation implications**:
- Protect sources primarily
- But sinks can still contribute (genetic diversity, buffer)
- Corridor quality matters

**Rescue Effect**:
- Immigration prevents local extinction
- Even struggling populations can persist
- Reduces extinction rate (e) in model
- Important in highly connected metapopulations

**Extinction Vortex** (opposite of rescue):
- Small population → Allee effects
- → Fewer emigrants → Less colonization
- → More local extinctions → Smaller metapopulation
- → Positive feedback → Collapse

**Patch Occupancy Patterns**:
- **Mainland-island**: One large source, many small sinks
- **Patchy**: Many equal patches, balanced dynamics
- **Source-sink**: Mix of high and low quality
- **Stepping stones**: Linear corridor of patches

**Habitat Fragmentation Effects**:
- Reduces patch size → Higher extinction rate
- Increases isolation → Lower colonization rate
- Below threshold (c < e) → Metapopulation collapse
- Corridors increase c, mitigate fragmentation

**Interactive Visualizations**:
- Levins model simulator (adjust c, e, watch p over time)
- Equilibrium calculator (find p* from c and e)
- Patch network visualizer (colonization/extinction events)
- Source-sink map builder
- Fragmentation impact explorer

**Pattern Recognition**: **Metapopulation persistence depends on BALANCE** between colonization and extinction. If c > e, the metapopulation survives even though individual patches blink on and off. Habitat connectivity (corridors) increases c. Fragmentation increases e. Conservation = tipping the balance.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/The-Pattern-Hunter/interactive-ecology-biometry/blob/main/unit-2-population/notebooks/05_metapopulations.ipynb)

**Learning Time**: ~1.5 hours

**Real Examples**:
- Checkerspot butterfly (Edith's checkerspot in California)
- Pika populations in mountain patches
- Pond-breeding amphibians
- Forest bird populations in fragmented landscapes

---

## 🎨 Pattern Hunter Integration

### Patterns Discovered in Unit 2:

1. **Growth Curve Patterns**:
   - J-curve = Exponential (unlimited resources)
   - S-curve = Logistic (limited resources)
   - Shape reveals underlying process
   - Parameters r and K define entire curve

2. **Survivorship Patterns**:
   - Type I (convex) = High parental investment
   - Type II (linear) = Constant mortality
   - Type III (concave) = Many offspring, low care
   - Curve shape = life history strategy

3. **Age Structure Patterns**:
   - Triangle = Rapid growth (expanding)
   - Column = Stable (stationary)
   - Inverted = Decline (contracting)
   - Shape predicts future

4. **Oscillation Patterns**:
   - Predator-prey cycles (phase-shifted)
   - Density-dependent = Regular oscillations
   - Density-independent = Irregular crashes
   - Pattern reveals regulation mechanism

5. **Metapopulation Patterns**:
   - Blinking patches (extinction-colonization)
   - Source-sink flows (directional)
   - Connectivity maintains persistence
   - Network structure matters

### Pedagogical Approach:

**See the pattern FIRST**:
- Plot growth curves BEFORE dN/dt = rN
- Visualize survivorship BEFORE calculating l_x
- Examine pyramids BEFORE demographic formulas
- Watch predator-prey oscillate BEFORE Lotka-Volterra
- Map metapopulations BEFORE Levins model

**Then formulas make sense** as descriptions of observed patterns.

---

## 🔗 Connections to Other Units

### From Unit 1 (Ecosystem Ecology):
- Energy flow → Resources limit population growth (K)
- Nutrient cycles → Resources affect birth/death rates
- Limiting factors → Determine carrying capacity
- Decomposition → Nutrient availability influences r

### To Unit 3 (Community Ecology):
- Predator-prey → Species interactions
- Competition → Niche partitioning
- Metapopulations → Community assembly
- Life history → Succession roles

### To Unit 4 (Biometry):
- Growth models → Exponential functions
- Life tables → Probability and expectation
- Age structure → Frequency distributions
- Population regulation → Time series analysis
- Metapopulations → Stochastic processes

---

## 📊 Interactive Features

All notebooks include:

✅ **Learning objectives** (8-9 per notebook)  
✅ **Parameter sliders** (manipulate r, K, c, e, etc.)  
✅ **Real-time visualizations** (curves update instantly)  
✅ **Real demographic data** (humans, Dall sheep, hare-lynx)  
✅ **Pattern recognition prompts** ("What shape do you see?")  
✅ **Key insights** (boxed summaries)  
✅ **Discussion questions** (critical thinking)  
✅ **Code explanations** (commented for learners)  
✅ **Literature references** (classic papers cited)

---

## 🎓 Skills Developed

### Conceptual:
- Understanding exponential vs logistic growth
- Interpreting life history strategies from data
- Predicting demographic futures from age structure
- Recognizing regulatory mechanisms from time series
- Thinking spatially about fragmented populations

### Quantitative:
- Calculating population growth rates (r)
- Constructing and interpreting life tables
- Computing dependency ratios
- Parameterizing models from data
- Solving for equilibria (K, p*)

### Computational:
- Running population simulations
- Plotting growth curves and pyramids
- Animating predator-prey dynamics
- Visualizing metapopulation networks
- Fitting models to real data

### Analytical:
- Distinguishing density-dependent from independent
- Identifying source vs sink populations
- Evaluating conservation strategies
- Predicting extinction risk
- Designing corridors for connectivity

---

## 📖 Recommended Reading

### Classic Population Ecology:
- Gotelli, N. J. (2008). *A Primer of Ecology*. 4th edition.
- Vandermeer, J. H., & Goldberg, D. E. (2013). *Population Ecology: First Principles*. 2nd edition.

### Life Tables & Demography:
- Murie, A. (1944). *The Wolves of Mount McKinley*. [Dall sheep life table]
- Preston, S. H., Heuveline, P., & Guillot, M. (2000). *Demography: Measuring and Modeling Population Processes*.

### Predator-Prey Dynamics:
- Lotka, A. J. (1925). *Elements of Physical Biology*.
- Volterra, V. (1926). Fluctuations in the abundance of a species. *Nature*, 118, 558-560.

### Metapopulations:
- Levins, R. (1969). Some demographic and genetic consequences of environmental heterogeneity. *Bulletin of the Entomological Society of America*, 15, 237-240.
- Hanski, I. (1999). *Metapopulation Ecology*. Oxford University Press.

---

## 💡 Teaching & Learning Tips

### For Instructors:

1. **Start with curves, not equations**: Show growth plots, let students describe patterns
2. **Use sliders extensively**: Parameter exploration builds intuition
3. **Connect to current events**: Human population, COVID-19, invasive species
4. **Emphasize pattern → formula**: "This S-curve is described by dN/dt = rN(1-N/K)"
5. **Link to conservation**: Metapopulations, fragmentation, extinction risk
6. **Use real data**: Dall sheep, hare-lynx, human pyramids more engaging than hypotheticals

### For Students:

1. **Manipulate parameters**: Change r, K, c, e - predict outcome, then test
2. **Sketch curves first**: Draw what you expect before running code
3. **Compare shapes**: Exponential vs logistic, Type I vs III, expanding vs contracting
4. **Real-world connections**: How does this apply to human population? Conservation?
5. **Ask "what if"**: What if K drops? What if c < e? Build causal understanding
6. **Pattern before formula**: Understand the curve shape, then the math makes sense

### Suggested Pacing:

**Week 1**: Notebook 1 (Growth Models)  
**Week 2**: Notebook 2 (Life Tables)  
**Week 3**: Notebook 3 (Age Structure)  
**Week 4**: Notebook 4 (Regulation)  
**Week 5**: Notebook 5 (Metapopulations)

---

## 🔍 Assessment Ideas

### Formative:
- **Curve identification**: Show growth curve, identify exponential vs logistic
- **Pyramid interpretation**: Given age pyramid, predict growth trend
- **Parameter effects**: "If r doubles, how does doubling time change?"
- **Model selection**: "Which model fits this scenario?" (and why)

### Summative:
- **Life table construction**: Given raw data, build complete life table
- **Population projection**: Use age-specific rates to project 50 years
- **Regulation analysis**: Time series data, identify mechanism
- **Metapopulation design**: Propose corridor network for conservation

### Pattern Hunter:
- **Visual interpretation**: Describe pattern before calculating
- **Conceptual explanation**: "Why is survivorship Type III?" (mechanism, not just definition)
- **Parameter intuition**: "Sketch curve for r=0.5 vs r=1.5" (without calculator)
- **Model critique**: "When would logistic model fail?" (assumptions)

---

## 🌍 Real-World Applications

### Human Demography:
- Population projections (Social Security, healthcare planning)
- Demographic dividend vs burden
- Migration patterns and aging
- COVID-19 impacts on age structure

### Wildlife Management:
- Harvest quotas (sustainable yield)
- Endangered species recovery (minimum viable population)
- Invasive species control (r-selected)
- Reintroduction success (Allee effects)

### Conservation Biology:
- Habitat corridor design (metapopulations)
- Fragmentation impacts (extinction threshold)
- Protected area networks (sources)
- Climate change refugia (shifting habitats)

### Fisheries & Agriculture:
- Maximum sustainable yield
- Pest population dynamics (r-selected)
- Predator-prey in biological control
- Life history and harvest strategies

---

## 🛠️ Technical Requirements

### Auto-installed:
- Python 3.8+
- NumPy, Pandas
- Plotly, Matplotlib
- SciPy (ODE solvers)
- NetworkX (for metapopulation graphs)

### Hardware:
- Web browser (Colab)
- OR local Jupyter

### Prerequisites:
- **None!** Beginner-friendly
- Basic algebra helpful (exponentials)
- Curiosity essential

---

## 🤝 Contributing

Improvements welcome!

**Ideas**:
- Additional species examples
- More interactive simulations
- Clearer explanations
- Bug fixes
- Translations
- Exercise sets

**Process**:
1. Fork repository
2. Make changes
3. Test in Colab
4. Submit pull request

---

## 📧 Support

**Questions?**
- 📧 aloksu@gmail.com
- 💬 [GitHub Issues](https://github.com/The-Pattern-Hunter/interactive-ecology-biometry/issues)
- 📚 Main README

---

## 📜 License

**MIT License** - Free to use, modify, distribute with attribution.

Copyright © 2024 Susama Kar & Dr. Alok Patel

---

## 🎉 Acknowledgments

**Data sources**: UN Population Division, Hudson Bay Company, USGS, Murie (1944)  
**Classic papers**: Lotka, Volterra, Levins, Hanski  
**Philosophy**: Dr. Alok Patel's Pattern Hunter methodology  
**Tools**: Jupyter, Plotly, SciPy, NetworkX

---

<div align="center">

**👥 Unit 2: Population Ecology 👥**

**5 Interactive Notebooks • Growth Models • Life Tables • Demography • Regulation • Metapopulations**

[📓 Previous: Unit 1 - Ecosystem Ecology](../unit-1-ecosystem/) | [📓 Next: Unit 3 - Community Ecology](../unit-3-community/) | [🏠 Main Repository](../)

**Made with 💚 by Dr. Alok Patel & Ms. Susama Kar**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.14463277.svg)](https://doi.org/10.5281/zenodo.14463277)

</div>
