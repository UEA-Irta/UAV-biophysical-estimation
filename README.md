
# UAV Biophysical Traits Estimation

## Objective

This library is designed to estimate biophysical variables such as LAI (Leaf Area Index), fIPAR (Fraction of Incoming Photosynthetically Active Radiation), and other related traits derived from UAV data using configurable empirical models, specifically Random Forest (RF) and Neural Networks (NN). The goal is to facilitate biophysical parameter extraction for applications in precision agriculture and ecological research.

The library provides:

1. **Data Preprocessing**: Processes UAV-derived datasets, ensuring compatibility for model training and inference.
2. **Model Training and Testing**: Includes tools to configure, train, and validate RF and NN models for biophysical variable estimation.
3. **Inference**: Applies trained models to predict biophysical variables on new datasets.

---

## Features

### Biophysical Variables Extracted

- **LAI (Leaf Area Index)**: Quantifies canopy density and leaf area.
- **fIPAR (Fraction of Incoming Photosynthetically Active Radiation)**: Indicates the fraction of light intercepted by the canopy.
- **Additional Traits**: The library is extensible to estimate other biophysical variables with appropriate data and model configurations.

### Supported Models

- **Random Forest (RF)**: Ensemble-based regressor with configurable hyperparameters.
- **Neural Networks (NN)**: Fully connected networks with customizable architecture.

---

## Installation

To use this project, ensure you have Python 3.x installed. Then, clone the repository and install the required dependencies.

1. Clone the repository:
   ```bash
   git clone https://github.com/cesar-minuesa/uav-biophysical-estimation.git


2. Install dependencies:
   ```bash
   pip install -r requirements.txt


## Requirements

This project requires the following libraries:

- `numpy`
- `pandas`
- `matplotlib`
- `scikit-learn`
- `keras`
- `joblib`
- `geopandas`
- `rasterio`
- `fiona`
- `shapely`
- `rasterstats`
- `scikit-image`

---

## Main Scientific References

- Gao, R., Torres-Rua, A., Aboutalebi, M., White, W., Anderson, M., Kustas, W., Agam, N., Alsina, M., Alfieri, J., Hipps, L., Dokoozlian, N., Nieto, H., Gao, F., McKee, L., Prueger, J., Sanchez, L., Mcelrone, A., Bambach-Ortiz, N., Coopmans, C., and Gowing, I.: LAI estimation across California vineyards using sUAS multi-seasonal multi-spectral, thermal, and elevation information and machine learning, Irrigation Sci., 40, 731–759, https://doi.org/10.1007/s00271-022-00776-0, 2022. 
- Quintanilla-Albornoz, M., Miarnau, X., Pelechá, A., Casadesús, J., García-Tejera, O., and Bellvert, J.: Evaluation of transpiration in different almond production systems with two-source energy balance models from UAV thermal and multispectral imagery, Irrigation Sci., https://doi.org/10.1007/s00271-023-00888-1, 2023. 

## Notes

- **Extensibility**: The pipeline is designed to support additional features or biophysical variables by updating the configuration file and adapting the utility scripts.
- **Reproducibility**: Using the `config/` directory ensures consistency in parameter settings across different runs.

---

## Contact

For issues or feature requests, please contact: [cesar.minuesa@irta.cat].

