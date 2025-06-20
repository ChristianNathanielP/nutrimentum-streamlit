# 🍱 Nutrimentum — Your AI-Powered Indonesian Nutrition Companion

Nutrimentum is a machine learning–based platform that helps Indonesians make healthier food choices in a simple and personalized way.

Just take a photo of your meal to instantly identify the dish and reveal detailed nutrition facts such as calories, protein, carbohydrates, and fat, all tailored for authentic Indonesian cuisine.

Whether you're aiming to lose weight, build muscle, boost your energy, or strengthen immunity, Nutrimentum gives you personalized food recommendations aligned with your health goals and taste preferences.

---

## 📸 Main Features

### 🥗 Nutri Guide
Nutri Guide offers a personalized recommendation system to support your health goals through two smart approaches:

1. **Goal-Based Recommendation**  
   Get food suggestions that align with your primary health objective such as weight loss, muscle development, energy boost, heart health, or immunity support.

2. **Content-Based Filtering (Nutrient Similarity)**  
   Discover alternative foods with similar nutritional profiles to the ones you already eat — great for maintaining variety without sacrificing your goals.

**How to Use:**  
- Choose your primary health goal or a food you often eat.  
- Get a list of personalized food recommendations based on nutrients or lifestyle goals.

### 📸 Snap Nutri
Snap Nutri lets you recognize your meal and instantly reveal its nutritional value using image classification. Trained on 23 popular Indonesian dishes, this feature is ideal for quick insights.

**How to Use:**  
1. Take a clear photo of your Indonesian meal.  
2. Upload the image in the app.  
3. View the dish name and its estimated nutritional content (calories, fat, protein, carbs, etc.).

---

## 🧠 Model Info

### Image Classification Model

- **Architecture:** InceptionV3 (transfer learning)
- **Input size:** 299x299 pixels
- **Classes:** 23 Indonesian traditional foods
- **File format:** `.keras` (169 MB)
- **Source:** Downloaded from Hugging Face:  
  [`cnginn/indonesiafoodimageclassification`](https://huggingface.co/cnginn/indonesiafoodimageclassification)

The model is automatically downloaded on first app run. Make sure you're connected to the internet.

### Recommendation System

Two intelligent approaches power the food recommendations:

1. **Goal-Based Recommender**  
   Uses rule-based filtering by matching user health goals (e.g. muscle development, weight loss) with suitable food choices using nutrition data.

2. **Content-Based Filtering**  
   Recommends foods that are nutritionally similar to a selected food based on cosine similarity of macro-nutrient vectors (calories, carbs, protein, fat).

Both systems use `nutrition_data.csv` as their knowledge base.

---