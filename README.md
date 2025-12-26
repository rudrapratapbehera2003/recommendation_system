Course Recommendation System:
An end-to-end machine learning project that provides personalized course suggestions based on user preferences. This system utilizes a Random Forest model for robust predictions and is deployed as an interactive web application using Streamlit.

Project Overview:
This project follows a systematic machine learning pipeline to recommend online courses. It explores various recommendation strategies, including Content-Based and Collaborative Filtering, before selecting a fine-tuned Random Forest ensemble for final deployment.

The Machine Learning Pipeline:
1. Problem Framing:-
The goal is to solve the "information overload" problem for students by providing a tool that suggests relevant courses based on their past behavior or course descriptions.

2. Exploratory Data Analysis (EDA):-
- Analyzed course distributions across categories and platforms.
- Visualized user ratings, course difficulty levels, and enrollment trends.
- Identified data sparsity and handled missing values or duplicates.

3. Model Implementation:-
We explored multiple recommendation approaches to find the most effective solution:
- Content-Based Filtering: Suggested courses similar to a specific item using Cosine Similarity.
- Collaborative Filtering: Predicted user interests by identifying patterns from similar users.
- Final Choice - Random Forest: Chosen for its high predictive accuracy, robustness to overfitting, and ability to handle non-linear relationships in complex datasets.

4. Deployment
The final Random Forest model was "pickled" and integrated into a Streamlit application for a real-time, interactive user experience.

Setup and Installation:
Note: Due to GitHub's file size limits, the pre-trained Random Forest model (model.pkl) is not included in this repository. You must generate it locally before running the application.

How to Run Locally:
1. Clone the repository:(use the following command)
git clone https://github.com/rudrapratapbehera2003/recommendation_system.git
cd recommendation_model_deployment

2. Install dependencies:
pip install -r requirements.txt

3. Run the application:
streamlit run app.py
