(Refer to the ZIP archive for the normal project files. It includes both macOS-generated metadata files (e.g., __MACOSX folders) and the actual project files.)

# 🧁 Sweeter-Native

**A project for the 418 Hackathon — hosted by Enigma, under AEON 2025**

> This is a zip folder containing the normal files and the macosx files. Follow the instruction in the readme to run a streamlit app. Do download the requirements and set up a .env file with a hugging face api key for the second page of the app to respond.

## 🚨 The Problem

Sugar is everywhere — and that's the problem.

Linked to obesity, diabetes, heart disease, and countless chronic conditions, refined sugar is under increasing scrutiny. But the alternatives? They're not perfect either:

- 🌱 **Natural sweeteners** (like stevia or erythritol) may be healthier — but don't always work across recipes or taste profiles
- 🧪 **Ingredient interactions** can distort flavor, texture, or aroma when sweeteners are substituted
- 🔬 In R&D, it's impossible to physically test every sweetener in every food matrix
- 🏭 Manufacturers waste time and money trialing formulations with uncertain outcomes

👨‍🍳 Consumers want healthy.  
🏢 Industry wants efficiency.  
🔬 Science wants precision.

Until now, there's been no tool that brings it all together.

## ✅ The Solution: Sweeter-Native, powered by SweetPredict

A breakthrough AI platform that combines molecular modeling, taste prediction, and dietary context to recommend the best sugar alternatives — personalized for any user, recipe, or product.

Whether you're a home cook, food technologist, or R&D scientist, this tool helps you build smarter, healthier, tastier foods — faster.

## 🧠 What Makes It Different?

### 🧬 Molecular-Level Predictions

We analyze sweeteners based on their chemical structure (SMILES) and use ML models to predict:
- Sweetness Index
- Aftertaste Score

**Models**: Random Forest (for sweetness) + CNN (for flavor/aftertaste)

### 🤖 LLM-Powered Recommendation Engine

Our agentic AI framework factors in:
- Full recipe & ingredient context
- User health conditions or goals
- Flavor interactions between molecules
- Scientific sweetener rankings & constraints

### 🧪 A Tool for Everyone

This isn't just a consumer gadget — it's a science-backed toolkit for:
- 🏭 Manufacturers optimizing sugar-free formulations
- 🧪 R&D labs accelerating food product development
- 🍽 Nutrition startups building personalized food experiences
- 🧑‍⚕ Dietitians crafting smarter health recommendations

 (https://github.com/user-attachments/assets/d5bda737-e8a9-4db8-8654-690c23173957)


## 🚀 Quick Start Guide

### 1️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 2️⃣ Generate Molecular Data

```bash
python generate-csv.py
```

Processes sweetener structures and outputs `sweetness.csv` + `flavor.csv`

### 3️⃣ Train the Models

```bash
python sweetness_train.py    # Random Forest for sweetness
python cnn_train.py          # CNN for flavor/aftertaste
```

### 4️⃣ Launch the App

```bash
streamlit run app.py
```

### 5️⃣ Set Up Environment

Create a `.env` file in the root directory with your Hugging Face API key:

```bash
echo "HUGGINGFACE_API_KEY=your_api_key_here" > .env
```

## 🌐 App Features

### 🔍 Page 1 – Molecular Sweetness Predictor

- Input any SMILES string
- Get instant ML-based predictions:
  - Sweetness score
  - Aftertaste score
  - Model visualizations

### 🎯 Page 2 – AI Sweetener Recommender

A smart, LLM-powered agent that:
- Analyzes recipes & ingredients
- Factors in user dietary needs
- Evaluates and compares sweeteners
- Models flavor interactions
- Recommends the best sweetener or combo
- Justifies choices with scientific reasoning
- Suggests where to buy (Amazon, iHerb, etc.)

## 🧪 Scientifically Ranked Sweeteners

| Rank | Sweetener | Health Value | Highlights |
|------|-----------|--------------|------------|
| 1 | Allulose | ⭐⭐⭐⭐⭐ | Natural, metabolically safe |
| 2 | Yacon Syrup | ⭐⭐⭐⭐ | Gut-friendly, prebiotic |
| 3 | Stevia | ⭐⭐⭐⭐ | Natural, calorie-free |
| 4 | Erythritol | ⭐⭐⭐⭐ | Low-calorie, widely accepted |
| 5 | Xylitol | ⭐⭐⭐ | Dental benefits, mildly sweet |
| 6 | Coconut Sugar | ⭐⭐ | Low GI, good for baking |
| 7 | Date Sugar | ⭐⭐ | Whole-food sweetness |
| 8 | Pomegranate Mol. | ⭐⭐ | Tart, functional, nutrient-rich |

## 💡 Why This Is Unique

Other tools recommend sweeteners.  
**We predict, simulate, and recommend — using real science.**

We combine:
- 🔬 Molecular analysis
- 🧠 ML-driven sweetness prediction
- 🤖 LLMs for ingredient reasoning
- 📊 Real-time dietary customization

We're not just replacing sugar —  
We're reimagining the intersection of food science, AI, and wellness.

**Sweeter-Native can be your AI co-pilot for healthier, tastier innovation.**

