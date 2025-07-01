# AI_Nutrition_Assistant
# 🧠 AI Nutrition Assistant

AI Nutrition Assistant is a smart and interactive tool designed to assist users in identifying food items and retrieving their nutritional information in real-time. Supporting both text input and image recognition, the application provides a convenient and educational way for users to make healthier food choices.

---

## 🎯 Objectives

- Build an intelligent assistant that recognizes food via text or image input.
- Educate users on the nutritional value of everyday food items.
- Promote healthy eating habits by making nutrition data easily accessible.

---

## 📖 Problem Statement

Many people find it challenging to understand the nutritional content of their food. With rising health concerns and busy lifestyles, there's a growing need for a quick, AI-driven solution that:

- Recognizes food visually via images.
- Provides verified nutrition facts without manual searches.
- Supports offline recognition and real-time nutrition retrieval via API.

---

## ⚙️ How It Works

### 🖼️ Image Mode:
1. User uploads a food image.
2. The MobileNetV2 deep learning model predicts the food type.
3. The predicted label is sent to the USDA API.
4. Nutritional data is fetched and displayed.

### 📝 Text Mode:
1. User enters the name of a food item.
2. Nutrition data is fetched directly from the USDA FoodData Central API.

---

## 🌐 Data Source

- **USDA FoodData Central API** – A government-backed database offering reliable, comprehensive nutrient data.
- Provides:
  - Macronutrients: Protein, Carbs, Fats
  - Micronutrients: Vitamins, Minerals, Sodium
  - Standardized food portions and descriptions

---

## 🧪 Use Cases

- 📱 Fitness Apps – Integrate into mobile diet and exercise trackers
- 🧑‍⚕️ Dietitians – Quickly assess clients' food intake
- 🛒 Grocery Assistants – Scan food labels for nutrition data
- 🧑‍🎓 Education – Teach students about AI and food science

---

## 🚧 Limitations and Future Improvements

### ❌ Current Limitations:
- MobileNetV2 may misclassify complex or non-standard food items.
- Internet is required for real-time data via USDA API.
- Only top-5 predictions from the model; not food-specific fine-tuning.

### ✅ Planned Enhancements:
- Train a custom food image classifier using a larger food dataset.
- Add voice input and OCR support (e.g., label scanning).
- Develop Streamlit/web/mobile front-end for user-friendly UX.
- Implement calorie tracking, diet logs, and meal planning.

---

## 💡 Unique Highlights

- Combines Computer Vision and Nutrition Science.
- Uses public health APIs for accurate, real-world data.
- Interactive CLI, easily extendable to web/mobile apps.
- Encourages healthy eating with minimal user input.

---

## 🛠️ Tech Stack

- **Python 3**
- **TensorFlow / Keras (MobileNetV2)**
- **USDA FoodData Central API**
- **NumPy, Requests, Pillow**
- *(Optional)*: Streamlit, SpeechRecognition, OCR (Tesseract), FastAPI

---

## 🏁 Getting Started

### 📦 Installation

```bash
pip install tensorflow numpy requests pillow

Utilizes public health APIs for data accuracy.

Offers an interactive CLI experience, which can be expanded into a web/mobile interface.

Encourages awareness about healthy eating with minimal user input.
