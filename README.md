# Student-Performance-Prediction-
A web-based application developed using Streamlit and Machine Learning to predict student performance based on academic and socio-demographic features. The app supports both classification (Pass/Fail) and regression (score prediction) using a Random Forest model, and includes interactive data visualizations to provide insights into the dataset.

## Features

* Predicts whether a student will **Pass** or **Fail**
* Estimates the **exam score**
* Utilizes **Random Forest** for classification and regression
* Offers interactive **visualizations** including heatmaps, bar charts, and scatter plots
* Accepts **custom user input** for real-time prediction
* Displays **GIFs** based on prediction results (Pass or Fail)
* Uses a cleaned and preprocessed combined dataset with relevant features

---

## Tech Stack

| Tool                 | Purpose                        |
| -------------------- | ------------------------------ |
| Python               | Core programming language      |
| Streamlit            | Web application interface      |
| Pandas               | Data manipulation and handling |
| NumPy                | Numerical computations         |
| Seaborn & Matplotlib | Data visualization             |
| Scikit-learn         | Machine learning models        |

---

## Dataset

Two datasets were merged and preprocessed:

1. **UCI Student Performance Dataset**

   * Source: [UCI Repository](https://archive.ics.uci.edu/ml/datasets/Student+Performance)
   * Features: demographics, academics, lifestyle (33 attributes)

2. **Kaggle Student Performance Dataset**

   * Source: [Kaggle](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)
   * Features: exam scores (math, reading, writing), and demographic information

The final dataset used for model training and prediction is named `StudentPerformanceFactors.csv`.

---

## Installation

To run the application locally:

```bash
git clone https://github.com/your-username/student-performance-prediction.git
cd student-performance-prediction
pip install -r requirements.txt
streamlit run app.py
```

---

## File Structure

```
├── app.py                         # Main Streamlit application
├── StudentPerformanceFactors.csv  # Dataset used for model training and prediction
├── style.css                      # Custom styles for the Streamlit app
├── image_home.jpeg                # Image used on the home screen
├── pass.gif                       # GIF displayed when prediction is 'Pass'
├── fail.gif                       # GIF displayed when prediction is 'Fail'
├── requirements.txt               # List of Python dependencies
```

---

## Models Used

| Task           | Model                  | Metric   | Performance |
| -------------- | ---------------------- | -------- | ----------- |
| Classification | RandomForestClassifier | Accuracy | \~87%       |
| Regression     | RandomForestRegressor  | RMSE     | \~1.75      |

---

## Team

Developed as a Mini Project for the **Bachelor of Engineering in Artificial Intelligence & Machine Learning**
**Canara Engineering College**

* Reeshal Dsouza (4CB23AI079)
* Sanjana Mahale (4CB23AI087)
* Vrinda Bhaskar Kumtakar (4CB23AI125)

**Guided by:**
Mr. Arjun K
Assistant Professor, Department of AIML

---

## Future Work

* Deploy the application on cloud platforms (e.g., Streamlit Cloud, Heroku)
* Integrate real-time prediction APIs
* Include psychological and behavioral indicators
* Improve accuracy using advanced ensemble models
* Develop a mobile-responsive interface
