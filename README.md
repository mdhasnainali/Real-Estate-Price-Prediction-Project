# Real Estate Price Prediction

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

This project aims to predict real estate prices using the [Bengaluru House Price Dataset](https://www.kaggle.com/datasets/amitabhajoy/bengaluru-house-price-data). The dataset contains information about various attributes of houses in Bengaluru, including area type, availability, location, size, society, total square footage, number of bathrooms, number of balconies, and price.

## Dataset Information

- Attribute Type: Real
- Instances: 13320
- Attributes: 9

## Project Overview

This data science project series guides you through the step-by-step process of building a real estate price prediction website. The project encompasses the following components:

1. **Model Building**: We use scikit-learn and linear regression to build a model using the Bengaluru home prices dataset from Kaggle. The model incorporates various data science concepts such as data loading and cleaning, outlier detection and removal, feature engineering, dimensionality reduction, grid search cross-validation for hyperparameter tuning, and more.

2. **Python Flask Server**: We develop a Python Flask server that utilizes the trained model to serve HTTP requests. The server handles requests from the website and returns the predicted prices.

3. **Website**: The project also includes a website built using HTML, CSS, and JavaScript. The website allows users to input home square footage, number of bedrooms, etc. It then communicates with the Python Flask server to retrieve the predicted price and displays it to the user.

## Project Structure

The project repository is structured as follows:

```
├── README.md
├── client
│ ├── app.css
│ ├── app.html
│ └── app.js
├── model
│ ├── banglore_home_prices_model.pickle
│ ├── columns.json
│ ├── dataset
│ │ └── Bengaluru_House_Data.csv
│ └── real-estate-price.ipynb
└── server
├── artifacts
│ ├── banglore_home_prices_model.pickle
│ └── columns.json
├── server.py
└── util.py

```

- `/client`: Contains the client-side code for the website, including HTML, CSS, and JavaScript files.
- `/model`: Contains the trained model and related files, such as the pickled model file (`banglore_home_prices_model.pickle`), the column mapping file (`columns.json`), and the dataset file (`Bengaluru_House_Data.csv`).
- `/server`: Contains the server-side code for the Python Flask server, including the Flask server file (`server.py`) and utility functions file (`util.py`).
- `/server/artifacts`: Contains additional artifacts related to the server, such as the pickled model file and the column mapping file.

## Getting Started

To get started with the project, follow these steps:

1. Clone the repository: `git clone https://github.com/mdhasnainali/Real-Estate-Price-Prediction-Project.git`
2. Set up the required dependencies.
3. Explore the Jupyter notebooks in the `/model` directory for data preprocessing and model building.
4. Start the Flask server by running `server.py` in the `/server` directory.
5. Access the website by opening the HTML file (`app.html`) in the `/client` directory.

## Contributing

Contributions are welcome! Feel free to submit pull requests or report issues.

## Acknowledgements

We would like to acknowledge the Kaggle community for providing the Bengaluru House Price Dataset.

## License

This project is licensed under the [MIT License](LICENSE).

---

© Copyright 2023 | Md. Hasnain Ali
