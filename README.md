# 📸 InstaVision: LLM-Powered Photo Caption & Hashtag Generator

InstaVision is an AI-powered tool that generates stylish Instagram captions and trending hashtags from any uploaded photo. It combines image understanding using BLIP (Bootstrapped Language Image Pretraining) with natural language generation via OpenAI’s GPT, making it ideal for content creators, marketers, and influencers.

---

## 🚀 Features

- 🖼️ Upload any image (scenic, travel, food, pets, etc.)
- 🧠 Scene description via BLIP (Vision-Language model)
- 💬 Caption + Hashtag generation via GPT-4 / GPT-3.5
- ✨ Captions include emojis, tone, and aesthetic
- 🔁 Fully automated pipeline in Google Colab

---

## 🧠 Model Details

### 🖼️ BLIP (Bootstrapped Language Image Pretraining)
- **Purpose:** Generates a high-level natural language description of the uploaded image.
- **Architecture:**
  - **Vision Encoder:** Vision Transformer (ViT-B)
  - **Text Decoder:** Transformer decoder
  - **Training Objective:** Captioning, image-text matching, and retrieval
- **Model Used:** `Salesforce/blip-image-captioning-base`
- **Input:** Raw image
- **Output:** Natural language description like _"a scenic view of a mountain at sunset"_

### 💬 GPT (OpenAI GPT-3.5 / GPT-4)
- **Purpose:** Stylizes the BLIP-generated caption and adds emojis + popular hashtags
- **Model Used:** `gpt-4` or `gpt-3.5-turbo`
- **Prompt Structure:**  
  _“Turn this image description into a stylish Instagram caption with emojis and 10 popular hashtags.”_
- **Output:**  
  _"Chasing waterfalls in the mountains 🌄☀️ Nature's beauty at its finest 💦 #MountainMagic #NatureLovers #Wanderlust..."_

---

## 🛠️ Tech Stack

- Python
- Google Colab
- Hugging Face Transformers
- OpenAI GPT API
- PyTorch, PIL, Matplotlib

---

## 📦 Setup Instructions

1. Clone the repository or open the Colab notebook
2. Install dependencies:
    ```bash
    pip install transformers timm accelerate openai
    ```
3. Upload your image
4. Enter your OpenAI API key
5. Run the notebook and get your caption!

---

## 🔑 Requirements

- Python 3.8+
- OpenAI API key
- Google Colab (Free tier compatible)

---

## 🧪 Example Output

> **BLIP Caption:**  
> _"a scenic view of a waterfall in the mountains at sunset"_

> **Generated Instagram Caption:**  
> _"Chasing waterfalls in the mountains 🌄☀️ Nature's beauty at its finest 💦"_

> **Hashtags:**  
> `#MountainMagic #SunshineVibes #NaturePhotography #AdventureAwaits #ExploreMore #Wanderlust #ScenicViews #NatureLovers #ChasingWaterfalls #MountainLife`

---

## 📌 Future Enhancements

- Style selector: Funny, Poetic, Minimalist, Chill
- Gradio Web UI
- Batch mode for multiple image captioning
- Hashtag ranking based on engagement stats

---

## 🙌 Credits

- [BLIP by Salesforce](https://github.com/salesforce/BLIP)
- [OpenAI GPT](https://platform.openai.com/)
- [Hugging Face Transformers](https://huggingface.co/transformers/)

---


