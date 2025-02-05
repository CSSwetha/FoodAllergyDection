# SafeBite: AI-Powered Allergen Detection in Food

**SafeBite** is an AI-powered application designed to help individuals with food allergies make informed decisions by identifying allergens in food products. By leveraging machine learning models, SafeBite provides real-time allergen detection, ensuring safer food choices and a better quality of life for people with food sensitivities.

## Vision

Our vision is to create an inclusive world where individuals with food allergies can confidently make safe food choices. Through AI-powered allergen detection, SafeBite aims to empower people with the tools they need to avoid allergens and live healthier, more secure lives.

## Mission

Our mission is to develop an intuitive, reliable, and efficient tool that allows users to identify potential allergens in food. By using advanced machine learning, SafeBite provides users with the ability to instantly detect allergens and make informed decisions.

## Features

- **Real-Time Allergen Detection**: Identify allergens in food products by analyzing ingredient data.
- **Instant Allergen Alerts**: Receive notifications when a food item contains allergens, such as nuts, dairy, or gluten.
- **User-Friendly Interface**: The app provides a clean, simple interface for easy interactions and quick allergen detection.
- **Customizable Allergen Preferences**: Users can personalize the app to detect allergens based on their specific needs.
- **Multi-Ingredient Detection**: SafeBite can process complex food items with multiple ingredients to detect allergens.
- **Real-Time Performance**: The application offers quick responses for faster decision-making.

## Technologies Used

- **Python**: For backend development, machine learning model training, and data manipulation.
- **Pandas**: For data processing, cleaning, and manipulation.
- **Scikit-learn**: For implementing machine learning algorithms, including Random Forest for allergen detection.
- **Flask**: A micro-framework for building the API and handling backend requests.
- **Streamlit**: For front-end development, providing an interactive and user-friendly interface.
- **Joblib/Pickle**: For saving and loading the trained machine learning models.

## Project Structure

```
Datasets/
├── Allergen_Status_of_Food_Products.csv    # Raw food allergen data
├── preprocessed_data.csv                  # Cleaned and preprocessed dataset for model training

Model/
├── leave_one_out_encoder.pkl              # Encoder used during data preprocessing
├── random_forest_model.pkl               # Trained Random Forest model for allergen detection

Scripts/
├── AI_SafeBite_Data_Preprocessing.ipynb    # Data preprocessing and cleaning steps
├── AI_SafeBite_EDA.ipynb                  # Exploratory data analysis (EDA)
├── AI_SafeBite_Model_Testing.ipynb        # Model testing and evaluation
├── AI_SafeBite_Streamlit_Flask_App.py     # Main app code using Flask and Streamlit
├── AI_SafeBite_flask_api.py              # Flask API for allergen prediction
├── AI_SafeBite_Modeltraining.ipynb       # Model training and validation
├── AI_SafeBite.pdf                       # Final project documentation
```

## Getting Started

Follow these steps to set up and run the **SafeBite** project locally.

### 1. Clone the Repository

Open your terminal or command prompt and clone the repository by running the following command:

```bash
git clone https://github.com/AabidMK/SafeBite_Infosys_Internship_Oct2024.git
```

Navigate into the cloned directory:

```bash
cd SafeBite_Infosys_Internship_Oct2024
```

### 2. Install Required Packages

Make sure you have **pip** installed. 
To simplify the installation of dependencies, use the requirements.txt file 

```bash
pip install -r requirements.txt
```

### 3. Prepare the Datasets

Ensure that the datasets are placed in the `Datasets/` directory as shown below:

```
Datasets/
├── Allergen_Status_of_Food_Products.csv    # Raw allergen data
└── preprocessed_data.csv                  # Cleaned dataset for training
```

If these files are missing, you need to obtain them and place them in the correct directory.

### 4. Train the Model

To train the model on the dataset, run the following script:

```bash
python AI_SafeBite_Modeltraining.ipynb
```

This script will preprocess the data, train the model, and save the trained models (`random_forest_model.pkl` and `leave_one_out_encoder.pkl`).

### 5. Run the Application

To run the SafeBite web app, use the following command:

```bash
streamlit run AI_SafeBite_Streamlit_Flask_App.py
```

Once the app is running, open your browser and visit `http://localhost:5000` to interact with the application.

### 6. Run the Flask API

If you want to use the SafeBite Flask API for allergen detection, run:

```bash
python AI_SafeBite_flask_api.py
```

This will start the Flask API server, allowing you to interact with the app programmatically for allergen predictions.

## Live Demo

```bash
https://safebite-551h.onrender.com/
```

## Contributing

We welcome contributions to improve SafeBite! If you'd like to contribute, please fork the repository, make changes, and submit a pull request. You can also open an issue if you have suggestions or find any bugs.
---


### Food Allergy Detection System  
GitHub: [github.com/CSSwetha/FoodAllergyDetection](https://github.com/CSSwetha/FoodAllergyDetection)  
Technologies: Python, Machine Learning, OpenCV, TensorFlow/Keras, Flask, React, OCR  

#### Project Overview: 
Developed an AI-powered Food Allergy Detection System that identifies potential allergens in food items by analyzing images and ingredient lists. The system integrates **computer vision and natural language processing (NLP)** to detect allergens from food labels, ensuring safety for individuals with dietary restrictions.

#### Key Contributions:  
- Image Processing & OCR: Implemented Optical Character Recognition (OCR) using Tesseract to extract ingredient lists from food packaging.  
- Allergen Classification: Developed a machine learning model (TensorFlow/Keras) to classify food items and cross-check allergens based on predefined allergy databases.  
- Web Application: Built an intuitive React-based front-end with a Flask backend, allowing users to scan food labels via mobile or upload images for allergen detection.  
- Database Management: Designed and maintained a structured SQL/NoSQL database to store allergen information and user preferences.  
- API Integration: Integrated external APIs for real-time allergen database updates and user notifications.  
- Deployment & Optimization: Optimized model inference time for real-time allergen detection and deployed the system on **AWS/GCP** for scalability.  

#### Impact & Achievements:
✅ Enhanced Food Safety: Helps individuals with food allergies make informed choices by identifying allergens in real time.  
✅ High Accuracy: Achieved X% accuracy (mention model performance) in allergen detection based on extensive dataset training.  
✅ User-Centric Design:Created a seamless, mobile-friendly interface improving accessibility and usability.  

---



