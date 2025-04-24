# 🌾 Farmer Guider – Smart Crop Recommendation System

**Farmer Guider** is a machine learning-powered web application that helps farmers choose the most suitable crop to plant based on real-time soil and environmental parameters like Nitrogen, Phosphorus, Potassium, temperature, humidity, pH, and rainfall. 

🚜 Designed to support better agricultural decisions and boost crop yield through data-driven intelligence.

---

## 🧠 Project Highlights

- 📊 Uses **KMeans Clustering** to recommend crops based on grouped environmental conditions.
- 🧪 **Preprocessing & Scaling** with `StandardScaler` to normalize input data.
- 🔄 **User-friendly Web Interface** built using **Flask** and HTML/CSS.
- 🗃️ Local **SQLite Database** to store user inputs and prediction results.
- 🎨 Aesthetic design with images, GIFs, and multiple CSS stylesheets.

---

## 🚀 How It Works

1. User inputs values like temperature, humidity, NPK levels, etc.
2. Data is preprocessed using a saved `StandardScaler`.
3. The `KMeans` model identifies the closest cluster.
4. Based on the cluster, the system recommends the best-suited crop.
5. Inputs and results are saved in a local database (`form_data.db`).

---

## 🛠️ Tech Stack

| Layer       | Technologies Used                |
|-------------|----------------------------------|
| **Frontend**| HTML, CSS, GIFs, Static Assets   |
| **Backend** | Python, Flask                    |
| **ML Model**| Scikit-learn (KMeans, Scaler)    |
| **Database**| SQLite (`form_data.db`)          |
| **Others**  | Pandas, NumPy, Joblib            |

---

## 📂 Project Structure

```bash
Farmer-Guider/
├── models/                  # Trained model & scaler
│   ├── filtering_data.csv
│   ├── kmeans_model.lb
│   └── standardscaler.lb
├── static/                  # UI assets
│   ├── images/
│   ├── background.jpg
│   ├── styles.css
│   ├── styles2.css
│   └── styles3.css
├── templates/               # HTML templates
│   ├── home.html
│   ├── output.html
│   ├── project.html
│   └── weather-natue.gif
├── app.py                   # Flask app (main backend logic)
├── farmer_guider.ipynb      # Model training and EDA notebook
├── farmer.csv               # Raw dataset
├── farmerdata.py            # Helper Python file
├── form_data.db             # Local database
└── README.md                # This file

🔧 Local Setup & Installation
🐍 Requirements
Python 3.8+

pip (Python Package Manager)

🛠️ Steps

# Clone the repo
git clone https://github.com/Abhishek-Sharma-i/Farmer-Guider.git
cd Farmer-Guider

# Install dependencies
pip install -r requirements.txt

# Run the application
python app.py
Visit http://127.0.0.1:5000 in your browser to use the app.


💡 Future Scope
🌦️ Integrate real-time weather APIs

📱 Make it mobile-responsive

🗣️ Multi-language support for local farmers

🤖 Upgrade to classification models for higher accuracy

📊 Add dashboards for trend analysis & insights


👨‍💻 Developed By
Abhishek Sharma
Data Science Enthusiast | Developer | B.Tech Student

🔗 LinkedIn
📬 https://www.linkedin.com/in/abhishek-sharma-tech/

📄 License
This project is open-sourced under the MIT License.
