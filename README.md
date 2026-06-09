# corporate-credit-portfolio-analytics
Python-based credit portfolio analytics framework including PD/LGD/EAD modeling, stress testing, Economic Capital and RAROC analysis.

# Corporate Credit Portfolio Analytics & Economic Capital Modeling

## Project Overview

This project simulates how financial institutions assess, monitor, and manage corporate credit portfolios. The objective was to develop an end-to-end credit risk analytics framework capable of evaluating borrower credit quality, measuring portfolio risk concentrations, estimating capital requirements, and assessing risk-adjusted profitability.

The framework combines traditional commercial banking credit analysis with portfolio risk management methodologies commonly used by credit risk, portfolio analytics, treasury risk, and capital management teams.

---

## Business Objective

The project was designed to answer several key portfolio management questions:

- How much credit risk exists within the portfolio?
- Which sectors contribute most to portfolio risk?
- How sensitive is the portfolio to economic stress?
- What level of capital is required to absorb unexpected losses?
- How does diversification affect portfolio risk and profitability?
- Does reducing concentration necessarily improve portfolio performance?

---

## Portfolio Construction

A diversified portfolio of corporate borrowers was constructed across multiple industries:

- Energy
- Industrials
- Transportation
- Utilities
- Consumer
- Technology
- Telecommunications
- Real Estate & Infrastructure

Each borrower was assigned:

- Exposure at Default (EAD)
- Probability of Default (PD)
- Loss Given Default (LGD)
- Internal Credit Rating
- Industry Classification

---

## Credit Risk Modeling

### Expected Loss (EL)

Expected Loss was calculated at both the borrower and portfolio levels using:

EL = PD × LGD × EAD

This metric estimates the average credit losses expected over time.

### Risk-Adjusted Return on Capital (RAROC)

RAROC was incorporated to evaluate whether portfolio returns adequately compensate for the risks assumed.

The analysis compared expected profitability against both regulatory and economic capital requirements.

---

## Portfolio Monitoring & Risk Assessment

### Sector Concentration Analysis

Portfolio exposures were aggregated by sector to identify concentration risks.

Key findings included elevated exposures to:

- Energy (23.4%)
- Transportation (15.5%)

These sectors represented the largest contributors to portfolio risk and became focal points for stress testing and optimization analysis.

### Credit Quality Analysis

Borrowers were segmented by internal rating category to evaluate:

- Portfolio credit quality
- Rating distribution
- Migration risk
- Concentration by rating bucket

### Single Name Exposure Analysis

Large borrower exposures were analyzed to identify concentration risks associated with individual counterparties.

---

## Rating Migration Analysis

A rating migration framework was developed to simulate changes in borrower credit quality over time.

Outputs included:

- Transition matrices
- Upgrade statistics
- Downgrade statistics
- Migration heatmaps

This analysis helps quantify deterioration and improvement in portfolio credit quality.

---

## Stress Testing

Multiple stress scenarios were implemented to evaluate portfolio resilience during adverse economic conditions.

Stress assumptions included:

- Higher default probabilities
- Increased loss severities
- Credit quality deterioration

The resulting stressed losses were compared against baseline portfolio losses to assess downside risk.

---

## Monte Carlo Simulation

A Monte Carlo framework was developed to simulate thousands of potential portfolio outcomes.

The simulation generated a portfolio loss distribution and quantified the likelihood of extreme loss events.

Outputs included:

- Portfolio Loss Distribution
- Tail Risk Analysis
- Scenario-Based Loss Estimation

---

## Value-at-Risk (VaR)

Value-at-Risk was estimated from the simulated portfolio loss distribution.

VaR measures the maximum expected loss at a specified confidence level under normal conditions.

---

## Expected Shortfall (ES)

Expected Shortfall was calculated to measure average losses beyond the VaR threshold.

Unlike VaR, Expected Shortfall captures the severity of extreme tail-loss events.

---

## Economic Capital

Economic Capital was estimated using Monte Carlo simulation outputs.

The objective was to determine the amount of capital required to absorb unexpected losses under adverse credit conditions.

Key outputs included:

- Expected Loss
- VaR
- Expected Shortfall
- Economic Capital

---

## Portfolio Optimization

Sector allocations were adjusted to evaluate whether diversification would improve portfolio performance.

The optimization analysis measured the impact on:

- Expected Loss
- Economic Capital
- VaR
- Expected Shortfall
- RAROC

### Key Finding

An important conclusion emerged from the analysis:

> Diversification alone does not necessarily reduce portfolio risk.

Although sector concentrations were reduced, the optimized portfolio exhibited higher Expected Loss, Economic Capital, and tail-risk metrics because capital was reallocated toward sectors containing borrowers with higher underlying credit risk.

This finding highlights the importance of balancing:

- Diversification
- Borrower quality
- Capital efficiency
- Risk-adjusted profitability

when managing corporate credit portfolios.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook

---

## Skills Demonstrated

### Credit Risk

- Credit Risk Assessment
- Probability of Default Modeling
- Loss Given Default Analysis
- Expected Loss Calculation
- Credit Portfolio Monitoring

### Portfolio Risk Management

- Concentration Risk Analysis
- Rating Migration Analysis
- Stress Testing
- Economic Capital Modeling
- RAROC Analysis

### Quantitative Analytics

- Monte Carlo Simulation
- Value-at-Risk (VaR)
- Expected Shortfall (ES)
- Portfolio Optimization
- Statistical Risk Modeling

---

## Project Outcome

The project successfully developed a corporate credit portfolio analytics framework capable of assessing borrower-level and portfolio-level credit risk.

The analysis demonstrated how concentration risk, borrower credit quality, economic capital, and risk-adjusted returns interact within a portfolio management context and provided practical insights similar to those used by commercial banks, export credit agencies, and institutional risk management teams.
