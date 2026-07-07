# FBI Crime Data — Human Trafficking Exploratory Analysis

## Table of Contents

- [Description](#description)
- [The Data](#the-data)
- [Analysis Approach](#analysis-approach)
- [Installation](#installation)
- [Usage](#usage)
- [Author](#author)

<hr style="border: none; height: 10px; background-color: #003057;" />

## Name

Exploratory Data Analysis of FBI Human Trafficking Data (2013–2021)

## Description

Human trafficking is a significant issue in the United States. This project examines a human trafficking dataset compiled from local, state, city, county, and federal law enforcement agencies, published through the __FBI Crime Data Explorer__, covering incidents from __2013 through 2021__.

The analysis is built as a single, fully documented Jupyter notebook organized into pages with a linked table of contents — covering data acquisition, a data dictionary, data type assessment, null value analysis, and exploratory visualizations.

**A note on reproducibility:** the notebook downloads the dataset directly from the FBI's public data repository at runtime, so anyone can run it end-to-end and replicate the results without needing to source the data separately.

This project has these files:
- `Crime-Study.ipynb` — the complete analysis notebook (88 cells), organized into linked pages
- `HT_2013-2021.csv` — the human trafficking dataset (also downloaded automatically by the notebook)
- `Data/` — supporting data files, including a Florida-specific extract
- `media/` — images used in the notebook

[Back to Top](#table-of-contents)

## The Data

The dataset comes from the [FBI Crime Data Explorer](https://cde.ucr.cjis.gov/) and includes fields such as:

- `DATA_YEAR` — the year the incident occurred
- `ORI` (Originating Agency Identifier) — identifies the reporting agency
- Agency details — the level of government (city, county, state, federal) and location of each reporting agency
- Offense and incident details for commercial sex acts and involuntary servitude

The notebook includes a full data dictionary explaining every column before any analysis begins — establishing a shared understanding of the data the way a professional analysis should.

[Back to Top](#table-of-contents)

## Analysis Approach

The notebook walks through the analysis in clearly labeled pages:

1. **Introduction** — the assignment context and why this dataset matters
2. **Explanation of Data** — full column-by-column data dictionary
3. **Importing Libraries and Reading in the Data** — reproducible download from the FBI's public S3 repository
4. **Preliminary Look at Data Types** — identifying numeric, categorical, and null values
5. **Exploratory Data Analysis** — value distributions, percentage breakdowns for every column, null value quantification, and visualizations

[Back to Top](#table-of-contents)

## Installation

Clone the repository:

```bash
git clone https://github.com/M-arcy/FBI-Crime-EDA.git
cd FBI-Crime-EDA
```

Install the required dependencies:

```bash
pip install pandas numpy matplotlib seaborn requests jupyter
```

[Back to Top](#table-of-contents)

## Usage

Open the analysis notebook:

```bash
jupyter notebook Crime-Study.ipynb
```

Run all cells in order. The notebook downloads the dataset directly from the FBI's public repository, so no manual data setup is needed.

## Support

For questions, open an issue on the [GitHub repository](https://github.com/M-arcy/FBI-Crime-EDA/issues) or reach out via [LinkedIn](https://www.linkedin.com/in/marcy-misner/).

## Author

Developed by __Marcy Misner__.

For more of my work: [GitHub](https://github.com/M-arcy) | [LinkedIn](https://www.linkedin.com/in/marcy-misner/)

## License

This project is licensed under the MIT License.

[Back to Top](#table-of-contents)
