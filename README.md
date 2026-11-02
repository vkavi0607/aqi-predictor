# 🌫️ AQI Predictor

This project predicts the **Air Quality Index (AQI)** based on environmental pollution parameters using a **Random Forest Regressor**. It provides both a **Jupyter Notebook** for model development and a **Streamlit web app** for interactive use.

---

## 📌 Features

- Predict AQI from PM2.5, NO2, CO, and O3 levels
- Visualize predictions using an interactive gauge
- Show feature importance for AQI prediction
- Evaluate model performance (RMSE, R²)
- Streamlit app for user-friendly deployment

---

## 🗂️ Project Structure

```
aqi_predictor_project/
├── app/                      # Streamlit app code
│   └── main.py
├── data/                     # Dataset directory
│   └── global_air_pollution_dataset.csv
├── models/                   # Trained model artifacts (saved after training)
├── notebooks/                # Jupyter notebook for development
│   └── AQI_Model_Development.ipynb
├── src/                      # Modular source code
│   ├── data_loader.py
│   ├── train_model.py
│   ├── predict.py
│   └── visualize.py
├── utils/                    # Utility functions
│   ├── logger.py
│   └── metrics.py
├── tests/                    # Unit tests
│   └── test_train_model.py
├── requirements.txt          # Dependencies
└── README.md                 # You are here 📍
```

---

## 📦 Installation

### 🔧 1. Clone the Repository
```bash
git clone https://github.com/your-username/aqi_predictor_project.git
cd aqi_predictor_project
```

### 🔧 2. Install Python Dependencies
```bash
pip install -r requirements.txt
```

> Optional: Create a virtual environment:
> ```bash
> python -m venv venv
> source venv/bin/activate  # On Windows: venv\Scripts\activate
> ```

---

## 📊 Dataset

The dataset must be placed in the `data/` folder and named:

```
global_air_pollution_dataset.csv
```

It should contain the following columns:

- `PM2.5 AQI Value`
- `NO2 AQI Value`
- `CO AQI Value`
- `Ozone AQI Value`
- `AQI Value`

---

## 🚀 Run the Streamlit App

```bash
streamlit run app/main.py
```

- Visit `http://localhost:8501` in your browser.
- Use sliders to adjust pollution levels and view the AQI prediction.

---

## 📓 Run the Notebook

If you prefer working in a Jupyter Notebook:

```bash
jupyter notebook notebooks/AQI_Model_Development.ipynb
```

This lets you:

- Experiment with data
- Tune the model
- Evaluate performance

---

## ✅ Running Tests

```bash
pytest tests/
```

This will execute unit tests defined in the `tests/` folder.

---

## 📈 Example Output

- AQI Prediction: `125.3`
- Category: ⚠️ Unhealthy for Sensitive Groups
- RMSE on test data: `23.47`

---![image](https://github.com/user-attachments/assets/38c5a653-2f6e-4584-9f9b-fd71c46800ad)
![image](https://github.com/user-attachments/assets/ed89ff3d-5d0d-410c-8bd5-30479cfc9992)
![image](https://github.com/user-attachments/assets/adaeacba-5e1f-4849-b395-409b01d1fb70)
![image](https://github.com/user-attachments/assets/d64f9ec0-9edd-456d-9f4e-0a72cfd464cf)
![image](https://github.com/user-attachments/assets/bf709449-2fe8-4d4e-bdfc-c1fe45d4874c)



## 📌 Future Improvements

- Add support for time-series forecasting
- Integrate external APIs (e.g., OpenAQ)
- Deploy to Streamlit Cloud or Heroku
- Add location-based pollution insights

---

## 👨‍💻 Author

Kaviyarasu V
[GitHub](https://github.com/vkavi0607/AQI-Prediction) | [LinkedIn](http://www.linkedin.com/in/kaviyarasu-v-502662367)
