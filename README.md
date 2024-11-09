# Revolutionizing Tamil Nadu Agriculture: AI-Powered Crop Yield Forecasting and Disease Prediction for Oil Seed Crops 🌱

## Project Overview

This project aims to empower farmers with AI-based insights for predicting crop yields and identifying diseases early, potentially transforming the agriculture sector in Tamil Nadu and beyond. By leveraging cutting-edge technologies, including machine learning and deep learning, the system provides crop recommendations based on weather patterns and soil conditions, fertilizer suggestions, and disease predictions using image recognition.

### Features:
- **Crop Yield Prediction:** Provides recommendations on suitable crops based on soil health, weather conditions, and region.
- **Fertilizer Recommendation:** Suggests appropriate fertilizers based on soil nutrients for oilseed crops.
- **Plant Disease Detection:** Detects diseases in plants through image recognition and provides guidance on treatment.
- **Weather Data Integration:** Fetches real-time temperature and humidity data for accurate recommendations.

---

## Technologies Used

This project uses the following libraries and frameworks:

- **Flask:** Web framework for building the application interface.
- **NumPy & Pandas:** For data manipulation and analysis.
- **scikit-learn:** For machine learning models (e.g., Random Forest).
- **Torch (PyTorch):** For deep learning-based image classification models.
- **requests:** For fetching weather data via an API.
- **Pillow:** For image processing.
- **Gunicorn:** For serving the Flask application.

---

## How to Run the Application

1. **Download the code** or clone the repository:

    ```bash
    git clone <repository-url>
    cd <project-directory>
    ```

2. **Ensure models are in the correct paths:**
   
    - The `plant_disease_model.pth` file should be located in the `TnHarvest\models` directory.
    - The `RandomForest.pkl` model should also be located in the `TnHarvest\models` directory.
    - Ensure the `fertilizer.csv` file is located in the `TnHarvest\Data` directory for fertilizer recommendations.

4. **Set up the configuration file (`config.py`):**
   
    - In `config.py`, add your **weather API key** to access weather data:

    ```python
    weather_api_key = "<Your-OpenWeatherMap-API-Key>"
    ```

6. **Run the Flask Application:**

    To run the app locally in development mode:

    ```bash
    python app.py
    ```

    The Flask app will start running on `http://127.0.0.1:5000/`.
