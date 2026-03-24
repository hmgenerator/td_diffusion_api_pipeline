# 🧠 TouchDesigner + OpenAI Image Generation  
### Interactive Generative AI System (Workshop Setup)

This project demonstrates how to integrate **Generative AI image creation** into **TouchDesigner**, using the OpenAI API to generate images dynamically based on user input.

The system is designed as a **safe, controlled workshop environment**, combining:

- real-time interaction (TouchDesigner)
- generative image models (OpenAI)
- structured constraints (cooldown, prompt limits, session limits)

---

# 🎯 Learning Objectives

By working with this project, students will:

- Understand how to connect **TouchDesigner with external APIs**
- Learn how to build **interactive generative systems**
- Explore **prompt-based image generation**
- Reflect on **limitations, costs, and ethics** of generative AI
- Shift from:
  - “generate an image”
  - to
  - “design a system that generates images”

---

# ⚙️ System Overview

User Input → TouchDesigner → OpenAI API → Image File → TouchDesigner Output

---

# 🧩 Features

## Dynamic Prompt Input
Users type prompts directly in TouchDesigner.

## Image Generation via API
Uses OpenAI (`gpt-image-1-mini`) to generate images.

## Visual Feedback
Images are loaded automatically into a TOP.

## Safety System

- Cooldown (10s)
- Prompt limit (300 characters)
- Session limit (20 images)
- Generation lock

---

# 📦 Requirements

- TouchDesigner
- Internet connection
- Python `requests` library

---

# 🔑 API Key Setup

⚠️ Never share your API key publicly.

Replace:

```python
API_KEY = "PASTE_YOUR_OPENAI_API_KEY_HERE"
```

---

# 🖥️ TouchDesigner Setup

Required Operators:

- prompt_input (Text COMP)
- generate_image (Text DAT)
- status_data (Text DAT)
- moviefilein1 (TOP)
- null_button_trigger (CHOP)
- chopexecute1 (DAT)

---

# ▶️ Usage

1. Enter a prompt  
2. Trigger generation  
3. Wait  
4. View result  

---

# 💡 Prompt Tips

subject + material + lighting + mood + style

Example:

abstract glass landscape, soft light, cinematic mood

---

# 💰 Cost Awareness

Approx:

- €0.01 – €0.08 per image

---

# 🧠 Critical Reflection

- Who authors AI-generated images?
- How does cost affect creativity?
- Are aesthetics becoming homogenized?

---

# 🧪 Exercises

- Prompt variations
- System-based prompting
- Feedback visuals

---

# 🛠️ Extensions

- Audio-reactive prompts
- Camera input
- Multi-user systems

---

# 📚 Key Concept

TouchDesigner does not generate the image.  
It orchestrates a system where images are generated and transformed.

---

# 👨‍🏫 Teaching Note

Use this project as:

- technical introduction  
- creative tool  
- critical framework  

