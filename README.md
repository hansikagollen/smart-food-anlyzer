#  Fruit & Vegetable Freshness Detection with Shelf-Life Estimation  

##  Overview  
This project presents an **AI-powered system for detecting freshness levels in fruits and vegetables**, classifying them into three categories:  
-  Fresh  
-  Semi-Rotten (Intermediate stage)  
-  Rotten  

Unlike conventional systems that only provide **binary outputs (fresh/rotten)**, our model introduces an **intermediate freshness stage** and also provides an approximate **shelf-life estimation (days until spoiled)**.  

The approach combines **deep learning (CNN/EfficientNet/YOLO)** with **heuristic preprocessing (color fading, brown-spot, and texture analysis)** to build a robust multi-class classification system. When datasets lack intermediate labels, semi-rotten categories are created using **image augmentation + heuristics**.  

---

##  Features  
-  Upload/capture images of fruits or vegetables for quality check.  
-  Multi-class classification: Fresh / Semi-Rotten / Rotten.  
-  Shelf-life estimation (remaining days).  
-  Confidence score visualization for interpretability.  
-  Edge-AI deployment for smartphones (real-time detection on-device).  
-  Optional **nutritional value mapping** using USDA FoodData Central API.  

---

##  Tech Stack  
- **Deep Learning Frameworks**: TensorFlow / PyTorch  
- **Models**: EfficientNet / DenseNet / MobileNet 
- **Computer Vision**: OpenCV (spot detection, texture analysis)  
- **Backend**: Flask / FastAPI / Streamlit  
- **Deployment**: Mobile/Edge AI with TensorFlow Lite / ONNX  
- **Dataset Sources**: Kaggle, GitHub (fruits & vegetables at different decay stages)  

---

##  Dataset  
- Multiple Kaggle & GitHub datasets of fruits and vegetables .  
- Unified into **3 classes**: Fresh, Semi-Rotten, Rotten.  
- Semi-Rotten class generated using:  
  - Color/texture heuristics (spot/brown fade detection).  
  - Image augmentation (blurring, contrast reduction, partial decay synthesis).  

---

##  Applications  
-  **Consumers**: Detect quality before eating.  
-  **Retailers**: Monitor inventory freshness to reduce waste.  
-  **Supply Chain**: Predict shelf life during storage/transport.  
-  **Healthcare**: Prevent consumption of harmful spoiled produce.  

