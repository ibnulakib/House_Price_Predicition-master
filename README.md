# 🏠 House Price Prediction

A full-stack machine learning web application that predicts house prices based on user-provided property features. Built with Python (scikit-learn + Flask) for the ML backend and a PHP/HTML frontend, this project demonstrates an end-to-end ML pipeline - from data preprocessing and model training to real-time predictions via a web interface.

---

## 📌 Project Overview

This project was developed to explore supervised machine learning regression techniques applied to real estate data. A trained ML model is served through a Flask REST API, which a web frontend calls to return live price predictions to the user.

**Key highlights:**
- Trained and evaluated a regression model using scikit-learn
- Built a REST API with Python Flask to serve model predictions
- Created a full web interface (PHP + HTML/CSS/JS) to interact with the API
- Covered the full ML lifecycle: data loading → preprocessing → training → evaluation → deployment

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Machine Learning | Python, scikit-learn, NumPy, Pandas |
| Model Training | Jupyter Notebook, Anaconda |
| Backend API | Python Flask |
| Frontend | PHP, HTML, CSS, JavaScript |
| Local Server | XAMPP |
| IDE | PyCharm |

---

## 🧠 How It Works

```
User Input (Web Form)
        ↓
PHP Frontend  →  Flask REST API  →  Trained ML Model
                                          ↓
                              Predicted Price Returned
                                          ↓
                              Displayed on Web Page
```

1. The user enters property details (e.g. number of rooms, area, location) in the web form
2. The PHP frontend sends the data to the Flask API endpoint
3. Flask passes the input to the pre-trained scikit-learn model
4. The model returns a predicted price, which is displayed back to the user

---

## 📁 Project Structure

```
House_Price_Predicition-master/
│
├── House_Price_Predicition-master/
│   ├── notebook/               # Jupyter Notebooks for EDA & model training
│   ├── model/                  # Saved trained model (pickle file)
│   ├── static/                 # CSS and JavaScript files
│   ├── templates/              # HTML templates
│   ├── app.py                  # Flask API - serves predictions
│   └── *.php                   # PHP frontend pages
│
└── README.md
```

---

## ⚙️ Installation & Setup

### Prerequisites

Make sure the following are installed on your machine:

- [XAMPP v3.2.3+](https://www.apachefriends.org/) - for running the PHP frontend
- [Python 3.6+](https://www.python.org/)
- [Anaconda](https://www.anaconda.com/) - for managing Python environments
- [PyCharm](https://www.jetbrains.com/pycharm/) - recommended IDE

### Step 1 - Clone the repository

```bash
git clone https://github.com/ibnulakib/House_Price_Predicition-master.git
cd House_Price_Predicition-master
```

### Step 2 - Set up the Python environment

```bash
# Create and activate a conda environment
conda create -n house-price python=3.6
conda activate house-price

# Install required packages
pip install numpy pandas scikit-learn flask
```

### Step 3 - Train the model (optional)

Open the Jupyter Notebook to explore the data and retrain the model:

```bash
jupyter notebook
```

Run the notebook cells to preprocess the data and save the trained model.

### Step 4 - Start the Flask API

```bash
python app.py
```

The API will run at `http://localhost:5000`

### Step 5 - Start the PHP frontend

1. Copy the project folder into your XAMPP `htdocs` directory
2. Start Apache in the XAMPP Control Panel
3. Open your browser and go to `http://localhost/House_Price_Predicition-master`

---

## 📦 Required Python Packages

```
numpy
pandas
scikit-learn
flask
```

Install all at once:

```bash
pip install numpy pandas scikit-learn flask
```

---

## 🔍 ML Model Details

- **Algorithm:** Regression (e.g. Linear Regression / Random Forest - see notebook for details)
- **Libraries:** scikit-learn, NumPy, Pandas
- **Training environment:** Jupyter Notebook (Anaconda)
- **Input features:** Property characteristics (area, rooms, location, etc.)
- **Output:** Predicted house price

---

## 📊 Features

- Interactive web form for entering property details
- Real-time price prediction via Flask REST API
- Clean, simple frontend UI
- Modular codebase separating ML logic from web layer

---

## 🚀 Future Improvements

- [ ] Upgrade Python to 3.11+ and modernise dependencies
- [ ] Replace PHP frontend with a React or Next.js UI
- [ ] Add model accuracy metrics and a visualisation dashboard
- [ ] Deploy to cloud (e.g. Heroku, Render, or AWS)
- [ ] Add input validation and error handling on the API

---

## 👤 Author

**Ibnul Akib**
[GitHub Profile](https://github.com/ibnulakib)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
