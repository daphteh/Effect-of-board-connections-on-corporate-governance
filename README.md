# Effect of Board Connections between Corporations and Nonprofits on Corporate Governance
In this repo, I examined how board connections between corporations and nonprofit organizations influenced the occurrence of negative earnings restatements. 

### Methods Used ###
* Exploratory Data Analytics
* Statistics: Ordinary least squares regression with firm-level fixed effects and standard error clustering
* Data visualization (data and results)

### Tools ###
* Linear models
* Matplotlib
* Seaborn

The code here is useful for working with time series data and visualizing the effect of independent variables from different regressions on the dependent variable.

# The Data and Context

The data in this repo is proprietary and pertains to Fortune 500 firms from 1998 till 2014. The analysis is conducted on 12,436 observations and an average of 731 firms for each calendar year. 
<img width="1274" alt="Baseline Independent Variable" src="https://github.com/daphteh/Effect-of-board-connections-on-corporate-governance/blob/f40642525ee669dcc8630e4b0057abdc25451724/Reports/cnbi_over_time.png">

<details>
<summary> Data sources </summary>
<br>
<p> Boardex (board data) </p>
<p> Audit analytcis (earnings restatements and their characteristics) </p>
<p> Compustat (companies' financials) </p>
<p> Candid.org (US nonprofit organizations) </p>
</details>

<details>
<summary>  Variables </summary>
<br>
<p> The dependent variable: the number of negative non-accidental earnings restatements affecting a firm-year. </p>
<p> Independent variables: </p>
<p>- H1: the number of board connections a corporation has with nonprofits (CNBI) </p>
<p>- H2: CNBI with social welfare (SW) nonprofits </p>
<p>- H3: CNBI by the CEO </p>
<p>- H4: CNBI by the CEO with SW nonprofts </p>
<p>- H5: CNBI by the Chairman </p>

<p> Control variables: </p>
<p>- Natural log of total assets</p>
<p>- Book to market value </p>
<p>- Return on assets </p>
<p>- Leverage </p>
<p>- Number of board connections with other Fortune 500 corporations </p>
<p>- Board size </p>
<p>- Average age of board members </p>
<p>- If the CEO is also a the chairman (CEO-chair duality)  </p>
<p>- Size of the audit committee </p>
<p>- Number of independent directors </p>
<p>- Recidivism (the extent to which the firm engaged in potential deviance in the past) </p>
</details>

# Methodology

<details>
<summary> Step 0: Prepare the data </summary>
      <br>
      <p>   Combine the variables relevant for your analysis from different data sources</p>
      <p>   Explore the data to understand your context especially over time </p>
</details>

<details>   
<summary> Step 1: Conduct the analysis </summary>  
  <br>
  <p>   Assess the appropriate method for analysis</p>
  <p>   Fixed effects were included to account for endogenous firm level characteristics </p>
</details>

<details>
<summary> Step 2: Aggregate the coefficients in a separate data frame </summary>
</details>

<details>
<summary> Step 3: Visualize your coefficients </summary>
</details>


<img width="1274" alt="Effects on DV" src="https://github.com/daphteh/Effect-of-board-connections-on-corporate-governance/blob/ea8b06fcb4683f579923f1ae3461ac8fc7601e7b/Reports/coefficients_from_regression.png">
