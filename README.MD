# **Keystroke AI: Typing Patterns for User ID**  
A machine learning project for user identification based on keystroke dynamics using a Multi-Layer Perceptron (MLP).

## **Project Overview**  
This project aims to identify users based on their unique typing patterns. Using keystroke dynamics, we extract features from typing logs and train an MLP model to classify users. The dataset consists of keystroke data collected from different devices (desktop, phone, and tablet). The project includes preprocessing, feature extraction, model training, and evaluation.

## **Dataset**  
The project contains three datasets:  
- `combined_desktop_data.csv` – Keystroke data collected from desktop users.  
- `combined_phone_data.csv` – Keystroke data collected from phone users.  
- `combined_tablet_data.csv` – Keystroke data collected from tablet users.  

Each dataset includes key press timings, and we extract features such as the average and standard deviation of key hold times for specific keys ("t", "a", "e", "i", "h").

## **Models**  
Each device has its own MLP model for user identification:  
- `desktop_model.ipynb` – Model training and evaluation for desktop users.  
- `phone_model.ipynb` – Model training and evaluation for phone users.  
- `tablet_model.ipynb` – Model training and evaluation for tablet users.  

Each model follows these specifications:
- Input size: **10** (mean and standard deviation for 5 keys)
- Output size: **10** (10 user classes)
- Hidden layers: **2 to 4 layers with 5-10 neurons each**
- Training: **100 epochs minimum**
- Evaluation: **3-fold cross-validation**
- Metrics: **Accuracy, loss curves, and validation performance**

## **Report**  
- `Report.pdf` contains the findings, accuracy results, and performance metrics for the trained models.

