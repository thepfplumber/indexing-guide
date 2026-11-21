# Indexing Guide

Companion code for [The Portfolio Plumber](https://thepfplumber.substack.com), a Substack about how to design indices from first principles.

Each notebook goes with an article. Read the article for the reasoning, and run the notebook to reproduce the results and adapt them to your own index.

## Notebooks

| # | Notebook | Article |
|---|---|---|
| 1.1 | [1.1 Starting Universe](https://github.com/thepfplumber/indexing-guide/blob/main/1.1%20Starting%20Universe.ipynb) | [The Anatomy of a Starting Universe](https://thepfplumber.substack.com/p/11-the-anatomy-of-a-starting-universe) |

Notebooks are numbered to match the articles and build on one another. Later notebooks may use outputs from earlier ones, so run them in order.

## Principles

* **Public data only.** Everything comes from free public sources. No paid data or subscriptions.
* **Rolling 10-year backtests.** By default, backtests cover the 10 years up to the run date. A notebook says so when it differs.
* **Runs anywhere.** Plain Python in any Jupyter environment. No cloud platform or proprietary tools required.
* **Transparent limits.** Each notebook ends with a "Known limitations" section.

## Getting started

1. Clone the repo and move into it.
2. Create a Python 3.9+ environment and install the packages listed in the notebook's opening cell.
3. Open the notebook and read its **Configuration** cell before running. Some data sources ask you to identify yourself, for example SEC EDGAR requires a contact email. Notebooks stop with a clear message until required settings are filled in.
4. Run all cells.

## Data and outputs

Notebooks write caches and outputs to a local `data/` folder relative to where you run them. You can change this in each notebook's Configuration cell. The `data/` folder is not tracked in Git, so data never ends up in the repo.

When a notebook calls a public API, it stays within that provider's published rate limits. Please keep it that way if you change the code.

## Contributing

Found a bug or a data issue? Open an issue. Mention the notebook number and, where relevant, the run date, since results depend on when the data was pulled.

## Disclaimer

This code is for education. It is not investment advice, and the results are not a recommendation to buy or sell any security. Data comes as-is from public sources and may contain errors.

## License
GNU General Public License v3.0
