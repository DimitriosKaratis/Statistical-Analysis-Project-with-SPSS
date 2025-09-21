# Statistical Analysis Project (SPSS)

This repository contains the implementation of a project in **Statistics**, focusing on descriptive analysis, hypothesis testing, confidence intervals, correlation, and regression modeling using **SPSS**.  
The work was developed as part of the *Statistics* course at the **Department of Electrical and Computer Engineering, Aristotle University of Thessaloniki (AUTH).**

---

## 📘 Study A – Descriptive and Comparative Analysis

### Tasks
1. **Descriptive Statistics**:  
   - Computed measures of central tendency (mean, median) and variability (variance, standard deviation, range, quartiles).  
   - Constructed histograms and boxplots for two players (Player A and Player B – our dataset).  

2. **Confidence Intervals for Variance & Standard Deviation**:  
   - Built 95% confidence intervals for σ² and σ.  

3. **Confidence Intervals for the Mean**:  
   - Calculated both 90% and 95% confidence intervals.  
   - Compared the means between Player A and Player B.  

4. **Comparison of Means**:  
   - Hypothesis testing of differences in average solving times for Sudoku puzzles.  

### Results & Observations
- Player A’s sample appeared **closer to normal distribution**, while Player B’s sample deviated from normality, showing skewness towards lower solving times.  
- Descriptive stats confirmed:  
  - Player A had **higher mean solving time** and **greater variability**.  
  - Player B (our data) had **lower average solving time** and slightly reduced variance.  
- 95% confidence intervals:  
  - Variability was **slightly higher** for Player A ([26.71, 39.94]) than Player B ([19.51, 32.93]).  
- For both confidence levels (90% & 95%), the mean solving time of Player B was **significantly lower** than that of Player A.  
- Threshold of **40 minutes** (to be considered a "good" player) was below the confidence intervals of both players, so neither met this criterion.

### Conclusions
- **Player B outperformed Player A** in average Sudoku solving time.  
- Variability between the two players was not drastically different, but Player A showed slightly more dispersion.  
- Neither player reached the benchmark of "good performance" (≤ 40 minutes).  

---

## 📘 Study B – Correlation and Regression Analysis

### Tasks
5. **Scatterplots**:  
   - Built scatterplots of solving time vs. day (“experience”).  

6. **Correlation Analysis**:  
   - Pearson correlation coefficients between time and day for both players.  

7. **Linear Regression (Least Squares Method)**:  
   - Estimated regression models:  
     - Player A: *time = 145.318 – 0.622 × day*  
     - Player B: *time = 94.609 – 0.618 × day*  

8. **Quarter Predictions**:  
   - Used regression to predict times at the 1st and 3rd quartiles of days.  

9. **Piecewise Regression**:  
   - Compared regression slopes in first vs. second half of days for each player.  

10. **Learning Rate Comparison**:  
   - Analyzed differences in performance improvement over time.  

### Results & Observations
- Correlations were **negative and significant**:  
  - Player A: r = –0.781  
  - Player B: r = –0.820  
  - Both show improvement with experience (time decreases as days increase).  
- Regression slopes:  
  - Nearly identical (–0.622 vs. –0.618), suggesting similar **learning rates**.  
- Predictions:  
  - Player A: from ~121.7 minutes at Q1 → ~75.0 minutes at Q3.  
  - Player B: from ~79.2 minutes at Q1 → ~48.3 minutes at Q3.  
- Piecewise regression:  
  - Player A’s improvement accelerated in the second half (slope –0.755 vs. –0.622).  
  - Player B’s learning rate remained stable across both halves (–0.408 vs. –0.438).  

### Conclusions
- Both players demonstrated **consistent learning effects** with experience.  
- Player B consistently maintained **lower solving times**, confirming better performance.  
- Player A improved more rapidly in later days, while Player B’s improvement was **steady and stable**.  
- Linear regression models were reliable within the observed intervals but unrealistic for extreme extrapolation (predicting negative times).  

---

## 🔧 Tools & Methods
- **SPSS** for descriptive statistics, hypothesis testing, correlation, and regression.  
- **Histograms, Boxplots, Scatterplots** for visual analysis.  
- **Confidence Intervals** and **t-tests** for statistical inference.
- Reports are written in Greek, while the README provides an English overview.   
