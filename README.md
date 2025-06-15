# Data Analysis on Drugs, Side Effects and Medical Conditions 

An end-to-end data science project built using Python and Tableau, leveraging real-world drug data scraped from Drugs.com. The project combines data cleaning, exploratory analysis, visualization, and interactive dashboards to uncover insights about drugs, side effects, usage conditions, user reviews, and safety classifications.

## 🧠 Objectives

- Develop an end-to-end data-driven application focused on drug information, side effects, and medical conditions.
- Clean and preprocess raw pharmaceutical data with inconsistent and missing values.
- Perform in-depth exploratory data analysis (EDA) to extract meaningful insights.
- Build interactive visualizations for dynamic data exploration using Python and Tableau.
- Create a user-friendly search tool to look up drugs or diseases with relevant details like side effects, brand names, safety data, and ratings.

## 🔧 Tools & Technologies

- Python (Pandas, NumPy, Matplotlib, Seaborn and Scikit-Learn)
- Tableau Public (for interactive dashboards): [ ] 
- Jupyter Notebook
- Git & GitHub (for version control)

## 📂 Dataset

- The dataset includes: Drug names (generic & brand), Medical conditions, Side effects, User ratings, Prescription status (Rx, OTC) etc. 
- Due to privacy and size limits, the full dataset is not included in this repo.

➡️ [Download dataset here] [https://www.kaggle.com/datasets/nailasrivastava/drugs-side-effects-and-medical-conditions ]

## 💻 How to Run
1. Clone the repo  
2. Install dependencies: `pip install -r requirements.txt`  
3. Open the notebook: `Drugs, side_effects_&_medical_conditions.ipynb`  
4. Run all cells and enjoy the visuals!

## 🧪 Functional Tool: Drug & Disease Lookup Tool (CLI-based)

- Created a command-line interface where users can input a drug name or medical condition
- The tool fetches detailed info like brand names, activity, side effects, rating, and links
- Clean error-handling for unfound queries with a friendly "Error 404. Not Found!" message
- Fully extensible- can be integrated into future UI dashboards or apps

💡 This feature makes the dataset not just explorable but interactive. Think of it like a mini drug search engine.

## 📊 Key Analysis

* Cleaned and filtered data with inconsistent numeric/categorical values
* Counted and ranked conditions by the number of associated drugs
* Identified most-reviewed drugs and their user ratings
* Analyzed safety across pregnancy and alcohol interaction categories
* Assessed Controlled Substance (CSA) classifications
* Mapped drug classes to usage patterns

## 📈 Sample Visualizations

* Bar plots showing most-reviewed drugs and most common conditions
* Pie chart or donut chart for Rx vs OTC distribution
* Box plot of user ratings across pregnancy categories
* Scatter plot comparing number of reviews vs average ratings

## 🌍 Advanced Visuals

* Word Cloud of most frequent side effects per condition or drug class
* Tableau Dashboard for interactive filtering by drug, class, condition, or side effects

## 📝 Key Takeaways

* Certain drug classes dominate treatment for multiple high-risk conditions
* Most commonly reported side effects cluster around a few recurring symptoms
* Many drugs have concerning pregnancy categories (C/D/X), yet are frequently reviewed
* Alcohol interaction warning (X) appears in several commonly used drugs
* OTC drugs generally receive higher ratings than strict Rx-only drugs
* Some conditions like Acne and Depression have a large pool of drug options, while others like Cancer are more limited
* The CLI Lookup Tool enhances dataset usability and educational value

## 🧩 What’s Next?

- Add advanced analytics like PCA, clustering, and heatmaps in the next version
- Build a Streamlit or Flask app version of the CLI tool for web-based interaction
- Add a layer of sentiment analysis using NLP from user reviews (if available later)
- Integrate external APIs for real-time drug data comparison

## 🙌 Acknowledgments

Huge thanks to the open-source community and dataset contributors. 
This project was done as part of a 12-week upskilling sprint (Data Analyst Internship).

Massive thanks to:
* **Drugs.com** – for making the raw data accessible
* Project inspired by real-world pharmacovigilance, bioinformatics, and healthcare analytics needs

## 📂 Project Structure

```plaintext
Drugs_Side-Effects_Conditions_Analysis/
│
│── drugs_side_effects.csv                                         # Raw dataset from Drugs.com
│── drugs_cleaned_dataset.csv                                      # Cleaned and preprocessed dataset
│
├── plots/                                                         # All charts and graphs
├── Tableau Dashboard                                              # Tableau workbook (.twbx file)
├── Tableau df script.ipynb                                        # Tableau dashboard notebook
├── Drugs, side_effects_&_medical_conditions.ipynb                 # Main analysis notebook
├── .gitignore
├── README.md
└── requirements.txt                                               # All required packages
