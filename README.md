# 🌄 Generate Panoramic Images with Python

> Transform text into stunning panoramic visuals with HunyuanWorld-1.0 Text to Panorama

<p align="center">
 <img src="https://cdn.wiro.ai/uploads/models/tencent-HunyuanWorld-text-to-panorama-cover.jpg" alt="HunyuanWorld-1.0 Text to Panorama Cover" width="100%">
</p>

---

<div align="center">

[![python](https://img.shields.io/badge/python-3.8+-blue)](https://www.python.org/downloads/release/python-380/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Wiro.ai](https://img.shields.io/badge/Powered%20by-Wiro.ai-brightgreen)](https://wiro.ai)

</div>

---

## ✨ Features

- 🎨 **4K Panoramic Generation**: Create wide-angle images with resolution 1920x960
- ⚙️ **Controlled Inference**: Adjust steps (40) and guidance scale (30.0)
- 🖼️ **Customizable Output**: Set blend extend (6), CFG scale (0.0), and seed (0)
- 🧠 **Advanced Prompting**: Use positive and negative prompts for fine control
- 📏 **Flexible Dimensions**: Configure width (1920) and height (960) dimensions

## 🛠️ Operations

1. **Go to [wiro.ai](https://wiro.ai)** and sign up for a free account
2. **Create a new project** at [wiro.ai/panel/project/new](https://wiro.ai/panel/project/new)
3. **Copy your credentials** from the project dashboard:
 - API Key (your public key)
 - API Secret (your private secret)
4. **Add to your project** using the exact format below:

```bash
# Copy the environment file and fill in your credentials
 cp .env.example .env

Edit your `.env` file with your Wiro credentials:

```env
WIRO_KEY=XYZXYZXYZXYZXYZXYZXYZXYZ
WIRO_SECRET=QWERTYQWERTYQWERTYQWERTY

Then run the project:

```bash
python main.py

## 📚 Resources

<div align="center">

<img src="https://wiro.ai/images/illustrations/koala-404.png" alt="Wiro Koala Mascot" height="100">

### Learn More

📖 [**tencent/hunyuanworld-text-to-panorama Model**](https://wiro.ai/models/tencent/hunyuanworld-text-to-panorama)
📋 [**API Documentation**](https://wiro.ai/models/tencent/hunyuanworld-text-to-panorama/llms-full.txt)
👨‍💻 [**API Samples (PYTHON)**](https://wiro.ai/models/tencent/hunyuanworld-text-to-panorama#apisamples-python)
🌐 [**Wiro Example Projects**](https://wiro.ai/docs/example-projects)

</div>

## 🧠 Compatibility

- Python 3.8+
- Wiro API v1

## 📁 Folder Structure

project-root/
├── requirements.txt
├── .env.example
├── .gitignore
├── main.py
├── wiro_client.py
└── examples/
 └── basic.py

## 📦 Installation

Install required packages:

```bash
pip install -r requirements.txt

## 💡 Inspire Examples

```python
from wiro_client import WiroClient
import os
from dotenv import load_dotenv

load_dotenv()

client = WiroClient(os.getenv("WIRO_KEY"), os.getenv("WIRO_SECRET"))

# Example 1: Abandoned Library Hall
params = {
 "prompt": "A grand, abandoned library hall, panoramic view. Towering bookshelves stretch from floor to ornate ceiling, filled with dusty, leather-bound tomes. Broken chandeliers hang precariously, casting fragmented light across cracked marble floors and scattered papers. Sunlight streams through tall, arched windows, illuminating swirling dust motes and highlighting the faded murals on the walls. A long, winding staircase leads to an upper gallery, partially collapsed in places, emphasizing the quiet decay and forgotten grandeur of the space.",
 "negativePrompt": "",
 "steps": 40,
 "scale": 30.0,
 "blendExtend": 6,
 "cfgScale": 0.0,
 "seed": "0",
 "width": 1920,
 "height": 960
}

print("🚀 Generate Panoramic Images with Python")
print("Running HunyuanWorld-1.0 Text to Panorama...")
print("Parameters:", params)

result = client.execute(params)
print("✅ Result:", result)
python
from wiro_client import WiroClient
import os
from dotenv import load_dotenv

load_dotenv()

client = WiroClient(os.getenv("WIRO_KEY"), os.getenv("WIRO_SECRET"))

# Example 2: Desert Sandstorm
params = {
 "prompt": "A raging desert sandstorm sweeping across a barren wasteland, panoramic view. Towering dunes shift under violent winds, with dust spiraling into colossal clouds that obscure the horizon. The sun is barely visible through the thick haze, casting diffused amber light over scattered rocks and cracked earth. Occasional remnants of abandoned structures peek through the sand, evoking a post-apocalyptic feel of nature's unstoppable force.",
 "negativePrompt": "",
 "steps": 40,
 "scale": 30.0,
 "blendExtend": 6,
 "cfgScale": 0.0,
 "seed": "0",
 "width": 1920,
 "height": 960
}

print("🚀 Generate Panoramic Images with Python")
print("Running HunyuanWorld-1.0 Text to Panorama...")
print("Parameters:", params)

result = client.execute(params)
print("✅ Result:", result)

## 🎬 Sample Output Gallery

| Sample 1 | Sample 2 | Sample 3 |
|:--------:|:--------:|:--------:|
| ![Sample 1](https://cdn.wiro.ai/uploads/models/tencent-HunyuanWorld-text-to-panorama-sample-8.jpg) | ![Sample 2](https://cdn.wiro.ai/uploads/models/tencent-HunyuanWorld-text-to-panorama-sample-9.jpg) | ![Sample 3](https://cdn.wiro.ai/uploads/models/tencent-HunyuanWorld-text-to-panorama-sample-10.jpg) |

| Sample 4 | Sample 5 | Sample 6 |
|:--------:|:--------:|:--------:|
| ![Sample 4](https://cdn.wiro.ai/uploads/models/tencent-HunyuanWorld-text-to-panorama-sample-11.jpg) | ![Sample 5](https://cdn.wiro.ai/uploads/models/tencent-HunyuanWorld-text-to-panorama-sample-12.jpg) | ![Sample 6](https://cdn.wiro.ai/uploads/models/tencent-HunyuanWorld-text-to-panorama-sample-13.jpg) |

| Sample 7 |
|:--------:|
| ![Sample 7](https://cdn.wiro.ai/uploads/models/tencent-HunyuanWorld-text-to-panorama-sample-14.jpg) |

---

⭐ Star this repo • 🐍 Python Implementation

---

<sub>**Keywords:** panoramic images, python, AI generation, text to image, wide angle, 4K panorama, image creation, studio photos</sub>
```