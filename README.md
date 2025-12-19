# 🌿 Interactive Ecology & Biometry Notebooks

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/The-Pattern-Hunter/interactive-ecology-biometry)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.14463277.svg)](https://doi.org/10.5281/zenodo.14463277)

> **Comprehensive, interactive Jupyter notebooks for learning ecology and biometry with Python**

---

## 📖 Overview

This repository contains **20 professional, interactive notebooks** covering fundamental concepts in ecology and biometry. Each notebook combines:

- 🎓 **Clear explanations** of ecological concepts
- 💻 **Working Python code** with real data
- 📊 **Interactive visualizations** using Plotly
- 🔬 **Real-world examples** and case studies
- ✅ **Hands-on exercises** for practice
- 📚 **Mathematical models** with simulations

Perfect for:
- **Students** learning ecology and data analysis
- **Educators** teaching quantitative ecology
- **Researchers** exploring ecological models
- **Self-learners** interested in environmental science

---

## 🚀 Quick Start

### Option 1: Google Colab (Easiest - No Installation!)

Click any "Open in Colab" badge in the notebooks and start immediately!

### Option 2: Local Installation
```bash
# Clone repository
git clone https://github.com/The-Pattern-Hunter/interactive-ecology-biometry.git
cd interactive-ecology-biometry

# Install dependencies
pip install numpy pandas plotly matplotlib scipy networkx

# Launch Jupyter
jupyter notebook
```

---

## 📚 Course Structure

### **Unit 1: Introduction to Ecology** (5 notebooks) ✅

Foundational concepts and ecosystem dynamics

1. **[What is Ecology?](unit-1-intro/notebooks/01_what_is_ecology.ipynb)**
   - Levels of organization
   - Ecological principles
   - Scientific method in ecology

2. **[Ecosystem Components](unit-1-intro/notebooks/02_ecosystem_components.ipynb)**
   - Biotic and abiotic factors
   - Energy flow
   - Nutrient cycling

3. **[Energy Flow](unit-1-intro/notebooks/03_energy_flow.ipynb)**
   - Trophic levels
   - Energy pyramids
   - Production and respiration

4. **[Nutrient Cycles](unit-1-intro/notebooks/04_nutrient_cycles.ipynb)**
   - Carbon cycle
   - Nitrogen cycle
   - Phosphorus cycle

5. **[Biomes](unit-1-intro/notebooks/05_biomes.ipynb)**
   - World biome distribution
   - Climate and vegetation
   - Biome characteristics

---

### **Unit 2: Population Ecology** (5 notebooks) ✅

Population dynamics, growth, and regulation

1. **[Population Growth Models](unit-2-population/notebooks/01_population_growth_models.ipynb)**
   - Exponential growth (J-curve)
   - Logistic growth (S-curve)
   - r vs K selection
   - Human population dynamics

2. **[Life Tables & Survivorship](unit-2-population/notebooks/02_life_tables_survivorship.ipynb)**
   - Cohort vs static life tables
   - Type I, II, III survivorship curves
   - Dall sheep case study
   - Salmon mortality patterns

3. **[Age Structure & Demography](unit-2-population/notebooks/03_age_structure_demography.ipynb)**
   - Population pyramids
   - Dependency ratios
   - Demographic transition model
   - Population momentum

4. **[Population Regulation](unit-2-population/notebooks/04_population_regulation.ipynb)**
   - Density-dependent vs independent factors
   - Intraspecific competition
   - Allee effects
   - Predator-prey cycles (Lotka-Volterra)

5. **[Metapopulations](unit-2-population/notebooks/05_metapopulations.ipynb)**
   - Levins model
   - Source-sink dynamics
   - Connectivity and rescue effects
   - Fragmented landscapes

---

### **Unit 3: Community Ecology** (5 notebooks) ✅

Species interactions and community patterns

1. **[Species Interactions](unit-3-community/notebooks/01_species_interactions.ipynb)**
   - Competition (Lotka-Volterra)
   - Predation models
   - Mutualism
   - Interaction networks

2. **[Community Structure & Diversity](unit-3-community/notebooks/02_community_structure_diversity.ipynb)**
   - Shannon diversity index
   - Simpson's index
   - Rank-abundance curves
   - Species evenness

3. **[Ecological Succession](unit-3-community/notebooks/03_ecological_succession.ipynb)**
   - Primary vs secondary succession
   - Pioneer species
   - Mt. St. Helens case study
   - Krakatoa recolonization

4. **[Keystone Species & Trophic Cascades](unit-3-community/notebooks/04_keystone_species_cascades.ipynb)**
   - Sea otter-kelp system
   - Wolves in Yellowstone
   - Trophic cascade dynamics
   - Conservation implications

5. **[Island Biogeography](unit-3-community/notebooks/05_island_biogeography.ipynb)**
   - MacArthur-Wilson theory
   - Species-area relationship
   - Habitat fragmentation
   - Reserve design (SLOSS debate)

---

### **Unit 4: Statistical Methods** (6 notebooks) ✅

Quantitative analysis for ecology

1. **[Descriptive Statistics](unit-4-statistics/notebooks/01_descriptive_statistics.ipynb)**
   - Central tendency
   - Dispersion measures
   - Data visualization
   - Distribution shapes

2. **[Probability Distributions](unit-4-statistics/notebooks/02_probability_distributions.ipynb)**
   - Normal distribution
   - Binomial distribution
   - Poisson distribution
   - Ecological applications

3. **[Hypothesis Testing](unit-4-statistics/notebooks/03_hypothesis_testing.ipynb)**
   - t-tests
   - ANOVA
   - Chi-square tests
   - P-values and confidence intervals

4. **[Regression Analysis](unit-4-statistics/notebooks/04_regression_analysis.ipynb)**
   - Linear regression
   - Multiple regression
   - Model diagnostics
   - Prediction and interpretation

5. **[Experimental Design](unit-4-statistics/notebooks/05_experimental_design.ipynb)**
   - Randomization
   - Replication
   - Blocking
   - Factorial designs

6. **[Multivariate Analysis](unit-4-statistics/notebooks/06_multivariate_analysis.ipynb)**
   - PCA (Principal Component Analysis)
   - Cluster analysis
   - Ordination
   - Community analysis

---

## 🛠️ Technologies Used

- **Python 3.8+**: Core programming language
- **NumPy**: Numerical computations
- **Pandas**: Data manipulation
- **Plotly**: Interactive visualizations
- **Matplotlib**: Static plots
- **SciPy**: Scientific computing
- **NetworkX**: Network analysis
- **Jupyter**: Interactive notebooks

---

## 📊 Features

### Interactive Visualizations

All notebooks use **Plotly** for interactive plots:
- Zoom, pan, and explore data
- Hover for detailed information
- Toggle traces on/off
- Export high-quality figures

### Real Data Examples

Notebooks include real ecological datasets:
- Hudson Bay fur trade records (lynx-hare cycles)
- Dall sheep mortality data
- Mt. St. Helens succession
- Yellowstone wolf reintroduction
- Human population statistics

### Reproducible Code

Every analysis is:
- Fully documented with comments
- Reproducible with provided code
- Extensible for your own data
- Follows best practices

### Educational Focus

Designed for learning:
- Clear explanations before code
- Step-by-step progressions
- Visual analogies and diagrams
- Summary sections
- Practice opportunities

---

## 🎯 Learning Outcomes

By completing these notebooks, you will be able to:

### Conceptual Understanding
- Explain fundamental ecological principles
- Describe population and community dynamics
- Understand ecosystem processes
- Apply ecological theory to real systems

### Quantitative Skills
- Model population growth
- Analyze species interactions
- Calculate diversity indices
- Interpret statistical tests
- Design ecological experiments

### Programming Proficiency
- Write Python code for ecological analysis
- Create professional visualizations
- Manipulate ecological datasets
- Implement mathematical models
- Conduct reproducible research

---

## 📖 How to Use

### For Students

1. **Follow in order**: Units build on each other
2. **Run all cells**: Execute code to see outputs
3. **Modify parameters**: Experiment with values
4. **Complete exercises**: Practice problems included
5. **Apply to data**: Use your own datasets

### For Educators

1. **Lecture material**: Use notebooks in class
2. **Lab exercises**: Students run analyses
3. **Assignments**: Modify problems for homework
4. **Demonstrations**: Interactive visualizations
5. **Customization**: Adapt to your curriculum

### For Researchers

1. **Quick reference**: Find methods and formulas
2. **Code templates**: Adapt for your analysis
3. **Model implementations**: Pre-built ecological models
4. **Visualization tools**: Publication-quality plots
5. **Methodology**: Reproducible workflows

---

## 🤝 Contributing

We welcome contributions! Please:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/AmazingFeature`)
3. **Commit** your changes (`git commit -m 'Add some AmazingFeature'`)
4. **Push** to the branch (`git push origin feature/AmazingFeature`)
5. **Open** a Pull Request

### Contribution Ideas

- Add new notebooks for additional topics
- Improve existing explanations
- Fix errors or typos
- Add datasets or examples
- Enhance visualizations
- Translate to other languages

---

## 📝 Citation

If you use these notebooks in your research or teaching, please cite:
```bibtex
@software{interactive_ecology_biometry_2024,
  author       = {Ms. Susama Kar & Dr. Alok Patel},
  title        = {Interactive Ecology & Biometry Notebooks},
  year         = 2024,
  publisher    = {Zenodo},
  doi          = {10.5281/zenodo.14463277},
  url          = {https://github.com/The-Pattern-Hunter/interactive-ecology-biometry}
}
```

**DOI**: [10.5281/zenodo.14463277](https://doi.org/10.5281/zenodo.14463277)

---

## 📜 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

### What This Means

✅ **Free to use** for any purpose  
✅ **Modify** and adapt as needed  
✅ **Share** with others  
✅ **Use in commercial projects**  
✅ **No warranty** (use at your own risk)

---

## 🙏 Acknowledgments

- **Data sources**: Hudson Bay Company, USGS, UN Population Division
- **Inspiration**: Classic ecology textbooks (Begon, Harper & Townsend)
- **Tools**: Jupyter Project, Plotly, Python community
- **Case studies**: Real ecological research and datasets

---

## 📧 Contact

**The Pattern Hunter Team**

- 📧 Email: aloksu@gmail.com (example)
- 🐙 GitHub: [@The-Pattern-Hunter](https://github.com/The-Pattern-Hunter)
- 🌐 Website: [patternhunter.org](https://patternhunter.org) (example)

---

## 🗺️ Roadmap

### Current Status: **20/20 notebooks complete** ✅

### Completed Units:
- ✅ Unit 1: Introduction to Ecology (5 notebooks)
- ✅ Unit 2: Population Ecology (5 notebooks)
- ✅ Unit 3: Community Ecology (5 notebooks)
- ✅ Unit 4: Statistical Methods (6 notebooks)

### Future Plans:
- 🔄 Unit 5: Ecosystem Ecology (planned)
- 🔄 Unit 6: Conservation Biology (planned)
- 🔄 Unit 7: Landscape Ecology (planned)
- 🔄 Advanced topics and specialized modules

---

## 📈 Repository Stats

- **Total Notebooks**: 20
- **Total Units**: 4 (complete)
- **Programming Language**: Python
- **Interactive Plots**: Plotly
- **License**: MIT
- **Status**: Active Development

---

## 🌟 Star History

If you find these notebooks useful, please ⭐ **star** this repository!

[![Star History Chart](https://api.star-history.com/svg?repos=The-Pattern-Hunter/interactive-ecology-biometry&type=Date)](https://star-history.com/#The-Pattern-Hunter/interactive-ecology-biometry&Date)

---

## 📚 Related Resources

### Textbooks
- Begon, Harper & Townsend - *Ecology: From Individuals to Ecosystems*
- Gotelli - *A Primer of Ecology*
- Stevens - *The Ecological Detective*

### Online Courses
- [Coursera: Introduction to Ecology](https://www.coursera.org)
- [edX: Ecology and Conservation](https://www.edx.org)

### Tools & Software
- [R for Ecology](https://www.r-project.org/)
- [Python Scientific Stack](https://www.scipy.org/)
- [Jupyter Project](https://jupyter.org/)

---

## 💬 FAQ

### Q: Do I need prior programming experience?
**A**: Basic Python knowledge helps, but notebooks include explanations. Start with Unit 1!

### Q: Can I use these for teaching?
**A**: Yes! That's exactly what they're designed for. MIT License allows free use.

### Q: How do I report bugs or issues?
**A**: Open an issue on GitHub with details about the problem.

### Q: Can I contribute my own notebooks?
**A**: Absolutely! Fork the repo and submit a pull request.

### Q: Are solutions provided for exercises?
**A**: Some notebooks include worked examples. More solutions coming soon!

### Q: Can I use my own data?
**A**: Yes! Code is designed to be adaptable to your datasets.

---

<div align="center">

## 🌿 Learn Ecology Through Code 🌿

**Made with 💚 by The Pattern Hunter Team**

⭐ **Star us on GitHub** | 🍴 **Fork** | 📢 **Share**

[📚 Explore Notebooks](unit-1-intro/) | [🐛 Report Issue](https://github.com/The-Pattern-Hunter/interactive-ecology-biometry/issues) | [💬 Discussions](https://github.com/The-Pattern-Hunter/interactive-ecology-biometry/discussions)

</div>
