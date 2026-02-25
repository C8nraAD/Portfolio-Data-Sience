# 🛡️ AI Insurance Premium Advisor: Predictive Underwriting Engine

[Live Deployment](https://ai-health-advisor-onjbw9a9ecq5pnxhekzhep.streamlit.app) | [Repository](https://github.com/C8nraAD/AI-Health-Advisor)

## 🎯 Architecture Overview & Business Objective

An interactive underwriting tool designed to simulate individual insurance premiums based on health and lifestyle factors. The application dynamically fetches a pre-trained regression model from cloud storage and performs real-time inference. It features a custom recommendation engine that quantifies the financial impact of health improvements (e.g., BMI reduction, quitting smoking), visualizing potential savings through interactive dashboards.

## 🛠 Tech Stack & Ecosystem

| Component | Technology |
| :--- | :--- |
| **Frontend & UI** | `Streamlit` (Stateful interactive UI) |
| **Machine Learning** | `PyCaret` (Regression pipeline & inference) |
| **Cloud Storage** | `AWS S3 / Boto3` (Remote model provisioning) |
| **Data Engineering** | `Pandas` (Data transformation), `Dataclasses` (State management) |
| **Data Visualization** | `Plotly Express` (Dynamic financial impact charts) |

## 🏗 Core Pipeline Mechanics

### 1. Dynamic Cloud Inference
The application avoids bundling heavy `.pkl` files in the repository. It authenticates with AWS S3 via Boto3 to securely download and cache the PyCaret regression model (`@st.cache_resource`) into memory on startup, ensuring fast, real-time inference on user input.

### 2. Object-Oriented Simulation Engine
A modular `RecommendationEngine` evaluates the user's health profile (`UserProfile`) against predefined medical thresholds. It executes real-time "what-if" simulations by duplicating and mutating the user's state, recalculating the risk baseline to project localized financial savings.

### 3. Stateful UI Orchestration
Leverages Streamlit's `session_state` to decouple user inputs from the simulation cache. This ensures the UI remains highly responsive during Plotly chart rendering and prevents redundant model inferences during state changes.# 🛡️ AI Insurance Premium Advisor: Predictive Underwriting Engine

[Live Deployment](TUTAJ_WSTAW_LINK) | [Repository](TUTAJ_WSTAW_LINK)

## 🎯 Architecture Overview & Business Objective

An interactive underwriting tool designed to simulate individual insurance premiums based on health and lifestyle factors. The application dynamically fetches a pre-trained regression model from cloud storage and performs real-time inference. It features a custom recommendation engine that quantifies the financial impact of health improvements (e.g., BMI reduction, quitting smoking), visualizing potential savings through interactive dashboards.

## 🛠 Tech Stack & Ecosystem

| Component | Technology |
| :--- | :--- |
| **Frontend & UI** | `Streamlit` (Stateful interactive UI) |
| **Machine Learning** | `PyCaret` (Regression pipeline & inference) |
| **Cloud Storage** | `AWS S3 / Boto3` (Remote model provisioning) |
| **Data Engineering** | `Pandas` (Data transformation), `Dataclasses` (State management) |
| **Data Visualization** | `Plotly Express` (Dynamic financial impact charts) |

## 🏗 Core Pipeline Mechanics

### 1. Dynamic Cloud Inference
The application avoids bundling heavy `.pkl` files in the repository. It authenticates with AWS S3 via Boto3 to securely download and cache the PyCaret regression model (`@st.cache_resource`) into memory on startup, ensuring fast, real-time inference on user input.

### 2. Object-Oriented Simulation Engine
A modular `RecommendationEngine` evaluates the user's health profile (`UserProfile`) against predefined medical thresholds. It executes real-time "what-if" simulations by duplicating and mutating the user's state, recalculating the risk baseline to project localized financial savings.

### 3. Stateful UI Orchestration
Leverages Streamlit's `session_state` to decouple user inputs from the simulation cache. This ensures the UI remains highly responsive during Plotly chart rendering and prevents redundant model inferences during state changes.