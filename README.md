Personalization of Clinical Decisions Using Clustering
This project clusters heart patients based on vital signs and biomarkers to propose personalized clinical insights. The aim is to assist in clinical decision-making by identifying similar patient profiles using unsupervised learning (KMeans clustering).

🔬 Objective
To group patients based on medical parameters such as age, blood pressure, heart rate, blood sugar, CK-MB, and Troponin levels to derive personalized insights about their health and risk of heart attack.

💡 Novelty
While most heart-related ML studies focus on prediction, this project goes a step further to offer post-prediction recommendations based on cluster behavior—a rarely explored direction in clinical ML research.

📁 Dataset Description
The dataset includes the following 9 attributes:

Feature	Description
age	Age of the patient
gender	1 = Male, 0 = Female
heart_rate	Heartbeats per minute
systolic_blood_pressure	Pressure when the heart contracts
diastolic_blood_pressure	Pressure between heartbeats
blood_sugar	Blood glucose level
ck-mb	Cardiac enzyme released during muscle damage
troponin	Protein biomarker specific to heart injury
result	Target (1 = Positive for heart attack, 0 = Negative)

🧪 Steps Followed
Data Preprocessing

Handled missing values

Standardized features using StandardScaler

Clustering

Used KMeans with optimal cluster count (found using Silhouette Score)

Grouped patients into clusters

Cluster Analysis

Compared cluster centroids for clinical insight

Mapped average values of biomarkers and outcomes

Dashboard with Gradio

Built an interactive dashboard to explore clusters by inputting patient data

Displays cluster assignment and visual cluster profiles

📊 Technologies Used
Python (Pandas, NumPy, Matplotlib, Seaborn)

Scikit-learn (StandardScaler, KMeans, silhouette_score)

Gradio (for the interactive dashboard)

Google Colab (for development and experimentation)

🚀 How to Run
Open the notebook in Google Colab

Upload your dataset file (.csv)

Run the cells step-by-step to:

Preprocess and cluster the data

Train and save models

Launch the Gradio dashboard

🖥️ Dashboard Features
Input: Custom patient parameters

Output:

Cluster prediction

Visual analysis of cluster centers

📈 Sample Output
Optimal Clusters: 2 (based on Silhouette Score)

Cluster Insights:

Cluster 0: Lower average CK-MB and blood sugar (Lower risk)

Cluster 1: Elevated CK-MB and blood sugar levels (Higher risk)
