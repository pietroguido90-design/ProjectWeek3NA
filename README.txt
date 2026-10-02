Here is a professional, comprehensive, and engaging README.md file designed for your GitHub repository or project submission. It captures both the rigorous data science methodology and the storytelling tone we developed.
🇮🇹 The Mancini Effect: Data-Driven Impact Analysis & Italy 2030 World Cup Projection
"In Italy, you don't touch three things: Family, Food, and Football."
After recent World Cup heartbreaks, football anxiety is at an all-time high. This project brings objective Data Science to the rescue—measuring the real impact of manager Roberto Mancini and running predictive simulations for the Italy 2030 World Cup.
📋 Table of Contents
1. Project Overview
2. Research Questions
3. Dataset & Whitelist Engineering
4. Methodology & Performance Rating Model
5. Key Insights & Findings
6. Italy 2030 Predictive Simulation
7. Visualizations & Charts
8. Project Structure & Usage
9. Conclusion & Verdict
🎯 Project Overview
This project bridges sports analytics and predictive modeling to evaluate two core hypotheses:
1. The Managerial Impact ("The Mancini Effect"): Does a top-tier tactical manager systematically boost player performance across seasons, or is growth driven by natural career variance?
2. The 2030 Horizon: Will the Italian National Team possess a strong enough roster to comfortably qualify and compete at the 2030 World Cup?
Rather than relying on bar-room opinions, the pipeline cleans multi-season historical data, integrates advanced metrics (xG/xA), normalizes a player rating scale (5.0–10.0), and applies strict tactical constraints (4-3-3 formation) to evaluate future competitiveness.
❓ Research Questions
* How can we mathematically quantify a manager's influence on player development using multi-season data?
* What role do Expected Goals (xG) and Expected Assists (xA) play in stripping away short-term noise and luck?
* Does the projected 2030 squad surpass the UEFA minimum qualification threshold (7.10)?
⚙️ Dataset & Whitelist Engineering
* Source Data: Multi-season performance datasets (dati_mancini_multicampionato.csv) featuring club and international appearances.
* The Whitelist: A rigorous perimeter of 68 historical players coached by Roberto Mancini throughout his career (including top club stars and legends like Zlatan Ibrahimović).
* Data Wrangling:
   * Cleaned complex multi-index headers.
   * Handled missing values and standardized numerical metrics.
   * Reliability Filter: Imposed a minimum threshold of 800 total minutes under management to filter out short loans, anomalies, or short-term injuries, preserving true field variance.
📈 Methodology & Performance Rating Model
A synthetic normalized performance rating scale (5.0 to 10.0) was engineered, built on three pillars:
1. Base Score: Standard sufficiency baseline () with playing time validation.
2. Continuity Bonus: Ratio of actual minutes played against seasonal benchmarks (2,200 mins for club, 720 mins for national team).
3. Impact Bonus: Weighted offensive and defensive productivity incorporating Goals, Assists, Expected Goals (), and Expected Assists () tailored by field position (Forwards, Midfielders, Defenders/Goalkeepers).
🔍 Key Insights & Findings
   * The "Plot Twist" (Intellectual Honesty): Initial Exploratory Data Analysis (EDA) revealed that coaching impact is not a magical, automatic constant. Growth features natural individual variance. True data science avoids forcing narratives; the model respects the objective reality of the data.
   * Top Beneficiaries: Identified players who experienced the highest performance boost (Rating Delta) under tactical structuring.
🔮 Italy 2030 Predictive Simulation
   * Squad Construction: Evaluated projected profiles for the 2030 Italian talent pool across all departments (Goalkeepers, Defenders, Midfielders, Forwards).
   * Tactical Selection: Applied a strict 4-3-3 formation constraint to isolate the Top 11 starting lineup.
   * The Benchmark: Evaluated squad averages against the 7.10 UEFA Competitiveness Threshold.
📊 Visualizations & Charts
The pipeline automatically generates 5 professional Seaborn/Matplotlib charts saved directly to the root directory:
   1. valorizzazione_ruoli_mancini.png — Role-based performance growth comparison (Pre-Coach vs. Under Coach).
   2. top10_delta_giocatori.png — Horizontal bar chart of the Top 10 players with the highest performance boost.
   3. coaching_growth_scatter.png — Scatter plot analyzing initial player level against coaching improvement delta.
   4. department_scores_2030.png — Projected average score by department for the 2030 squad.
   5. proiezione_italia_2030_benchmark.png — Full Squad and Starting 11 benchmark against the 2030 World Cup qualification threshold.
🚀 Project Structure & Usage
Prerequisites
Make sure you have Python installed along with the required data science libraries:
Bash
   * pip install pandas numpy matplotlib seaborn


Running the Script
Ensure dati_mancini_multicampionato.csv is in your working directory, then execute the main script:
Bash
   * python mancini_analysis.py


🏁 Conclusion & Verdict
   * Does Mancini work miracles? The data shows a structured tactical lift, but individual growth depends heavily on baseline talent and context.
   * Will Italy make it to the 2030 World Cup? YES!
   * The Grand Finale: The starting XI average comfortably clears the UEFA threshold (7.10). However, the data proves that Italy qualifies thanks to the intrinsic generational talent, depth, and sheer quality of its players, rather than a magical managerial effect.
Italian football fans can finally sleep soundly! 🇮🇹⚽
👤 Author
   * Simonpietro (Pietro) Guido
   *