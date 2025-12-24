<p align="center"><b>🎓 Placement Predictor</b></p>
A machine learning project that predicts student placement outcomes based on academic performance, skills, extracurricular activities, and aptitude scores. 
This analysis helps students understand their placement probability and identify key factors that influence campus recruitment success.

🎯 Overview
This project analyzes a dataset of 10,000 students to predict placement outcomes using machine learning. The model achieves 80.85% accuracy and helps 
identify critical factors that influence placement success.

Project Goals:
  - Perform comprehensive Exploratory Data Analysis 
  - Build and evaluate predictive models
  - Achieve >60% accuracy ( Achieved 80.85%)
  - Identify key factors influencing placements

📊 Dataset
  - Dataset Size: 10,000 students
  - Features: 12 columns
  - Target Variable: PlacementStatus (Placed/Not Placed)

Features Description:
| Feature                  | Type   | Description                                |
|--------------------------|--------|--------------------------------------------|
| StudentID                | int    | Unique identifier                          |
| CGPA                     | float  | Cumulative Grade Point Average (6.5 - 9.1) |
| Internships              | int    | Number of internships completed (0-2)      |
| Projects                 | int    | Number of projects completed (0-3)         |
| Workshops/Certifications | int    | Number of workshops/certifications (0-3)   |
| AptitudeTestScore        | int    | Score in aptitude test (60-90)             |
| SoftSkillsRating         | float  | Rating of soft skills (3.0 - 4.8)          |
| ExtracurricularActivities| binary | Participation in activities (Yes/No)       |
| PlacementTraining        | binary | Underwent placement training (Yes/No)      |
| SSC_Marks                | int    | 10th grade marks (55-90)                   |
| HSC_Marks                | int    | 12th grade marks (57-88)                   |
| PlacementStatus          | binary | Placed (1) / Not Placed (0)                |


Data Quality: No missing values detected 

📈 Exploratory Data Analysis
Visualizations Included:
  - Placement Distribution Pie Chart - Shows 42% placement rate
  - CGPA Distribution - Histogram comparing placed vs not placed students
  - Aptitude Score Analysis - Distribution across placement outcomes
  - Internship Impact - Bar chart showing placement rate by internship count
  - Projects Impact - Correlation between number of projects and placement
  - Extracurricular Activities - Comparative placement rates
  - Placement Training Effect - Impact analysis

Statistical Insights:
  - Average CGPA: Placed (8.02) vs Not Placed (7.47)
  - Average Aptitude Score: Placed (84.46) vs Not Placed (75.83)
  - Placement Training Impact: 51.6% (with training) vs 15.6% (without)
  - Extracurricular Impact: 62.0% (with activities) vs 13.7% (without)

🛠️ Technologies Used
Programming & Libraries:
  - Python
  - NumPy - Numerical computations
  - Pandas - Data manipulation and analysis
  - Matplotlib & Seaborn - Data visualization
  - Scikit-learn - Machine learning models and evaluation

Machine Learning Algorithms:
  - Logistic Regression (Best Performance)
  - Decision Tree Classifier
  - Random Forest Classifier

Preprocessing Techniques:
  - Feature scaling using StandardScaler
  - Binary encoding for categorical variables
  - Train-test split (80-20 ratio)
  - Stratified sampling for class balance

📊 Model Performance
Comparison Table
| Model                 | Accuracy | ROC-AUC | CV Score (Mean ± Std) |
|-----------------------|----------|---------|-----------------------|
| Logistic Regression   | 80.85%   | 0.8837  | 79.67% ± 0.76%        |
| Random Forest         | 79.95%   | 0.8812  | 79.55% ± 0.70%        |
| Decision Tree         | 78.05%   | 0.8581  | 77.77% ± 1.06%        |
Best Model: Logistic Regression with 80.85% accuracy

🔍 Key Insights
Critical Success Factors:
 - CGPA is the Strongest Predictor
   Placed students: Average CGPA 8.02
   Not placed students: Average CGPA 7.47
   Impact: 0.55 point difference

  - Aptitude Scores Matter Significantly
   Placed students: Average score 84.46
   Not placed students: Average score 75.83
   Impact: 8.63 point difference


  - Placement Training is Crucial
   With training: 51.6% placement rate
   Without training: 15.6% placement rate
   Impact: 36% improvement (231% increase)


  - Extracurricular Activities Show Strong Correlation
   With activities: 62.0% placement rate
   Without activities: 13.7% placement rate
   Impact: 48.3% improvement (352% increase)


  - Internships and Projects Boost Chances
    More internships → higher placement rates
    More projects → better outcomes

📁 Project Structure
``
placement_predictor/
│
├── placement.ipynb           # Main Jupyter notebook with complete analysis
├── placement_data.csv        # Dataset (10,000 students)
├── README.md                 # Project documentation
└── requirements.txt          # Python dependencies
``

📌 Project Highlights
    80.85% Accuracy - Exceeds 60% requirement
    10,000 Students - Large, comprehensive dataset
    3 ML Algorithms - Comparative analysis
    Comprehensive EDA - 7+ visualizations
    Actionable Insights - Clear recommendations
    Production-Ready - Clean, documented code
