# 👕 Virtual Try-On System

A Computer Vision and Generative AI project that allows users to upload a photo and virtually change their clothing using AI-powered image segmentation and Stable Diffusion inpainting.

This project was developed as part of a Computer Vision assignment to demonstrate how semantic segmentation and image generation can be combined to create a virtual try-on experience.

---

## 🚀 Demo

> **Open in Google Colab**

[![Open In Colab](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQnP6Kj0hajFHp3aXMCx_IukLgUAkBc3VB8U34tmII1bQ&s)]


---

## 📌 Features

* Upload a person image
* Select **Upper Body** or **Lower Body**
* Automatically segment clothing using AI
* Generate new clothing from a text prompt
* Interactive web interface with Gradio
* Automatic fallback to local Stable Diffusion when API is unavailable
* Error handling for API failures and invalid inputs

---

## 🛠️ Tech Stack

* Python
* PyTorch
* Hugging Face Transformers
* SegFormer
* Stable Diffusion Inpainting
* Gradio
* Pillow
* NumPy

---

## 🧠 Project Workflow

```text
Upload Image
      │
      ▼
Image Preprocessing
      │
      ▼
Clothing Segmentation (SegFormer)
      │
      ▼
Generate Binary Mask
      │
      ▼
Stable Diffusion Inpainting
      │
      ▼
Virtual Try-On Result

## ▶️ Usage

1. Open the notebook in Google Colab.
2. Run all cells.
3. Upload a person image.
4. Select the clothing area:

   * Upper Body
   * Lower Body
5. Enter a clothing prompt (for example: **Black leather jacket**).
6. Click **Try On**.
7. View the generated image.

---

## 📸 Example

### Input

* Upload an image
* Select **Upper Body**
* Prompt:

  ```
  Black leather jacket
  ```

### Output

AI generates a new image with the selected clothing replaced while preserving the person's appearance.

---

## 🤖 AI Models Used

### SegFormer

Used for semantic clothing segmentation.

Model:

```
mattmdjaga/segformer_b2_clothes
```

### Stable Diffusion Inpainting

Used for AI-based clothing generation.

Model:

```
runwayml/stable-diffusion-inpainting
```

---

## 📦 Requirements

* Python 3.10+
* CUDA GPU (recommended)
* Google Colab GPU Runtime (recommended)

Libraries

```text
torch
transformers
gradio
numpy
pillow
requests
diffusers
accelerate
safetensors
```

---

## ⚠️ Notes

* A Hugging Face Access Token may be required for hosted inference.
* If the hosted API is unavailable, the project can automatically use a local Stable Diffusion pipeline.
* A GPU runtime is highly recommended for faster inference.

---

## 🎯 Learning Outcomes

This project helped me learn:

* Computer Vision
* Semantic Segmentation
* Stable Diffusion
* Prompt-based Image Editing
* Hugging Face Transformers
* Gradio Application Development
* AI Model Integration

---

## 📖 Future Improvements

* Support multiple clothing styles
* Better segmentation accuracy
* Faster inference
* Background preservation
* Higher-resolution outputs
* Mobile-friendly interface

---

