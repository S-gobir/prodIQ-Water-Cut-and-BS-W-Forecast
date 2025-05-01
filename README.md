# prodIQ: Water Cut and BS&W Forecast
# 🔍 ProdIQ: Forecasting Water Cut & BS&W in Oilfield Surface Operations

**ProdIQ** is a pilot machine learning project aimed at forecasting two essential parameters in oil and gas production operations:

- **Water Cut**
- **Basic Sediment & Water (BS&W)**

These forecasts are important for optimizing well performance, minimizing water handling costs, and making proactive field level decisions. The model is trained on real world surface production data and demonstrates strong predictive capabilities using several state of the art ML algorithms.

---

## 🎯 Project Objective

To develop and compare multiple regression models that accurately predict Water Cut and BS&W using key surface and near wellhead parameters. This helps operators gain real time insights into produced fluid characteristics  an important step for production optimization, planning, and surveillance.

---

## 📊 Input Parameters

The following features were used in training the models:

- `Wellhead Pressure`
- `Choke Size`
- `Behind Casing Pressure`
- `Tubing Head Pressure`
- `Tubing Head Temperature`
- `Pressure Downstream Choke`
- `Temperature Downstream Choke`

---

## 🤖 Model Performance

All models were evaluated using **R² Score**, **Mean Squared Error (MSE)**, and **Mean Absolute Error (MAE)**:

| Model                | R² Score | MSE           | MAE           |
|----------------------|----------|----------------|----------------|
| **XGBoost**          | 0.7768   | 25.49          | 3.91           |
| **HistGradientBoost**| 0.7730   | 25.92          | 3.82           |
| **CatBoost**         | 0.7730   | 25.92          | 3.82           |
| **ExtraTrees**       | 0.7708   | 26.18          | 3.98           |
| **KNN**              | 0.7685   | 26.44          | 3.88           |
| **RandomForest**     | 0.7681   | 26.49          | 3.89           |
| **Ridge**            | 0.4674   | 60.83          | 6.08           |
| **Lasso**            | 0.2746   | 82.85          | 7.60           |

> 🧠 Ensemble models (XGBoost, CatBoost, HistGradientBoost) performed the best, while linear models (Ridge, Lasso) were less effective on this dataset.

---

## 📂 Dataset (Open Source)

I’ve also released a **12 well production dataset** used in this project on Kaggle. It includes 17 parameters such as pressures, temperatures, fluid content, and gas lift info enabling researchers and practitioners to experiment and improve on this baseline.

📦 **Access the dataset**: [Kaggle - ProdIQ Dataset Series]((https://www.kaggle.com/datasets/sgobir/production-dataset/data))



## 🛠️ Libraries Used

- `scikit-learn`
- `xgboost`
- `catboost`
- `joblib`
- `pandas`, `numpy`, `matplotlib`, `seaborn`

---

## 📌 Applications in Oil & Gas

- Real time **production diagnostics**
- Forecasting produced **fluid properties**
- Reducing **water disposal** and **emulsion handling costs**
- Early detection of **formation or equipment issues**
- Supporting **digital oilfield** and **smart well** initiatives

---

## 🤝 Collaboration Invitation

This project is open-source, and I'm excited to collaborate with other researchers, engineers, and students working on:
- Subsurface & surface production modeling  
- Smart well operations  
- Machine learning applications in energy

Feel free to fork, improve, and contribute to this project — or reach out if you're interested in building something together!

---

## 👨‍💻 Author

**Sunusi Muhammad Ibrahim**  
Petroleum Engineering |  computer visio| AI for energy  
📍 Bayero University Kano  
🔗 [LinkedIn](https://www.linkedin.com/in/sunusimuhammadi) | [GitHub](https://github.com/your-profile)

---

> *Let’s power smarter oilfields with open data and machine learning.*

