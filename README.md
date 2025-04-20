# 🏡 Real Estate Bot

**Deployed at**: [https://huggingface.co/spaces/HarshBhati/Estate](https://huggingface.co/spaces/HarshBhati/Estate)

A smart and user-friendly Gradio app that assists with **property issue detection** through image analysis and answers **tenancy-related FAQs** using natural language understanding. Built using BLIP for image captioning and FLAN-T5 for language generation, this bot helps landlords, tenants, and real estate professionals alike.

---

## 🔧 Features

### 🛠 Property Issue Detector
- Upload an image of a property (e.g., broken walls, leaky pipes).
- Optionally describe the problem.
- The bot analyzes the image and suggests possible troubleshooting steps or repairs.

### 📘 Tenancy FAQ Assistant
- Ask any question related to tenancy (e.g., rent, deposit, lease terms).
- Optionally include your city/region for location-specific advice.
- Get friendly, helpful, and legally-aware responses.

---

## 🚀 Demo

🟢 **Try it here**: [Real Estate Bot on Hugging Face Spaces](https://huggingface.co/spaces/HarshBhati/Estate)

---

## 🧠 Tech Stack

| Component | Details |
|----------|---------|
| **Image Captioning** | [BLIP](https://huggingface.co/Salesforce/blip-image-captioning-base) |
| **Language Generation** | [FLAN-T5 Large](https://huggingface.co/google/flan-t5-large) |
| **Frontend** | Gradio (Tabbed Interface) |
| **Deployment** | Hugging Face Spaces |
| **Programming Language** | Python |

---

## 🗂️ App Structure

### 1. **Image Analyzer (Agent 1)**
- Captures details from the uploaded image using BLIP.
- Combines image caption with optional user input.
- Generates a repair suggestion via FLAN-T5.

### 2. **Tenancy Assistant (Agent 2)**
- Accepts a text question and optional location.
- Uses FLAN-T5 to generate friendly and accurate tenancy responses.

### 3. **Keyword Classification (Optional)**
- Keywords like `rent`, `deposit`, `eviction` help classify user queries as FAQs.

---

## 🖼 Example Use Cases

### Property Issue Detection
- **Input**: Upload image of a broken window.
- **Output**: _"Image Description: A cracked glass window. Suggested Fix: Inspect the damage, temporarily cover with tape, and consider glass replacement."_

### Tenancy FAQ
- **Input**: "Can my landlord increase rent without notice?" (Location: London)
- **Output**: _"In London, landlords typically must give at least one month's written notice before raising rent. It also depends on the type of agreement you have..."_

---

## 🔍 How It Works

1. **Image is processed** using `BLIP` to create a caption.
2. **Caption + user description** is passed into `FLAN-T5` for a helpful suggestion.
3. For FAQs, user's query (and location, if given) is passed to `FLAN-T5` for a legal response.

---

## 🎥 Working Demo

> 📺 **Watch the full walkthrough here:**  
[👉 Click to Watch Demo Video](https://drive.google.com/file/d/1T9PB6TW7fCGEDY4Xlch9fSK5jeDImRVe/view?usp=sharing)

---

## 🧪 Run Locally

To run this app locally:

```bash
git clone https://github.com/<your-repo>/real-estate-bot.git
cd real-estate-bot

# Install dependencies
pip install -r requirements.txt

# Run the app
python Real_Estate_Bot.py
```

Or if using a notebook:

```python
!pip install torch transformers gradio pillow
# Then run the notebook cells
```

---

## 📜 License

This project is open source and free to use under the MIT License.

---

## 👤 Author

**Harsh Bhati**  
[Hugging Face Profile](https://huggingface.co/HarshBhati)

