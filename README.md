smart irrigation system 
edunet foundation AICTE Shell virtual internship
An AI-powered irrigation system that predicts ON/OFF states for 19 sprinkler zones based on real-time environmental sensor data — built using Python, Scikit-learn, and Streamlit.

 Project Overview

This project aims to automate irrigation decisions using a machine learning model trained on sensor data. It predicts which of the 19 zones should be watered and triggers the relevant pumps, optimizing water usage and reducing manual intervention.

-  Input: Scaled values (0–1) from 19 environmental sensors
-  Output: ON/OFF prediction for each sprinkler
-  Goal: Efficient, data-driven irrigation using AI
 Methodology

1. **Data Simulation & Preprocessing**
   - Simulated environmental sensor readings across 19 farm parcels.
   - Normalized values and prepared labeled data for model training.

2. **Model Training**
   - Used `RandomForestClassifier` with `MultiOutputClassifier` to predict sprinkler status across zones.
   - Trained and evaluated using scikit-learn.

3. **Model Serialization**
   - Final model saved using `joblib` for easy deployment.

4. **App Interface**
   - Built an interactive web app using **Streamlit**.
   - Accepts sensor values as input sliders and displays sprinkler status predictions.

## 🛠 Tech Stack

| Category          | Tools & Frameworks                      |
|------------------|------------------------------------------|
| Language          | Python                                   |
| ML Libraries      | Scikit-learn, NumPy, Joblib              |
| UI & Deployment   | Streamlit, Pyngrok (for Colab hosting)   |
| Dev Environment   | Google Colab, VS Code                    |



 How to Run the App

 Option 1: Locally
```bash
git clone https://github.com/your-username/smart-sprinkler-system.git
cd smart-sprinkler-system
pip install -r requirements.txt
streamlit run app.py
