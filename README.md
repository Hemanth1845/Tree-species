🌿 Tree Species AI Classifier & Forestry Assistant
<div align="center">






</div>
📌 Project Summary
Tree Species AI Classifier is an intelligent, web-based tool for identifying tree species from images and location data. Leveraging deep learning and geospatial analysis, it empowers users to:

Classify tree images using a custom-trained CNN

Recommend species based on GPS and environment

Explore species distributions across cities

Gain insights from over 1.3M+ trees across the U.S.

Ideal for urban forestry planners, botanists, environmental scientists, and hobbyists.

🔥 Key Highlights
📷 AI-Powered Image Recognition (30 species)

📍 Location-Based Prediction Engine

📊 Interactive Distribution Visualizations

🌎 Real-Time Tree Analytics

💡 Streamlit Web Interface for seamless UX

🚀 Get Started Quickly
🧰 Requirements
Python 3.13+

pip package manager

At least 4GB RAM (recommended for model usage)

⚙️ Setup
bash
Copy
Edit
# Clone the repository
git clone https://github.com/SatyamPandey-07/TREE_SPECIES_CLASSIFICATION.git
cd TREE_SPECIES_CLASSIFICATION

# Install dependencies
pip install -r requirements.txt
▶️ Launch the App
bash
Copy
Edit
streamlit run streamlit_integrated.py
Visit http://localhost:8501 in your browser.

🧠 AI Models & Tech Stack
🗺️ Location Recommender (KNN)
Input: [Latitude, Longitude, Diameter, Native, City, State]

Model: K-Nearest Neighbors using geospatial clustering

Output: Top 5 most likely tree species in that area

🧠 CNN Image Classifier
Architecture: Conv2D layers → MaxPooling → Dropout → Dense

Input: 224×224 tree image

Output: Species name with confidence score

Accuracy: ~26% (real-world dataset, 1.4K+ images)

🧪 Tools Used
TensorFlow, Keras, scikit-learn, Pandas, NumPy, Joblib

Streamlit for web UI

ImageDataGenerator for augmentation

🗃️ Dataset Overview
🌳 Tree Metadata
Source: 50+ U.S. city tree inventories

Size: 1.38 million trees

Features: Species name, GPS, native flag, DBH, city/state

🖼️ Image Dataset
Classes: 30 common North American species

Images: 1,454 (augmented)

Format: Folder-per-species

Resolution: 224x224 RGB

📁 Project Layout
bash
Copy
Edit
TREE_SPECIES_CLASSIFICATION/
├── streamlit_integrated.py       # Main app
├── requirements.txt              # Python packages
├── tree_CNN.ipynb                # CNN training notebook
├── 5M_trees.ipynb                # Location model training
├── models/
│   ├── basic_cnn_tree_species.h5
│   ├── nn_model.joblib
│   ├── scaler.joblib
│   └── tree_data.pkl
└── docs/
    ├── performance_metrics.png
    └── cnn_architecture.png
🎮 How to Use
🧭 1. Predict via Location
Enter:

Latitude & Longitude

Diameter at Breast Height (DBH)

Native status

City & State

💡 You'll receive top 5 species with confidence.

📷 2. Classify Image
Upload:

A tree image (leaf, bark, full tree)

🧠 App returns:

Top 3 predicted species

Associated probabilities

🌍 3. Explore Species Distribution
Search for a species to visualize:

Geographic spread

City-wise occurrence

📉 Model Performance Snapshot
Model	Accuracy	Notes
CNN Classifier	~26%	Real-world, low-data setup
KNN Recommender	N/A	Fast lookup, non-probabilistic

🛠 Deployment Options
💻 Run Locally
bash
Copy
Edit
streamlit run streamlit_integrated.py
🐳 Docker
dockerfile
Copy
Edit
FROM python:3.13
COPY . /app
WORKDIR /app
RUN pip install -r requirements.txt
CMD ["streamlit", "run", "streamlit_integrated.py"]
🤝 Want to Contribute?
We welcome contributions of all kinds! Here's how:

Fork the repo

Create a branch: git checkout -b my-feature

Make changes and commit: git commit -am 'Add new feature'

Push: git push origin my-feature

Open a pull request!

✅ Add unit tests and update docs if relevant.

📜 License
Licensed under the MIT License.
See LICENSE for details.

📬 Contact & Support
Author: Satyam Pandey
Project Repo: TREE_SPECIES_CLASSIFICATION

Have a question, bug report, or feature idea?
Open an issue or start a discussion.

🌱 Acknowledgments
City Tree Inventories from U.S. municipalities

TensorFlow & Streamlit communities

Open-source botanical image datasets

<div align="center">
⭐ If you like this project, give it a star and share!
🌳 Built to promote smarter, greener urban spaces.

</div>
Let me know if you’d like this turned into a .md file or need a version tailored for GitHub Pages!
