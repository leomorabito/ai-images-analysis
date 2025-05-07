# 🧠 AI Images Analysis

## 🔍 Project Description

This project uses **AI models** to:
1. Analyze images (`.jpeg` format).
2. Generate a detailed natural language **description** of each image using a **Large Language Model (LLM)** via the **DeepSeek API**.
3. Perform **text analysis** on the image descriptions to:
   - Classify whether the content is **human (male/female)** or **non-human** (e.g., food, animals, objects).
   - Extract additional useful information for research or downstream applications.

The final output is a `.csv` file that contains:
- The image filename.
- A caption/description.
- A predicted category.
- [Optional] Other metadata derived from the text.

---

## 📁 Project Structure
ai-images-analysis/
├── data/
│ └── images/ # JPEG images to be analyzed
├── notebooks/
│ └── image_analysis.ipynb # Main notebook to run the pipeline
├── outputs/
│ └── results.csv # Output with descriptions and classifications
├── .gitignore # Ignoring .env and other temporary files
├── .env # Contains the DeepSeek API key (not committed)
├── README.md # Project documentation
└── requirements.txt # Dependencies



## 🛠️ Setup Instructions

1. **Clone the repository:**

```bash
git clone https://github.com/leomorabito/ai-images-analysis.git
cd ai-images-analysis
```

2. **Create a virtual environment (recommended):**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install Dependenciies:**
```bash
pip install -r requirements.txt
```

## 🚀 Run the Notebook
Open notebooks/image_analysis.ipynb and run all cells.
This will:
1. Generate descriptions using the DeepSeek API.

2. Classify images using text analysis or zero-shot image classification.

3. Save results to outputs/results.csv.

## 📜 License
MIT License 
