# 🛍 AI Shopping Assistant

## 📖 Introduction

AI Shopping Assistant is an intelligent Flask-based web application that uses Artificial Intelligence to identify products from uploaded images and search for similar products online.

The system combines:

- AI Image Captioning
- Product Recommendation
- Semantic Similarity Matching
- Scam Risk Analysis

to provide smart shopping suggestions and best-buy recommendations.

The application allows users to upload an image of a product, automatically analyze it using AI models, search online marketplaces, and display matching products with risk analysis.

---

# 🎯 Project Objectives

The main objectives of this project are:

- Detect and identify products from images
- Generate AI-based captions using BLIP
- Search online products automatically
- Compare product similarity using embeddings
- Detect possible scam risks
- Recommend the best available product
- Build an AI-powered shopping assistant

---

# 🛠 Technologies Used

| Technology | Purpose |
|------------|----------|
| Python | Backend programming |
| Flask | Web framework |
| Transformers | BLIP image captioning |
| Sentence Transformers | Semantic similarity |
| Pillow (PIL) | Image processing |
| SerpAPI | Google product search |
| HTML/CSS | Frontend UI |
| JavaScript | Dynamic frontend behavior |

---

# 🧠 AI Models Used

## BLIP Image Captioning Model

```python
Salesforce/blip-image-captioning-large

Used for:

Detecting products from uploaded images
Generating natural language captions
Sentence Transformer Model
all-MiniLM-L6-v2

Used for:

Semantic similarity matching
Product comparison
Match score calculation
📂 Project Structure
AI-Shopping-Assistant/
│
├── app.py
├── requirements.txt
├── README.md
│
├── uploads/
│
└── assets/
⚙️ System Workflow

The application works in the following steps:

User uploads a product image
BLIP model generates image caption
Keywords are extracted
SerpAPI searches online products
Semantic similarity is calculated
Scam risk percentage is estimated
Best product recommendation is shown
🔍 Features
AI-based product recognition
Product caption generation
Online product searching
Amazon & Daraz product search
Match score calculation
Scam risk detection
Best buy recommendation
Responsive web interface
Automatic image analysis
🖼 Image Captioning System

The uploaded image is processed using BLIP.

Example:

"a black wireless gaming mouse on a desk"

This caption is used to search products online.

🛒 Product Search System

The application searches products using:

Amazon
Daraz

through SerpAPI.

Search query example:

black wireless gaming mouse site:amazon.com OR site:daraz.pk
📊 Semantic Similarity Matching

The system compares:

AI-generated image caption
Product titles from search results

using Sentence Transformers.

This generates:

Match score
Product relevance
⚠ Scam Risk Detection

The application estimates scam risk based on similarity score.

Match Score	Scam Risk
High Match	10%
Low Match	30%

This helps users identify safer products.

✅ Best Buy Recommendation

The system automatically selects:

Lowest scam risk
Best matching product

and recommends it as the best buying option.

🎨 User Interface Features

The UI includes:

Clean modern layout
Product listing section
AI-generated captions
Keyword display
Best buy recommendation area
Upload image functionality
🚀 Installation Guide
Step 1 — Clone Repository
git clone https://github.com/your-username/AI-Shopping-Assistant.git
Step 2 — Open Project Folder
cd AI-Shopping-Assistant
Step 3 — Install Dependencies
pip install -r requirements.txt
🔑 Setup SerpAPI Key

Replace:

SERP_API_KEY = "YOUR_SERP_API_KEY"

with your real SerpAPI key.

Get API key from:

https://serpapi.com/

▶️ Run Application
python app.py
🌐 Application URL

After running:

http://127.0.0.1:5000/
📦 Requirements
flask
pillow
transformers
sentence-transformers
requests
nest_asyncio
torch
📸 Example Workflow
Input

User uploads:

Wireless Gaming Mouse Image
AI Output

Generated Caption:

black wireless gaming mouse
Search Results
Amazon products
Daraz products
Match scores
Scam risk analysis
