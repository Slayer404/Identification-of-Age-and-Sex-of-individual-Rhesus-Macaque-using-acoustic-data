# 🐒 Identification of Age-Sex Individual of Rhesus Macaque (Macaca mulatta) Based on Acoustic Data

This project is a final-year B.Tech dissertation developed by **Sasanka Barman** under the guidance of **Dr. Lachit Dutta**, as part of the **Department of Electronics and Communication Engineering**, **Gauhati University**.

---

## 📌 Abstract

This research focuses on automated recognition of Rhesus Macaque vocalizations to identify **age** and **sex** groups using machine learning. By transforming audio signals into **Mel spectrograms**, we trained **Convolutional Neural Networks (CNNs)** and **Long Short-Term Memory (LSTM)** networks to classify audio into five distinct categories:

- Adult Male  
- Adult Female  
- Infant  
- Juvenile    

Both models were evaluated using real-world bioacoustic datasets, showing that CNNs outperform LSTMs in recognizing adult vocalizations, while LSTMs performed well on juvenile and infant classes.

---

## 🎯 Objectives

- Develop an automated sound recognition system.
- Classify animal audio based on age and sex.
- Compare performance between CNN and LSTM models.
- Contribute to real-time biodiversity monitoring and conservation efforts.

---

## 🛠️ Tools & Technologies

- **Python**
- **TensorFlow / Keras**
- **Librosa** (for audio preprocessing)
- **Google Colab** (GPU training)

---

## 🧠 Methodology

### 🔹 CNN Approach:
- Input: Mel Spectrograms (128×128)
- Architecture:
  - Conv Layers: 32 and 64 filters
  - Pooling + Dropout
  - Dense: 512 → 256
  - Output: Softmax (5 classes)

### 🔹 LSTM Approach:
- Input: MFCC Sequences (T×40)
- Architecture:
  - Stacked LSTM: 128 + 64 units
  - Dense: 256 → 128
  - Output: Softmax (5 classes)

---

## 📊 Results

| Test Case     | CNN Accuracy | LSTM Accuracy |
|---------------|--------------|----------------|
| Adult Male    | 100%         | ❌ Misclassified |
| Adult Female  | 95.1%        | ❌ Misclassified |
| Infant        | 98.5%        | ✅ 99.9%       |
| Juvenile      | 100%         | ✅ 100%        |

- CNN excels at spatial pattern recognition in spectrograms.
- LSTM captures temporal sequences better but struggles with similar adult vocalizations.

---

## 🚀 Future Scope

- Build a **real-time IoT-enabled device** for wildlife monitoring.
- Implement a **hybrid CNN-LSTM model**.
- Integrate **MEMS microphones**, **LoRa/Wi-Fi modules**, and **low-power processors**.
- Expand datasets for better generalization.
- Apply **adaptive noise filtering** for field deployment.

---

## 🌍 Applications

- **Wildlife Conservation** (real-time species detection)
- **Biodiversity Monitoring**
- **Human-Wildlife Conflict Prevention**
- **Ecological Trend Analysis**

---

## 🧾 Citation

> Barman, S., & Das, H. (2025). *Identification of Age-Sex Individual of Rhesus Macaque (Macaca mulatta) Based on Acoustic Data*. Gauhati University, Dept. of ECE.

---

## 📬 Contact

- **Sasanka Barman** – [LinkedIn](https://www.linkedin.com/in/sasanka-barman-a58027226)
- **Email** – sasankabarman2016@gmail.com

---

> _"By understanding their voice, we help protect their world."_

