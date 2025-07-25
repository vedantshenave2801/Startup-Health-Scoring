# Startup Health Scoring Model 

### Overview
This is my submission for the ScaleDux AI Intern Task. The idea was to score and rank fictional startups based on various business factors like team experience, market size, traction, burn rate, funding, and valuation — kind of like a credit score system, but for startups.

---

### What I Did
- Cleaned and normalized the data using Min-Max scaling
- Inverted the burn rate since lower is better
- Assigned weights to each attribute based on what I felt mattered most
- Computed a final score out of 100
- Ranked all startups and picked the top 10 and bottom 10
- Added some simple visualizations to make the output easier to understand

---

### Feature Weights (My Logic)
- Team Experience – 15%  
- Market Size – 20%   
- Monthly Active Users – 25%  
- Burn Rate (Inverted) – 10%  
- Funds Raised – 15%  
- Valuation – 15%  

These weights are based on what I think investors would care about most when evaluating early-stage startups.

---

### Visualizations Included
- 📊 Bar chart of startup scores (sorted)
- 📈 Histogram of score distribution
- 🔥 Correlation heatmap of raw input features

All charts are saved in the `Outputs/` folder.

---

### ML Add-on (Optional Step)
I also added a simple **Linear Regression model** to predict startup valuation based on the input features.  
It helped me:
- Check which features affect valuation the most (via coefficients)
- Confirm that my scoring logic made sense (via R² score)

---

### Observations
- Startups with high valuation but poor traction or high burn often scored low — which felt fair.
- The top scorers had a good balance across users, team, funding, and market size.

---

### Tools Used
- Python  
- Pandas  
- Seaborn / Matplotlib  
- scikit-learn (for the regression model)  
- Jupyter Notebook

