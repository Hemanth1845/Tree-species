# 🌳 Tree Intelligence Assistant

> An intelligent machine learning-based tool that recommends the most suitable tree species for a given location. Designed to assist urban planners, botanists, researchers, and nature enthusiasts in selecting tree species based on key geospatial and botanical parameters.

---

## 📘 Project Overview

The **Tree Intelligence Assistant** is a user-friendly application that predicts the **top 3 suitable tree species** based on user inputs like:

- Latitude & Longitude  
- Tree Diameter  
- City and State  
- Native or Non-native status  

It is powered by a trained machine learning model that analyzes patterns from a large dataset (`5M_trees`) and offers real-time predictions through an interactive **Streamlit web interface**.

---

## 🚀 Key Features

- 🔎 **Species Prediction**: Get top 3 tree species suited for your location and input parameters.  
- 📍 **Location-Based Input**: Accepts latitude, longitude, and city for geo-specific results.  
- 📊 **Model Inference**: Uses a pre-trained neural network model for fast and reliable predictions.  
- 🧠 **Machine Learning Enabled**: Built using scikit-learn and joblib for robust model deployment.  
- ⚙️ **Streamlit Web UI**: Interactive and simple user interface for entering inputs and viewing results.  
- 🧪 **CNN Model Support (WIP)**: A deep learning CNN model (`tree_CNN.ipynb`) is included for image-based species classification (optional feature).  

---

## 📂 Folder Structure

```
Tree_Species_Classification/
├── streamlit_integrated.py        # Main Streamlit app file
├── scaler.joblib                  # Saved standard scaler
├── nn_model.joblib                # Trained machine learning model
├── tree_CNN.ipynb                 # CNN training notebook (optional feature)
├── requirements.txt               # Required Python dependencies
├── 5M_trees.zip                   # Original dataset used for model training
└── ...
```

---

## 🛠️ Installation & Usage

1. **Clone the repository**
```bash
git clone https://github.com/Hemanth1845/Tree_Species_Classification.git
cd Tree_Species_Classification
```

2. **Install dependencies**
```bash
pip install -r requirements.txt
```

3. **Run the Streamlit App**
```bash
streamlit run streamlit_integrated.py
```

4. **Use the Web Interface**

Follow the prompts on the webpage to enter inputs like latitude, longitude, tree diameter, city, and native status. The app will display the top 3 recommended tree species for your location.

---

## 🧠 Model Info

- **Model**: Neural Network Classifier  
- **Libraries used**: `scikit-learn`, `joblib`, `streamlit`, `pandas`, `numpy`  
- **Training Data**: Cleaned and preprocessed dataset with millions of tree samples  
- **Input Features**: `[Latitude, Longitude, Diameter, City, State, Native (1 or 0)]`  
- **Output**: Top 3 recommended tree species names based on model's probability ranking  

---

## 👤 Developed By

**Hemanth Ravada** ([@hemanth1845](https://github.com/Hemanth1845))  
Passionate ML Developer | Nature & AI Enthusiast

---

## 📄 License

This project is licensed under the **MIT License**. You are free to use, modify, and distribute it with proper attribution.
