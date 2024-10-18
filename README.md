# Fraud Detection with GANs / Betrugserkennung mit GANs

## Projektübersicht / Project Overview

### Deutsch:
Dieses Projekt zielt darauf ab, betrügerische Transaktionen mithilfe von **Generativen Adversarialen Netzwerken (GANs)** zu erkennen. Ein Datensatz mit Kreditkartentransaktionen, der sowohl normale als auch betrügerische Transaktionen enthält, wird verwendet, um ein **GAN-basiertes Modell** für die Anomalieerkennung zu entwickeln. Das Modell lernt, synthetische Transaktionsdaten zu generieren, die dann mit echten Transaktionen verglichen werden, um potenzielle Betrugsfälle zu identifizieren.

Der Arbeitsablauf umfasst:
1. **Datenvorverarbeitung:** Bereinigung und Normalisierung der Kreditkartentransaktionsdaten.
2. **Modellierung mit GANs:** Implementierung eines Generators und eines Diskriminators, um Muster in den Transaktionsdaten zu erlernen.
3. **Anomalieerkennung:** Generierung synthetischer Transaktionen und Vergleich mit realen Daten zur Identifikation von Anomalien (möglicher Betrug).
4. **Bewertung:** Beurteilung der Modellleistung durch Vergleich der erkannten Anomalien mit bekannten Betrugslabels.

Dieses Projekt zeigt, wie GANs auf ein bedeutendes realweltliches Problem angewendet werden können: **Betrugserkennung** bei Finanztransaktionen.

---

### English:
This project aims to detect fraudulent transactions using **Generative Adversarial Networks (GANs)**. A dataset containing credit card transactions, including both normal and fraudulent transactions, is used to build a **GAN-based model** for anomaly detection. The model learns to generate synthetic transaction data, which is then compared with real transactions to identify potential fraud.

The workflow includes:
1. **Data Preprocessing:** Cleaning and normalizing the credit card transaction data.
2. **Modeling with GANs:** Implementing a Generator and a Discriminator to learn patterns in the transaction data.
3. **Anomaly Detection:** Generating synthetic transactions and comparing them to real data to identify anomalies (potential fraud).
4. **Evaluation:** Assessing the model's performance by comparing detected anomalies with known fraud labels.

This project demonstrates how GANs can be applied to an important real-world problem: **fraud detection** in financial transactions.

---

## Wichtige Merkmale / Key Features:
- **Daten Normalisierung:** Standardisierung der Transaktionsdaten für ein effektives Training.  
- **GAN Architektur:** Eigenständige Implementierung von Generator- und Diskriminator-Netzwerken.  
- **Anomalieerkennung:** Identifikation potenziellen Betrugs durch Vergleich von echten und generierten Transaktionsdaten.  
- **Leistungsüberwachung:** Training des Modells über 30.000 Epochen zur Verbesserung der Erkennungsgenauigkeit.  

- **Data Normalization:** Standardization of transaction data for effective training.  
- **GAN Architecture:** Custom-built Generator and Discriminator networks.  
- **Anomaly Detection:** Identifying potential fraud by comparing real and generated transaction data.  
- **Performance Monitoring:** Training the model over 30,000 epochs to improve detection accuracy.  

---

## Verzeichnisstruktur / File and Directory Structure:
- `creditcard.csv`: Der originale Datensatz der Kreditkartentransaktionen. / The original dataset of credit card transactions.  
- `transactions.db`: SQLite-Datenbank, die die Transaktionsdaten speichert. / SQLite database storing the transaction data.  
- `fraud_detection_gan.ipynb`: Jupyter Notebook, das das GAN-Training und die Anomalieerkennung umfasst. / Jupyter notebook containing the GAN training and anomaly detection pipeline.  
- `README.md`: Dokumentation des Projekts. / Documentation of the project.  

---

## Technologien / Technologies Used:
- **Python**
- **PyTorch** (für die Erstellung von GANs / for building GANs)
- **SQLite** (für die Speicherung der Transaktionsdaten / for storing transaction data)
- **Pandas** (für Datenmanipulation / for data manipulation)
- **Matplotlib** (für die Visualisierung des Trainingsverlaufs / for visualizing the training losses)
