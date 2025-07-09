# Knee Osteoarthritis Grading Using X-ray Images (ResNet)

This project applies deep learning to grade the severity of **Knee Osteoarthritis (OA)** using X-ray images. It uses a **pretrained ResNet50 model** as a feature extractor and classifies images into 5 grades (KL-0 to KL-4).

## 📂 Dataset
- Digital Knee X-ray Images Dataset (from Kaggle)
- Includes expert-graded severity levels

## 📊 Grades:
- 0: Normal
- 1: Doubtful
- 2: Mild
- 3: Moderate
- 4: Severe

## 🧠 Model Architecture
- Pretrained **ResNet50 (ImageNet)**
- GlobalAveragePooling → Dense → Dropout → Softmax
- Transfer Learning + Fine Tuning

## 🔧 Steps:
1. Load and preprocess images
2. Normalize and apply ResNet-specific preprocessing
3. Train/validation/test split with stratification
4. Train model using frozen base
5. Fine-tune and evaluate performance

## 📈 Results
- Accuracy: ~XX% (to be updated after training)
- Evaluation: Confusion matrix, Precision, Recall

## 🚀 Future Improvements
- Use EfficientNet for better accuracy
- Integrate Grad-CAM for explainability
- Build Gradio demo for deployment

## 🧪 Requirements
```bash
pip install -r requirements.txt
