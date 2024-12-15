# Central Government Welfare Schemes Analysis

## Project Overview
This project analyzes the design, implementation, and impact of various central government welfare schemes across India’s six administrative zones. The study evaluates proportional resource allocation and highlights regional disparities using **data-driven approaches** like linear regression and dimensionality reduction techniques.

---

## Table of Contents
- [Datasets](#datasets)
- [Key Analysis Steps](#key-analysis-steps)
- [Files and Notebooks](#files-and-notebooks)
- [Methods Used](#methods-used)
- [Results](#results)
- [Future Work](#future-work)

---

## Datasets
The datasets used for this analysis are sourced from the [Open Government Data (OGD) Platform](https://www.data.gov.in/). The schemes analyzed include:
1. **[PMGSY](https://www.data.gov.in/resource/physical-financial-progress-pradhan-mantri-gram-sadak-yojna-pmgsy-date)** - Pradhan Mantri Gram Sadak Yojana  
2. **[IGNWPS](https://www.data.gov.in/resource/indira-gandhi-widow-pension-scheme-ignwps-beneficiaries-abstract-during-fy-2023-24)** - Indira Gandhi Widow Pension Scheme  
3. **[IGNDPS](https://www.data.gov.in/resource/indira-gandhi-national-disability-pension-scheme-igndps-beneficiaries-abstract-during-fy)** - Indira Gandhi National Disability Pension Scheme  
4. **[IGNOAPS](https://www.data.gov.in/resource/indira-gandhi-national-old-aged-pension-scheme-ignoaps-beneficiaries-abstract-during-fy)** - Indira Gandhi National Old Aged Pension Scheme  
5. **[BharatNet](https://www.data.gov.in/resource/district-wise-service-ready-gram-panchayat-31-03-2024)** - Service Ready Gram Panchayat  
6. **[TB Laboratory Infrastructure, 2022](https://www.data.gov.in/resource/tb-laboratory-infrastructure-2022)** - Tuberculosis laboratory infrastructure  
---

## Key Analysis Steps
1. **Hypothesis Testing**: Test proportional allocation of funds using **linear regression models**.
2. **Preprocessing**: Handle missing values, state name inconsistencies, and transform data to zone-wise format.
3. **Scaling Technique**: Use the **Johnson-Lindenstrauss (JL)** method for dimensionality reduction while preserving accuracy.
4. **Model Training**: Train models on actual and reduced datasets to compare performance.
5. **Time Complexity**: Evaluate efficiency gains using the JL scaling technique.

---

## Files and Notebooks

| Notebook Name              | Description                                        |
|----------------------------|----------------------------------------------------|
| `PMGSY.ipynb`              | Analysis of PMGSY scheme performance and funds.   |
| `IGNWPS.ipynb`             | Analysis of Indira Gandhi Widow Pension Scheme.   |
| `IGNDPS.ipynb`             | Analysis of National Disability Pension Scheme.   |
| `IGNOAPS.ipynb`            | Analysis of National Old Aged Pension Scheme.     |
| `BharatNet.ipynb`          | Analysis of BharatNet implementation.             |
| `TBLab_Infra.ipynb`        | Analysis of TB Laboratory Infrastructure dataset. |
| `Scaling_ML.ipynb`         | Dimensionality reduction and model scaling.       |

---

## Methods Used
- **Linear Regression**: To test the linearity of fund allocation with features like road length and sanctioned projects.
- **Johnson-Lindenstrauss (JL) Scaling**: Reducing data dimensionality while preserving model performance.
- **Z-Test for Proportions**: Hypothesis testing to identify regional disparities.
- **Time Complexity Analysis**: Comparison of computational efficiency for original and reduced datasets.

---

## Results
- Linear regression achieved **85\%+ accuracy** in explaining the variance of sanctioned costs.
- The **JL scaling technique** reduced rows significantly (to 175) while maintaining comparable performance (Train R² = 0.891, Test R² = 0.885).
- **Regional disparities** were observed despite proportional resource allocation efforts.

---

## Future Work
Future improvements include incorporating updated demographic indicators, such as population density and socio-economic metrics, and combining datasets at the district level for more granular analysis. This will provide deeper insights into regional disparities and enhance the assessment of welfare scheme performance.

---

## Dependencies
- Python 3.x
- Libraries: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, Jupyter Notebook

---
