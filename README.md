# **Is Bat Speed King? – Analyzing MLB's 2024 Bat Tracking Data**

## **Project Overview**
This project explores **Statcast's 2024 Bat Tracking Data** to analyze the **trade-offs between bat speed, swing length, and hitting effectiveness**. The study investigates whether **higher bat speed leads to better run production** while increasing whiff rates and whether swing length influences blast rate per contact.

## **Key Questions**
- Does **higher bat speed** correlate with **better run production (wOBA, blast rate) at the cost of more whiffs?**
- What distinguishes **above-average vs. below-average hitters** in terms of bat speed, swing mechanics, and squared-up contact?
- How does **swing length relate to contact quality (Blast Rate per Contact)?**
  
## **Data Sources**
The analysis integrates three datasets:
1. **Bat Tracking Data (`mlb_bat_tracking.csv`)** – Contains batter-specific metrics such as swing length, bat speed, and squared-up contact rates.
2. **Expected Stats (`expected_stats.csv`)** – Includes wOBA, batter run value, and other performance indicators.
3. **Home Run Data (`homeruns.csv`)** – Provides information on each player's home runs to validate power-hitting trends.

## **Key Findings**
1. **Better hitters have faster swings but also higher whiff rates**  
   - Scatter plot analysis shows a positive correlation between **bat speed and wOBA**, but with **increased swing-and-miss tendencies**.
   
2. **Squared-up contact and blast rate separate elite hitters from average ones**  
   - Density plots highlight that above-average hitters tend to square up the ball more efficiently.

3. **Longer swings lead to more explosive contact**  
   - Violin plot analysis shows **blast rate per contact increases** with **longer swing lengths**, suggesting a trade-off between **power and control**.

## **Visualizations**
The analysis is presented through three key plots:
1. **Facetted Density Plot** – Compares distributions of bat speed, swing length, and squared-up contact between **above-average vs. below-average hitters**.
2. **Scatter Plot (Bat Speed vs. Whiff Rate, colored by wOBA)** – Highlights the **trade-off between power and swing efficiency**.
3. **Violin Plot (Swing Length vs. Blast Rate per Contact)** – Shows **how swing length influences hard contact rates**.

## **Technologies Used**
- **Programming**: R (`tidyverse`, `patchwork`, `ggtext`)
- **Data Visualization**: Custom **MLB-style color themes** for interpretability
- **Statistical Analysis**: Distribution comparisons, scatter analysis, categorical binning

## **Reproducibility**
To reproduce this analysis:
1. Clone this repository.
2. Install required R packages:  
   ```r
   install.packages(c("tidyverse", "ggtext", "patchwork"))