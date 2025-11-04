# network_anamoly1
Machine Learning–based Network Anomaly Detection System using Isolation Forest to identify malicious traffic in real-time.
# 🧠 Network Anomaly Detection using Machine Learning

A lightweight Machine Learning project for detecting **network anomalies** and **suspicious traffic** in real time using the **Isolation Forest algorithm**.

---

## 🚀 Features
- ⚡ Detects unusual network behavior automatically  
- 🧩 Uses **Isolation Forest** for unsupervised anomaly detection  
- 📊 Supports live or static network data analysis  
- 💾 Trained model stored as `.pkl` for quick re-use  
- 🔍 Identifies “Normal” vs “Anomaly” connections  

---

## 🧰 Tech Stack
- **Python 3.10+**
- **Scikit-learn**
- **Pandas**
- **NumPy**
- **Joblib**

---

## 🧠 How It Works
1. Load and preprocess network traffic data (CSV)
2. Encode categorical features (`protocol`, `service`, etc.)
3. Train the **Isolation Forest** model on normal + mixed data
4. Save the model (`iforest_model.pkl`)
5. Run `live_monitor.py` to classify new connections in real-time

---

## 🧑‍💻 Usage
```bash
# Clone the repo
git clone https://github.com/<your-username>/network-anomaly-detection.git
cd network-anomaly-detection

# Create virtual environment
python -m venv .venv
.venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Train model
python train_iforest_fixed.py

# Monitor live data
python live_monitor.py
