# Forest Fire Prediction

This project predicts the Forest Weather Index based on various environmental parameters using a Ridge regression model. It leverages historical data from Algerian forest regions to provide predictions about fire likelihood, helping in early warning and resource management.

---

## About The Project

The model predicts forest fire risk using key weather and fuel moisture parameters: Temperature, Relative Humidity (RH), Wind speed (Ws), Rainfall (Rain), FFMC, DMC, ISI, Classes, and Region. It was trained on the Algerian Forest Fires Dataset which includes data from two regions of Algeria (Bejaia and Sidi Bel-abbes) during June to September 2012.

- Dataset contains 244 instances (122 per region) classified into fire (138 instances) and no fire (106 instances).
- The data attributes reflect daily weather observations and components of the Fire Weather Index system.

### Dataset Attributes Summary:
- **Temperature:** Max temperature at noon (22 to 42 °C)
- **RH:** Relative Humidity in %
- **Ws:** Wind speed in km/h
- **Rain:** Total daily rainfall in mm
- **FFMC, DMC, ISI:** Fire Weather Index components indicating fuel moisture and fire spread potential
- **Classes:** Fire occurrence (fire/not fire)
- **Region:** Location identifier for the forest area

---

## Folder Structure

├── application.py # Flask app entry point
├── requirements.txt # Project dependencies
├── models/ # Contains pickle files for scaler and trained Ridge regression model
│ ├── scaler_new.pkl
│ └── ridge_new.pkl
├── notebooks/ # Jupyter notebooks for data exploration and model development
│ └── your_notebook.ipynb
└── templates/ # HTML templates for Flask app UI
└── index.html, home.html, etc.


---

## Installation & Setup

1. Clone the repository: git clone https://github.com/MohammadSamiullaBilagi/Forest-Fire-Prediction.git
cd Forest-Fire-Prediction



2. Create and activate a Python virtual environment (recommended): python3 -m venv venv
source venv/bin/activate


3. Install dependencies: pip install -r requirements.txt


4. Run the Flask application: python application.py


5. Open a browser and access `http://localhost:5000` to interact with the prediction form.

---

## Usage

- Input weather parameters into the web form.
- Submit to get the predicted fire weather index.
- The prediction logic uses a standard scaler for input normalization followed by the Ridge regression model.

---

## Results

The model has been trained on historical data and predicts fire risk with the aim of aiding forest fire prevention and resource allocation.

---

## Future Work

- Integration of more recent datasets with broader geographic coverage.
- Deploy as a REST API for easier integration with other systems.
- Use advanced models such as Random Forest or Gradient Boosting to improve prediction accuracy.
- Visualize predictions on map-based dashboards.

---

## Acknowledgements

- Dataset Source: Algerian Forest Fires Dataset
- Machine Learning and Flask community support

---

## License

Specify your license here, e.g., MIT License or others.

---

Thank you for exploring the Forest Fire Prediction project! Feel free to contribute or raise issues for improvements.





