# Experiment-18
## Aim of Experiment: 
Exploring Statistical and Specialized Data Visualization
## Theory:
## Libraries Used
- `matplotlib.pyplot` — Core plotting engine for all static charts and figures
- `seaborn` — Statistical visualization library used for boxplot, heatmap, and styled scatter plots
- `pandas` — DataFrame creation and column-based data manipulation
- `numpy` — Numerical operations, random data generation, and seed control
## Plots / Visualizations
- **Area Plot (Simple)** — Fills area under the Values curve by Category using `plt.fill_between()` with green color and 0.25 alpha transparency
- **Area Plot (Overlapping)** — Overlays Sales (skyblue) and Profit (orange) filled areas on the same axes with a legend, styled using `sns.set_style("whitegrid")`
- **Pie Chart** — Shows percentage share of Values across Categories A–E using `plt.pie()` with `autopct='%1.2f%%'`
- **Donut Chart** — Same as pie chart but with a white circle (`plt.Circle` with radius 0.70) overlaid at center to create the donut hole effect
- **Boxplot** — Detects spread and outliers in the Values column using `sns.boxplot()`
- **Heatmap (2-variable)** — Displays correlation between Sales and Profit using `sns.heatmap()` with `annot=True` and `cmap='coolwarm'`
- **Heatmap (3-variable)** — Extended correlation heatmap including Values, Sales, and Profit with default colormap
- **Bubble Plot (Simple)** — 3-variable scatter using `plt.scatter()` where bubble size = `Values * 10`, X = Sales, Y = Profit
- **Bubble Plot (Seaborn)** — Enhanced bubble plot using `sns.scatterplot()` with `size` and `hue` both mapped to Values and `palette='viridis'`
## Functions Used
- `np.random.seed(0)` — Sets random seed for reproducibility of generated data
- `np.random.randint(low, high, size)` — Generates random integers for Sales and Profit columns
- `pd.DataFrame()` — Creates the main DataFrame with Category, Values, Sales, and Profit columns
- `plt.figure()` / `plt.figure(figsize)` — Initializes a new figure with optional size
- `plt.fill_between(x, y, color, alpha, label)` — Fills the area between x-axis and y values to create area plots
- `plt.pie(values, labels, autopct)` — Draws a pie chart with percentage labels
- `plt.Circle((0,0), radius, fc)` — Creates a white circle artist used to hollow out the donut chart
- `plt.gcf()` — Gets the current figure object
- `fig.gca().add_artist()` — Adds the centre circle artist to the current axes for the donut chart
- `sns.set_style("whitegrid")` — Applies seaborn's whitegrid theme to the plot background
- `sns.boxplot(x)` — Draws a horizontal box plot to show distribution and outliers
- `df[cols].corr()` — Computes pairwise Pearson correlation matrix between selected columns
- `sns.heatmap(corr, annot, cmap)` — Renders the correlation matrix as a color-coded heatmap
- `plt.scatter(x, y, s)` — Draws a bubble plot where `s` controls bubble size
- `sns.scat
## Conclusion: 
Demonstrates exploratory data analysis and visualization using Python libraries like pandas, matplotlib, and seaborn.  
