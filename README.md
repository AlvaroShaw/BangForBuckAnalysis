# Valuing actions and estimating probabilities
Evaluating market value of Ligue 1 players using VAEP, webpage: https://alvaroshaw.github.io/BangForBuckAnalysis-VAEP-/

## Skills & Tools

**Data Collection & Engineering**

* **Python** — primary environment for pipeline construction, large-scale data manipulation, and web scraping.
* **SPADL Parsing** — utilizing the **Friends of Tracking** (`socceraction`) framework to convert massive, complex Wyscout stream-event data into standardized Soccer Player Action Description Language format.
* **Big Data Handling** — processing a massive event dataset consisting of 1,941 matches, 3,251,294 unique on-ball events, and 4,299 players.


* **Web Scraping** — writing automated scripts to scrape player market values from Transfermarkt to evaluate financial and recruitment efficiency.


* **Feature Engineering** — structuring raw data into contextual real-valued features and rolling event horizons (capturing the 3 previous match actions to define the current game state).



**Machine Learning & Statistical Modelling**

* **XGBoost (Extreme Gradient Boosting)** — training an advanced tree-based ensemble classifier to predict multi-class probabilities.


* **Probabilistic Classification** — training dual machine learning models to simultaneously calculate the changing probabilities of scoring ($P_{scores}$) and conceding ($P_{concedes}$) for any given on-ball action.


* **VAEP Framework Application** — aggregating offensive and defensive action values to evaluate a player's total net contribution (rating between -1.0 and +1.0) to a team's success.



**Visualisation & Web Development**

* **Flourish BI Integration** — designing complex, interactive scatter plots, trade-off charts, and horizontal bar visualisations embedded via clean HTML wrappers.


* **Action Quality vs. Quantity Trade-off Matrix** — plotting average action count against average action value to accurately isolate efficiency and filter out sample-size noise.


* **HTML / CSS / JavaScript** — architecting a responsive, modular portfolio layout to house analysis reports.


* **Intersection Observer API** — implementing scroll-triggered layout transitions and smooth visual tracking.



**Research & Tactical Analysis**

* **Transfer Market Efficiency** — identifying undervalued tactical outliers (e.g., Javier Pastore at PSG) by cross-referencing objective VAEP ratings against crowdsourced transfer data.


* **Positional Capability & Profiling** — decomposing player ratings per-90 into action-specific values (e.g., separating dribble value vs. pass value) to run targeted player replacement studies (e.g., evaluating replacements for Cristiano Ronaldo).


* **Model Benchmarking** — evaluating the variance, robustness, and stability of a possession-based framework (xT) against a context-rich game-state framework (VAEP) across a full season.
