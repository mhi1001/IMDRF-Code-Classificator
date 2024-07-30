# IMDRF Codes App
Exam project

## Table of Contents
- [Research](#research)
- [Requirements](#requirements)
- [Installation](#installation)
- [Running the Application](#running-the-application)
- [Usage](#usage)

## Research

**Introduction:**
In the healthcare sector, accurate documentation and communication are critical for effective patient care and regulatory compliance. 
Messages from doctors often contain a wealth of information that needs to be accurately categorized according to the International Medical Device Regulators Forum (IMDRF) codes. 
These codes are essential for classifying and standardizing medical device-related information. 
However, manually identifying the correct IMDRF codes from doctors' messages is a time-consuming and error-prone process.

**Problem statement:**
**Context:** Accurate documentation in healthcare is critical for patient care and regulatory compliance.
**Problem:** Manually identifying IMDRF codes from doctors' messages is inefficient and error-prone due to the complexity of medical terminology.
**Impact:** This inefficiency leads to increased workload, potential misclassification, and compromised data quality.
**Solution**: To create an app that assists companies in identifying the appropriate IMDRF codes for messages sent by doctors.

**Research Questions:**
- How accurately can the AI model classify doctors' messages into the correct IMDRF codes compared to human classification?
- What are the most common errors made by the AI model in identifying IMDRF codes from doctors' messages?
- Can the AI model adapt to new medical terminology and updates in IMDRF codes over time?

**Hypotheses:**
- The AI model will classify doctors' messages into the correct IMDRF codes with an accuracy rate of at least 90%, comparable to or better than human classification.
- The most common errors made by the AI model will be related to ambiguous or highly specialized medical terminology.
- The AI model will demonstrate the ability to adapt to new medical terms and IMDRF code updates with minimal additional training.

## Requirements

- Python 3.6+
- pip (Python package installer)

## Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/mhi1001/prototype-LLM
    cd 
    ```

2. **Create and activate a virtual environment:**

    On Windows:

    ```bash
    python -m venv venv
    venv\Scripts\activate
    ```

    On macOS/Linux:

    ```bash
    python3 -m venv venv
    source venv/bin/activate
    ```

3. **Install the required packages:**

    ```bash
    pip install -r requirements.txt
    ```

4. **Download the trained model and scaler files:**

    Ensure you have the trained model (`diabetes_logistic_model.pkl`). Place it in the root directory of the folder.

5. **Create and populate the `label_encoder_classes` files:**

    Ensure you have the `label_encoder_diabetes_classes.npy` file. Place it in the root directory of the folder.

## Running the Application

1. **Start the Flask application:**

    ```bash
    python app.py
    ```

2. **Open your web browser and go to:**

    ```
    http://127.0.0.1:5000/
    ```

## Usage

1. Fill out the form with the required health metrics and personal information.
2. Click the "Predict" button.
3. The prediction result will be displayed on the page.
