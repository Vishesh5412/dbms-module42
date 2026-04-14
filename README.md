# 🏥 Secure Clinical Summary View Generator — Sign-In

A modern Streamlit sign-in page backed by MongoDB, JWT authentication, and cookie-based session management.

## Quick Start

### 1. Prerequisites

- **Python 3.9+**
- **MongoDB** running locally (`mongodb://localhost:27017`) or on Atlas

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Seed the test users

```bash
python setup_user.py
```

This creates three demo accounts in the `clinical_db.users` collection:

| Username     | Password       | Role            |
|--------------|----------------|-----------------|
| `admin`      | `admin123`     | Clinical        |
| `researcher` | `research123`  | Research        |
| `manager`    | `manage123`    | Administrative  |

### 4. Run the app

```bash
streamlit run app.py
```

Open the URL printed in the terminal (usually `http://localhost:8501`).

## Environment Variables (optional)

| Variable     | Default                                     | Description          |
|-------------|----------------------------------------------|----------------------|
| `MONGO_URI` | `mongodb://localhost:27017`                  | MongoDB connection   |
| `JWT_SECRET`| `clinical-summary-dev-secret-key-change-in-prod` | JWT signing key  |

## Project Structure

```
├── app.py            # Streamlit sign-in page + dashboard stub
├── setup_user.py     # Seed demo users into MongoDB
├── requirements.txt  # Python dependencies
└── README.md         # You are here
```
# DBMS-sem3
