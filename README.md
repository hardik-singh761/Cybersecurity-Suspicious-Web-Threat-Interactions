# 🛡️ Cybersecurity: Suspicious Web Threat Interactions

An AI-powered security analytics project to detect patterns in web traffic logs and identify suspicious or potentially harmful activities using machine learning and deep learning techniques.

## 📌 Project Objective

To analyze structured server logs and model the behavior of web interactions that may signal threats, breaches, or intrusion attempts. This helps in building a proactive threat detection system.

## 🔗 Project Link

👉 [GitHub Repository](https://github.com/hardik-singh761/Cybersecurity-Suspicious-Web-Threat-Interactions)

---

## 📁 Dataset Overview

Custom-labeled AWS CloudWatch web logs containing:

- **src_ip / dst_ip** – Source and destination IPs  
- **bytes_in / bytes_out** – Data volume  
- **protocol, dst_port, response.code**  
- **rule_names / detection_types**  
- **timestamps: creation_time, end_time, event_time**

📂 Shape: 282 rows × 16 columns  
📎 [View Dataset](https://drive.google.com/file/d/1-OpnR9FK8EqGuLFB1k45ctPbl-vuZnC-/view)

---

## 🧹 Workflow

### 1. Data Cleaning
- Cleaned IP formats, timestamps, and structured logs
- Converted categorical detection rules to labels

### 2. Exploratory Data Analysis (EDA)
- Protocol distribution, response codes, IP heatmaps
- Visualized anomalies in traffic and rule triggers

### 3. Feature Engineering
- Built flag-based rule indicators
- Extracted geo-based threat metrics using country codes

### 4. Modeling
- Applied **Deep Learning Binary Classifier** (TensorFlow/Keras)
- Used categorical encoding + normalization

---

## 🛠️ Technologies Used

- Python, Jupyter Notebook
- Pandas, NumPy, Seaborn, Matplotlib
- Scikit-learn, TensorFlow
- Custom rule parsing logic for source.meta analysis

---

## ✅ Model Performance

| Metric     | Score   |
|------------|--------:|
| Accuracy   | 93%     |
| Precision  | 89%     |
| Recall     | 91%     |
| F1 Score   | 90%     |

> ✅ Deep learning outperformed classical models for complex rule detection

---

## 🚀 Future Enhancements

- Deploy model as a REST API using Flask
- Add real-time stream detection via Kafka
- Use GeoIP and WHOIS data for threat intelligence

---

## 🤝 Contributors

- **Hardik Singh**  
  Data Science Intern @ Unified Mentor  
  [GitHub](https://github.com/hardik-singh761)

---

## 📃 License

This project is licensed under the MIT License.
