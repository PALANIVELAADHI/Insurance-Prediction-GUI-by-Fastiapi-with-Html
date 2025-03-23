# Insurance-Prediction-GUI-by-Fastiapi-with-Html

# Crime Prediction by AI

## Overview
This project implements a **crime prediction system** using machine learning models. It is built with **FastAPI** for the backend, **SQLAlchemy** for database management, and includes authentication features. The system supports multiple machine learning models for crime prediction, including **Decision Tree, Random Forest, and SVM**.

## Features
- **User Authentication:** Register and login system using FastAPI.
- **Machine Learning Models:** Predict crime occurrences using trained models.
- **Database Integration:** SQLAlchemy for user management.
- **Preprocessing:** Pre-trained preprocessing pipeline for handling input data.
- **Web UI:** HTML templates for login, registration, and home pages.

---
## Project Structure

```
fastapi-auth/
├── main.py                 # Main FastAPI app setup
├── auth.py                 # Authentication routes
├── model.py                # Prediction and home routes
├── config.py               # Centralized templates config
├── db.py                   # Database setup (SQLAlchemy)
├── models.py               # SQLAlchemy User model
├── templates/
│   ├── auth/
│   │   ├── login.html      # Login page
│   │   ├── register.html   # Registration page
│   │   ├── home.html       # Home page with form and back button
│   ├── result.html         # (Optional) Result page if used
│   ├── error.html          # Error page
├── static/
│   ├── auth/
│   │   ├── home.css        # CSS for home.html
├── decision_tree.h5        # Trained Decision Tree model
├── random_forest.h5        # Trained Random Forest model
├── svm.h5                  # Trained SVM model
├── preprocessor.pkl        # Preprocessor for model input
├── .gitignore              # Git ignore file
├── README.md               # Project documentation
└── requirements.txt        # Python dependencies
```

---
## Installation

### Prerequisites
- Python 3.8+
- FastAPI
- SQLAlchemy
- scikit-learn
- TensorFlow/Keras (for model loading)
- Uvicorn (for running the FastAPI server)

### Setup
1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/fastapi-auth.git
   cd fastapi-auth
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the FastAPI server**:
   ```bash
   uvicorn main:app --reload
   ```

4. **Access the application**:
   Open your browser and go to `http://127.0.0.1:8000`

---
## Usage
1. **Register/Login** using the authentication system.
2. **Navigate to Home** and provide input for crime prediction.
3. **Choose a Model** (Decision Tree, Random Forest, or SVM).
4. **Submit the form** and view predictions.

---
## API Endpoints
| Endpoint         | Method | Description              |
|-----------------|--------|--------------------------|
| `/register`     | POST   | User registration        |
| `/login`        | POST   | User login               |
| `/home`         | GET    | Home page                |
| `/predict`      | POST   | Predict crime occurrence |

---
## Contributing
Pull requests are welcome! Please open an issue first to discuss proposed changes.

---
## License
This project is open-source and available under the [MIT License](LICENSE).

---
## Contact
For questions or support, contact [your-email@example.com].

