# AI-Powered Freshness Detection for Fruits and Vegetables

## Project Overview
Reducing food waste and promoting healthy eating require accurate, real-time assessment of fruit and vegetable quality. This project presents an AI-powered end-to-end system that detects freshness, estimates calories and nutrient content, and delivers the results via a user-friendly application. Freshness is analyzed using a hybrid CNN–BiLSTM model, where CNN extracts spatial features from images and Bi-LSTM captures temporal or multi-view variations, enabling classification into fresh, semi-fresh, or spoiled categories. For nutritional estimation, YOLOv5 detects and segments individual fruits and vegetables, which are then mapped to an external database (e.g., USDA FoodData Central) to calculate calorie and nutrient content. The system is integrated into an application that allows users to capture images of produce and instantly receive freshness status and nutritional information. This project combines deep learning, object detection, database mapping, and real-world deployment, offering a novel and practical solution for consumers, retailers, and the food supply chain.


## Features
- Automatic classification of fruits and vegetables into freshness categories.
- Hybrid **CNN + Bi-LSTM** model for spatial and temporal feature analysis.
- Support for **multi-view and time-lapse datasets**.
- Robust and scalable solution for real-world applications in retail, supply chain, and home use.
- Use of public datasets like **Fruits-360** and **Kaggle Fresh/Rotten Fruits & Vegetables** for training and evaluation.

## Datasets
- [Fruits-360](https://www.kaggle.com/moltean/fruits)
- [Kaggle Fresh/Rotten Fruits & Vegetables](https://www.kaggle.com/sriramr/fruits-fresh-and-rotten-for-classification)

## Technologies Used
- Python
- TensorFlow / Keras
- OpenCV for image preprocessing
- NumPy, Pandas for data manipulation
- Matplotlib / Seaborn for visualization


