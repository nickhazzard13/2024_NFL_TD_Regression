# Fantasy Football Touchdown Regression Analysis: 2024 Season Report  

**Tableau Dashboard Link:** [CLICK HERE](https://public.tableau.com/views/2024fantasybook-final/OFFICIALFINAL?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)  

---

## Introduction  
The purpose of this project was to identify touchdown regression candidates among wide receivers (WRs), tight ends (TEs), and running backs (RBs) during the 2024 NFL season. I restricted the dataset to players with at least 9 games played, ensuring stability in the sample.  

**Core Question:**  
*Which players are most likely to regress positively (increase scoring) or negatively (decline) based on touchdown performance relative to their underlying volume?*  

---

## Methodology  

### Expected Fantasy Points (EFP) Model  
- Built a linear regression ML model using volume and yardage features (rush attempts, targets, snaps, receiving/rushing yards).  
- Excluded touchdowns from the model to create a baseline “expected” scoring output derived only from usage.  
- Abandoned earlier hand-calculated league-average methods, which inflated weaker players and exaggerated outliers.  

### Relative Regression Risk (RRR)  
- Compared **actual fantasy points vs. expected fantasy points**.  
- Used this difference to generate a **Relative Regression Risk** score:  
  - **Negative regression candidates:** benefited disproportionately from touchdowns.  
  - **Positive regression candidates:** held back by a lack of touchdown production.  

---

## Visualization  
An interactive Tableau dashboard was created with separate tabs for RBs, WRs, and TEs, each featuring:  
- Actual vs. Expected Fantasy Points scatterplots.  
- Volume vs. Touchdown Rate graphs.  
- Relative Regression Risk rankings, highlighting likely regression candidates.  

---

## Results  

### Running Backs (RBs)  
- **Negative Regression Candidate:** *James Cook*  
  - Highest reliance on touchdown production relative to his usage.  
  - Ranked at the top of RRR, signaling significant downside risk.  
  - Without a major volume increase, repeating his 2024 production will be difficult.  

- **Positive Regression Candidate:** *Tony Pollard*  
  - 3rd lowest points from touchdowns despite elite workload.  
  - Already at his floor in touchdown scoring, leaving room for natural regression upward.  
  - With stable volume in 2025, Pollard projects to rebound significantly.  

---

### Wide Receivers (WRs)  
- **Negative Regression Candidate:** *Amon-Ra St. Brown*  
  - Ranked #1 in RRR, showing the largest deviation from expected scoring.  
  - Plays in a crowded offense with little chance of a meaningful volume increase.  
  - Since improvement would require an even higher TD rate, he is more likely to regress downward.  

- **Positive Regression Candidate:** *CeeDee Lamb*  
  - Posted the second-highest volume per game among WRs.  
  - Played much of the season without his starting QB, suppressing scoring efficiency.  
  - Ranked 8th in positive regression risk, with ample upside if touchdown production normalizes alongside QB stability.  

---

### Tight Ends (TEs)  
- **Negative Regression Candidate:** *Mark Andrews*  
  - Recorded the highest touchdown rate of all TEs.  
  - Further complicated by his TE teammate also posting the second-highest rate.  
  - It is highly unlikely both sustain this extreme level of efficiency, pointing to regression risk.  

- **Positive Regression Candidate:** *Jake Ferguson*  
  - Produced solid underlying usage while recording a 0% touchdown rate.  
  - With his QB returning healthy, he represents one of the clearest upward regression opportunities.  
  - Even modest red zone conversion would significantly raise his scoring output.  

---

## Conclusion  
This project highlights how touchdowns are volatile and regression-prone, making them a key area for forecasting changes in fantasy performance. By modeling expected points from usage and comparing them to actual results, I identified clear candidates for positive and negative touchdown regression heading into the 2025 season.  

**Key Findings:**  
- **RBs:** James Cook (negative), Tony Pollard (positive)  
- **WRs:** Amon-Ra St. Brown (negative), CeeDee Lamb (positive)  
- **TEs:** Mark Andrews (negative), Jake Ferguson (positive)  

The **Relative Regression Risk (RRR) framework** combined with Tableau visualization provides actionable, data-driven insights for fantasy managers preparing for drafts, ensuring a sharper understanding of which players are most likely to regress in touchdown production.  
