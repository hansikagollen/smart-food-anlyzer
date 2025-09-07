# AI-Powered Freshness Detection for Fruits and Vegetables

## Project Overview
Reducing food waste and promoting healthy eating require accurate, real-time assessment of fruit and vegetable quality. This project presents an AI-powered end-to-end system that detects freshness, estimates calories and nutrient content, and delivers the results via a user-friendly application. Freshness is analyzed using a hybrid CNN–BiLSTM model, where CNN extracts spatial features from images and Bi-LSTM captures temporal or multi-view variations, enabling classification into fresh, semi-fresh, or spoiled categories. For nutritional estimation, YOLOv5 detects and segments individual fruits and vegetables, which are then mapped to an external database (e.g., USDA FoodData Central) to calculate calorie and nutrient content. The system is integrated into an application that allows users to capture images of produce and instantly receive freshness status and nutritional information. This project combines deep learning, object detection, database mapping, and real-world deployment, offering a novel and practical solution for consumers, retailers, and the food supply chain.To enhance the practicality of our food freshness detection system, we extended it beyond simple classification into a more valuable application: shelf-life prediction. While detecting whether a fruit is fresh, semi-fresh, or rotten is useful, real-world stakeholders such as retailers, farmers, and consumers often need to know how many days remain before the produce becomes unusable. To address this, we mapped each freshness class to an estimated number of days left, based on the typical shelf life of different fruits and vegetables at room temperature. For example, a fresh apple may have around 20 days remaining, while a semi-rotten apple may only have 7 days left, and a rotten one is considered expired with 0 days.


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


