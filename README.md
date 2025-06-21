# Bazarya-Model-Training

This repository contains the data processing, model training, evaluation, and export pipelines for **Bazarya**, a lightweight market price forecasting and alert system designed for local markets in Ethiopia.

It serves as the **ML backend** for the [Bazarya Flask app](https://github.com/keneandita/bazarya), which provides a web interface for price forecasts, user submissions, and alerts.

---

## Purpose

To forecast daily prices of agricultural and food products using time series models (e.g., ARIMA, LSTM). This repo ensures:

- Clean and structured market price data
- Automated preprocessing and feature engineering
- Reproducible training and evaluation of models
- Export of serialized models (e.g., `.pkl`, `.h5`) for use in production

---

## Evaluation Metrics

- RMSE (Root Mean Square Error)
- MAE (Mean Absolute Error)
- MAPE (Mean Absolute Percentage Error)

These metrics are logged during training and exported in `logs/`.

---

## Planned Enhancements

- ✅ Support for multiple markets per product
- ✅ Support for categorical encodings
- 🔄 Multivariate models (e.g., inflation, weather)
- 🔄 Integration with real-time web scrapers
- 🔄 HuggingFace/DVC pipeline versioning

---

## Integration with Bazarya Flask App

Trained models from this repo are loaded in the [Bazarya Web App](https://github.com/yourusername/bazarya) for live price prediction.

Ensure the model file paths in the Flask repo point to exported files from this repo.

---

## Contributions

Feel free to:

- Add new model types (e.g., Prophet, XGBoost)
- Improve preprocessing or scaling techniques
- Report issues or raise pull requests

---

## Contact

Questions or feedback? email: `Keneansufa@gmail.com`