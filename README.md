# Healthcare Claims Data Analysis Assignment

## Project Description
This project analyzes a sample of **prospective healthcare claims data** from **Stony Brook University Hospital** to identify billing patterns, provider activity, payer mix, and clinical complexity. Using relational claims data (HEADER, LINE, and CODE files), the analysis demonstrates how healthcare data analysts and health informaticians use claims data to support **revenue cycle management, compliance auditing, and operational decision-making**.  

The project applies **Python and pandas** to perform multi-table joins, aggregations, and visualizations that reflect real-world healthcare analytics workflows.


## Data Source Information
The dataset consists of three interconnected CSV files that together form a relational claims database:

- **HEADER file**  
  Contains one row per claim with high-level claim information, including providers, payers, service dates, and place of service.

- **LINE file**  
  Contains one row per billed service or procedure (HCPCS/CPT codes), including charges and units.

- **CODE file**  
  Contains diagnosis codes (ICD-10) associated with each claim.

The data represents **prospective claims from September 2023 through May 2024** and is provided for **educational purposes only**.


## How to Run the Notebook
1. Clone this repository:
   ```bash
   git clone <repository-url>
   ```
2. (Optional) Create and activate a Python virtual environment.
3. Install the required libraries listed below.
4. Place the CSV files in the data/ directory (Data files are excluded from GitHub using .gitignore.)
5. Open the notebook:
    ```
    jupyter notebook notebooks/claims_analysis.ipynb
    ```
6. Run all cells sequentially from top to bottom.


## Summary of Key Findings

* The dataset contains **388 unique claims**, with an average of **1.34 service lines** and **3.96 diagnosis codes per claim**, indicating mostly straightforward billing with moderate clinical complexity.

* **SB Internists** accounts for the highest claim volume, while **New York Spine** and **Brain Surgery** exhibits the highest case complexity, averaging **9.23 diagnosis codes per claim**.

* **Medicare** is the dominant payer by both claim volume and total charges, reflecting the hospital’s patient population.

* **Critical care services (HCPCS 99291)** are frequently associated with acute respiratory failure and neurological emergencies.

* Only **1.3% of claims** include five or more service lines, suggesting that highly complex billing scenarios are relatively rare but concentrated among specific specialties.


## Required Libraries

* pandas >= 1.3.0

* matplotlib >= 3.4.0

* seaborn >= 0.11.0

* numpy (dependency)




