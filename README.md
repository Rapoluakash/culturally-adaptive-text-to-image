#culturally-adaptive-text-to-image
 
# Generative AI for Culturally Adaptive Text-to-Image Synthesis

This project explores the use of Stable Diffusion and Generative AI to synthesize culturally contextual images from textual prompts. It focuses on generating visuals that reflect regional traditions, festivals, and ethnic elements — such as *Ganesh idol immersions*, *Onam boat races*, or *Pongal celebrations*.

---

#🌍 Project Highlights

- 🎨 Text-to-Image generation using `stabilityai/stable-diffusion-2`
- 🌐 Hugging Face `diffusers` and `transformers` integration
- 🧠 Culturally relevant prompt crafting (India-focused, but extendable)
- 💻 Compatible with CPU and GPU environments (Colab-ready)

---

#📦 Dependencies

Install dependencies using pip:

```bash
pip install -r requirements.txt
````

Or use Conda:

```bash
conda env create -f environment.yml
conda activate culturally-adaptive-imagegen
```

---

#🚀 Usage

> ⚠️ For best performance, use this in a **GPU-enabled environment** like Google Colab.

1. Set your Hugging Face token (optional if already authenticated):

```bash
export HF_TOKEN=your_huggingface_token
```

2. Run the script:

```bash
python generate.py
```

3. Edit the prompts inside `generate.py` to try different cultural contexts, for example:

```python
generate_image("people are dancing in ganesh idol immersion", model)
generate_image("onam boat festival with snake boats", model)
```

---

#🧪 Running in GitHub Actions

GitHub Actions do not support CUDA, so this repo includes a CPU-safe CI workflow that only checks environment setup:

```bash
.github/workflows/python-app.yml
```

---

#📷 Example Prompts

| Prompt                                    | Sample Output |
| ----------------------------------------- | ------------- |
| `people dancing in Ganesh idol immersion` | *(image)*     |
| `Onam festival with traditional boats`    | *(image)*     |
| `Pongal celebrations in a village`        | *(image)*     |

> Add your outputs to the repo for showcase!

---

#🔐 Hugging Face Access Token

To use the `StableDiffusionPipeline`, set your token as an environment variable or use `.env`:

```env
HF_TOKEN=your_token_here
```

You can create a token at: [https://huggingface.co/settings/tokens](https://huggingface.co/settings/tokens)

---

#📁 File Structure

```
.
├── generate.py              # Main image generation script
├── config.py                # Configuration settings
├── requirements.txt         # pip dependencies
├── environment.yml          # Conda environment
├── .env.example             # Sample env file
└── .github/workflows/       # CI workflow for GitHub Actions
```

---

#🧠 Future Scope

* Cultural prompt generator using GPT-3/4
* Fine-tuned diffusion model on Indian art
* Gradio/Streamlit UI for end users
* Dataset creation for local traditions

---

#📄 License

This project is open-source under the MIT License. Attribution is appreciated.

```

---

Let me know if you'd like:
- To embed sample images in this README
- A badge (e.g., Build Passing, Hugging Face Space, Colab link)
- A custom logo/banner for the top of the repo

I can generate or design those for you too!
```
