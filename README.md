# BDA600
OSHA Severe Injury Incidents: Predictive Modeling, Risk Scoring, and Data Visualization (2015–2025) - BDA600-01 Big Data Analytics Captsone
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Methods & Tools</title>
  <link rel="stylesheet" href="styles.css">
</head>

<body>
<header>
  <h1>Data Sources, Tools & Methodology</h1>
</header>

<nav>
  <a href="index.html">Home</a>
  <a href="methods.html">Methods</a>
  <a href="risk-model.html">Risk Score Model</a>
  <a href="visualizations.html">Visualizations</a>
  <a href="findings.html">Findings</a>
  <a href="downloads.html">Downloads</a>
</nav>

<section>
  <h2>Data Source</h2>
  <p>
    The OSHA Severe Injury dataset (2015–2022) contains thousands of employer-reported 
    records documenting amputations, hospitalizations, fractures, and other significant injuries. 
    Each record includes the event date, location, employer, injury type, and severity indicators.
  </p>

  <h2>Tools Used</h2>
  <h3>Tableau</h3>
  <p>
    Tableau was used for exploratory visualization and dashboard development. Its geospatial 
    features enabled mapping incident trends across states and cities, while interactive filters 
    provided insights into employer-level patterns, injury types, and seasonal behavior.
  </p>

  <h3>R Studio</h3>
  <p>
    R Studio supported data cleaning, statistical modeling, prediction, and risk score 
    construction. Using packages such as <i>dplyr</i>, <i>lubridate</i>, and <i>MASS</i>, the analysis 
    included Negative Binomial regression modeling, forecast generation, and risk score 
    computation with severity weighting, uncertainty adjustments, and temporal smoothing.
  </p>

  <h2>Methodological Workflow</h2>
  <ol>
    <li>Data Cleaning & Aggregation</li>
    <li>Exploratory Visualization</li>
    <li>Poisson & Negative Binomial Regression Modeling</li>
    <li>36-month Forecasting (2023–2025)</li>
    <li>Risk Score Development & Validation</li>
  </ol>
</section>

<footer>
  <p>© 2025 Jasmine Buckley-Williams</p>
</footer>

</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Risk Score Model</title>
  <link rel="stylesheet" href="styles.css">
</head>

<body>
<header>
  <h1>Risk Score Model (0–100)</h1>
</header>

<nav>
  <a href="index.html">Home</a>
  <a href="methods.html">Methods</a>
  <a href="risk-model.html">Risk Score Model</a>
  <a href="visualizations.html">Visualizations</a>
  <a href="findings.html">Findings</a>
  <a href="downloads.html">Downloads</a>
</nav>

<section>
  <h2>Model Overview</h2>
  <p>
    The risk score model converts predicted incident counts into a normalized, comparable 
    measure of workplace safety risk across states and months. The final score incorporates 
    workforce normalization, severity weighting, uncertainty adjustments, and temporal 
    smoothing, producing a robust and actionable 0–100 metric.
  </p>

  <h2>Risk Model Figure</h2>
  <img src="images/risk_model_figure.png" alt="Risk Model Diagram" class="full-img">

  <h2>Risk Model Matrix</h2>
  <p>Below is the operational matrix outlining meaning and recommended actions:</p>

  <table>
    <tr><th>Score</th><th>Level</th><th>Interpretation</th></tr>
    <tr><td>0–9</td><td>Very Low</td><td>Minimal expected incidents</td></tr>
    <tr><td>10–29</td><td>Low</td><td>Seasonal increases possible</td></tr>
    <tr><td>30–49</td><td>Moderate</td><td>Elevated risk vs baseline</td></tr>
    <tr><td>50–69</td><td>High</td><td>Clear elevated risk</td></tr>
    <tr><td>70–89</td><td>Very High</td><td>Systemic risk present</td></tr>
    <tr><td>90–100</td><td>Critical</td><td>Immediate attention required</td></tr>
  </table>

</section>

<footer>
  <p>© 2025 Jasmine Buckley-Williams</p>
</footer>

</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Visualizations</title>
  <link rel="stylesheet" href="styles.css">
</head>

<body>
<header>
  <h1>Data Visualizations</h1>
</header>

<nav>
  <a href="index.html">Home</a>
  <a href="methods.html">Methods</a>
  <a href="risk-model.html">Risk Score Model</a>
  <a href="visualizations.html">Visualizations</a>
  <a href="findings.html">Findings</a>
  <a href="downloads.html">Downloads</a>
</nav>

<section>
  <h2>Heatmap of Historical Incidents (2015–2022)</h2>
  <img src="images/heatmap.png" class="full-img">

  <h2>Top 10 Highest-Risk State-Months</h2>
  <img src="images/top10_table.png" class="full-img">

  <h2>Tableau Dashboards</h2>
  <p>Interactive dashboards include:</p>
  <ul>
    <li>State-by-state risk distributions</li>
    <li>Monthly trend analyses</li>
    <li>Employer-level breakdowns</li>
    <li>Injury type composition</li>
  </ul>
</section>

<footer>
  <p>© 2025 Jasmine Buckley-Williams</p>
</footer>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Key Findings</title>
  <link rel="stylesheet" href="styles.css">
</head>

<body>
<header>
  <h1>Key Findings & Interpretation</h1>
</header>

<nav>
  <a href="index.html">Home</a>
  <a href="methods.html">Methods</a>
  <a href="risk-model.html">Risk Score Model</a>
  <a href="visualizations.html">Visualizations</a>
  <a href="findings.html">Findings</a>
  <a href="downloads.html">Downloads</a>
</nav>

<section>
  <h2>Geographic Patterns</h2>
  <p>
    Texas, California, Florida, New York, and Illinois consistently experience the highest 
    concentrations of severe injuries, driven by industrial composition, population, and 
    seasonal labor patterns.
  </p>

  <h2>Temporal Trends</h2>
  <p>
    Summer months (May–August) exhibit predictable spikes due to increased construction 
    and outdoor labor. The COVID-19 period (2020) shows a notable dip and rebound.
  </p>

  <h2>Predictive Implications</h2>
  <p>
    The Negative Binomial model successfully anticipates future incident patterns. Employers 
    can use risk scores to schedule interventions, and regulators can prioritize inspections 
    based on forecasted risk levels.
  </p>

  <h2>Operational Guidance</h2>
  <p>
    Scores above 70 for two consecutive months prompt inspector deployment; scores above 
    50 trigger employer safety plan updates; insurers may apply surcharges or safety program 
    requirements for scores above 50.
  </p>
</section>

<footer>
  <p>© 2025 Jasmine Buckley-Williams</p>
</footer>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Downloads</title>
  <link rel="stylesheet" href="styles.css">
</head>

<body>
<header>
  <h1>Downloadable Files</h1>
</header>

<nav>
  <a href="index.html">Home</a>
  <a href="methods.html">Methods</a>
  <a href="risk-model.html">Risk Score Model</a>
  <a href="visualizations.html">Visualizations</a>
  <a href="findings.html">Findings</a>
  <a href="downloads.html">Downloads</a>
</nav>

<section>
  <h2>Available Resources</h2>
  <ul>
    <li><a href="report.pdf">Full Report (PDF)</a></li>
    <li><a href="data-cleaning-script.R">R Data Cleaning Script</a></li>
    <li><a href="risk-score-script.R">Risk Score Generation Script</a></li>
    <li><a href="forecasting-script.R">Forecasting Script</a></li>
    <li><a href="images/risk_model_figure.png">Risk Model Figure</a></li>
  </ul>
</section>

<footer>
  <p>© 2025 Jasmine Buckley-Williams</p>
</footer>
</body>
</html>

body {
  font-family: Arial, sans-serif;
  margin: 0;
  background: #f9f9f9;
  color: #333;
}

header {
  background: #003366;
  color: white;
  padding: 20px;
  text-align: center;
}

.subtitle {
  font-size: 18px;
  margin-top: -8px;
}

nav {
  background: #004080;
  padding: 10px;
  text-align: center;
}

nav a {
  color: white;
  margin: 0 15px;
  text-decoration: none;
  font-weight: bold;
}

nav a:hover {
  text-decoration: underline;
}

section {
  padding: 40px;
  max-width: 1100px;
  margin: auto;
  background: white;
}

h1, h2, h3 {
  color: #003366;
}

table {
  width: 100%;
  border-collapse: collapse;
  margin-top: 20px;
}

table th, table td {
  border: 1px solid #aaa;
  padding: 10px;
  text-align: center;
}

.full-img {
  width: 100%;
  margin: 20px 0;
  border: 1px solid #ccc;
}

footer {
  text-align: center;
  padding: 20px;
  background: #003366;
  color: white;
  margin-top: 50px;
}
