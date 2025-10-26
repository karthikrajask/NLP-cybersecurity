
# NCRP — NLP Model for Cyber Crime Categorization

This repository contains the NCRP (National/Network Crime Response Program) NLP model for categorizing cyber crime reports. It also includes a simple Streamlit chatbot interface so users can interact with the model by asking questions or pasting incident text and receiving predicted cyber-crime categories.

This README shows how to set up the environment, run the Streamlit chatbot, and integrate your model file (sklearn, joblib, or a Transformers-based model). A ready-to-run example `streamlit_app.py` is included below — paste it into your repo and run `streamlit run streamlit_app.py`.

---
## Features
- Load a trained classification model (sklearn/joblib or transformers).
- Simple conversational UI using Streamlit where users ask queries or paste incident descriptions.
- Shows model prediction and confidence score.
- Easy to extend to return multi-label categories, explanation text (LIME/SHAP), or links to follow-up actions.

---
## Requirements

Create a virtual environment and install dependencies:

- Python 3.8+
- Streamlit
- scikit-learn (if using sklearn models)
- joblib (if using joblib-saved model)
- transformers & torch (if using transformer-based models)
## How to run the Streamlit chatbot

1. Place your trained model in `models/` (e.g., `models/ncrp_model.joblib`).
2. Run:
```bash
streamlit run streamlit_app.py
```
4. The app opens in your browser (usually http://localhost:8501). Ask a question or paste the text of an incident and press Enter / Submit to get a category prediction.

---
