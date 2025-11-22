# Sell in May and Go Away

A simple, data-driven look at the well-known market saying.

## Table of Contents

* [Overview](#overview)
* [About the Article](#about-the-article)
* [What This Project Does](#what-this-project-does)
* [Repository Structure](#repository-structure)
* [How to Run the Code](#how-to-run-the-code)
* [Key Findings](#key-findings)
* [Usage Notes](#usage-notes)
* [License](#license)

## Overview

This repository contains Python code used to study the long-standing investment saying: **"Sell in May and go away."** The idea claims that stocks often perform better from **November to April** than they do from **May to October**. This project tests that idea using real market data.

## About the Article

This repo supports the Medium article titled **"Sell in May and Go Away — Does this old saying still apply today?"** by Joohi Rana, Om Rana, and Amish Prajapati.

The article explains the history behind the saying and uses data from popular market indexes and ETFs to see if the pattern still holds true. The results show that broad-market indexes continue to follow this pattern, while tech-focused funds show a weaker effect.

## What This Project Does

* Downloads historical price data for major stock indexes and ETFs
* Calculates returns for:

  * **May to October**
  * **November to April**
* Compares the two seasonal periods across many years
* Saves final results into CSV files for easy review
* Includes two versions of the analysis script

## Repository Structure

```
├── get_data.py                # Pulls historical market data
├── analysis.py                # Computes seasonal returns
├── SellMayGoAwayV2.py         # Improved version of the analysis
├── main.py                    # Runs the complete workflow
├── tickers.csv                # List of tickers analyzed
├── returns_NASDAQ.csv         # NASDAQ seasonal returns
├── returns_NYSE.csv           # NYSE seasonal returns
├── returns_S&P.csv            # S&P 500 seasonal returns
└── LICENSE                    # GPL-3.0 license
```

## How to Run the Code

1. Install Python (version 3.7 or higher recommended).
2. Install required packages:

   ```bash
   pip install -r requirements.txt
   ```
3. Download data:

   ```bash
   python get_data.py
   ```
4. Run the analysis:

   ```bash
   python main.py
   ```
5. Review the output CSV files to see seasonal performance results.

## Key Findings

* Broad market indexes (like the S&P 500) tend to perform better in the **November to April** period.
* Tech-focused ETFs, such as QQQ, show a weaker version of this pattern.
* Around **84 percent** of S&P 500 companies had stronger returns in the November–April period.
* The pattern is still visible today, but it does not apply to every sector or individual stock.

## Usage Notes

* This project is for educational and research purposes.
* The results are based on historical data and do not predict future performance.
* You can expand the analysis by adding more tickers, changing date ranges, or adding visualizations.

## License

This project is released under the GPL-3.0 License. See the `LICENSE` file for details.
