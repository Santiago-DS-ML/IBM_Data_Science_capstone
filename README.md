SpaceX Falcon 9 First Stage Landing Prediction
🚀 Project Overview
The goal of this project is to predict whether the first stage of the Falcon 9 rocket will land successfully. SpaceX reduces launch costs by reusing the first stage; by predicting the landing outcome, we can estimate the cost of a launch and help other companies compete with SpaceX.

📊 Key Findings
Model Performance: The best-performing model was the Decision Tree (and KNN), achieving an accuracy of 83.33% on the test set.

Success Drivers: Success rates have improved significantly over time, with specific orbits (ES-L1, GEO, HEO, SSO) showing the highest reliability.

Operational Insight: Launch site KSC LC-39A has the highest success ratio among all sites.

🛠️ Data Science Pipeline
1. Data Collection & Wrangling
API Extraction: Retrieved data from the SpaceX REST API.

Web Scraping: Extracted Falcon 9 launch records from Wikipedia using BeautifulSoup.

Cleaning: Handled missing values and performed One-Hot Encoding on categorical features (Orbit, Launch Site, etc.).

2. Exploratory Data Analysis (EDA)
SQL: Used SQL to query landing outcomes, payload totals, and mission counts.

Visualization: Created scatter plots and bar charts using Matplotlib and Seaborn to identify trends in flight numbers and payload mass.

3. Interactive Analytics
Geospatial Mapping: Built an interactive map using Folium to visualize launch site proximities to coastlines and infrastructure.

Dashboard: Developed a Plotly Dash application to filter success rates by payload and site.

4. Machine Learning
Trained and tuned four classification models: Logistic Regression, SVM, Decision Tree, and KNN.

Used GridSearchCV for hyperparameter optimization.
