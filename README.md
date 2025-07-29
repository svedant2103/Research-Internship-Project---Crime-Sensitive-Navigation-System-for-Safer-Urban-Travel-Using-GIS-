# Research-Internship-Project---Crime-Sensitive-Navigation-System-for-Safer-Urban-Travel-Using-GIS-
A smart navigation system that integrates real crime data to highlight high-risk areas, assign safety scores to road segments, and compute both shortest and safest routes using graph algorithms. Users can view interactive city maps to choose routes based on safety and distance preferences.

cat << 'EOF' > README.md
# Crime-Sensitive Navigation System for Safer Urban Travel

A smart urban navigation system that integrates real-world crime data to recommend not just the shortest but also the safest routes for users. It maps crime-prone zones, assigns risk scores to road segments, and uses graph-based algorithms to suggest alternate paths that minimize personal safety risks.

---

## Table of Contents

- [About the Project](#about-the-project)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Dataset](#dataset)
- [How It Works](#how-it-works)
- [Model Performance](#model-performance)
- [Installation](#installation)
- [Visualizations](#visualizations)
- [Future Scope](#future-scope)
- [Author](#author)
- [License](#license)

---

## About the Project

With rising urban crime rates, traditional navigation systems fail to consider public safety while recommending routes. This project bridges that gap by integrating crime analytics into the pathfinding process. The system uses real crime data, geospatial analysis, and graph algorithms to recommend both shortest and safest routes for urban travelers.

---

## Features

- 📍 Maps real-time crime-prone zones using public datasets
- 📊 Assigns risk scores to each road segment
- 🧭 Calculates both shortest and safest paths using Dijkstra’s algorithm
- 🌐 Interactive map visualization using Folium
- 🧠 Trained machine learning models to classify risk zones
- ⚠️ Highlights high-risk areas in red; safest routes in green

---

## Tech Stack

| Category        | Tools & Libraries                        |
|---------------- |------------------------------------------|
| Language        | Python                                   |
| Data Handling   | Pandas, NumPy                            |
| ML Models       | Scikit-learn, XGBoost, LightGBM, MLP     |
| GIS Mapping     | Folium, Leaflet.js                       |
| Graph Algorithms| NetworkX, OSMnx                          |
| Visualization   | Matplotlib, Seaborn                      |

---

## 📂 Dataset

- 📌 [Indian Crimes Dataset (Kaggle)](https://www.kaggle.com/datasets/sudhanvahg/indian-crimes-dataset)
- Contains over 40,000+ entries with:
  - City, Type of Crime, Severity Score, Victim Age
  - Latitude/Longitude, Time of Occurrence, Police Deployed

---

## ⚙️ How It Works

1. **Data Collection & Cleaning**: Crime data is collected, cleaned, and geo-tagged.
2. **Feature Engineering**: Risk scores are calculated using severity, time, victim age, etc.
3. **Map Visualization**: Crime zones are plotted using Folium heatmaps.
4. **Road Graph Creation**: Road networks are built with OSMnx.
5. **Pathfinding**: 
   - Shortest route → based on physical distance
   - Safest route → avoids high-risk zones using crime scores
6. **Interactive Output**: Users can compare shortest vs safest paths visually.

---

## Model Performance

| Model                | Mean Accuracy |
|----------------------|---------------|
| XGBoost Classifier   | 99%           |
| LightGBM Classifier  | 99%           |
| MLP Classifier       | 98%           |
| Logistic Regression  | 98%           |
| Support Vector       | 96%           |

---

## 🧪 Installation

```bash
git clone https://github.com/svedant2103/Crime-Sensitive-Navigation.git
cd Crime-Sensitive-Navigation
pip install -r requirements.txt

🌍 Visualizations
1. Red markers: Crime hotspots

2. Green line: Safest path (avoids crime zones)

3. Red dashed line: Shortest path (ignores safety)

4. Popups: Show city, severity, and risk score info

🔮 Future Scope
1. Real-time crime data from APIs or police databases

2. Multi-modal navigation (pedestrian, vehicle, public transport)

3. LLM-based feedback integration for user-submitted alerts

5. Mobile or web-based deployment

6. Multilingual and offline support for remote users

👨‍💻 Author
Vedant Singh
B.Tech IT, III Year
IIIT Sonepat
📧 svedant2103@gmail.com

📄 License
This project was developed during a summer internship at MNNIT Allahabad under the mentorship of Prof. D.S. Kushwaha, and is released for educational and non-commercial use only.

EOF

---

### ✅ How to Use

1. Open your terminal in the root of the project directory
2. Paste the entire command above and hit **Enter**
3. This will generate a clean, fully formatted `README.md` file
