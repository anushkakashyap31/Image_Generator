> # **🚀Image Generation using Diffusers and StableDiffussion**

Generating images from text prompts using Hugging Face’s Diffusers library and Stable Diffusion model.

### **💡 Project Overview**

In this task, I have:

- Used the Hugging Face `diffusers` library and PyTorch.
- Generated images using a pre-trained Stable Diffusion model.
- Worked completely on **Google Colab** for convenience and GPU support.

### **📄 Files**

- `Task_2_Image_Generation.ipynb`: Colab Notebook used to generate images from text prompts.
- `image_outputs/`: Folder for sample outputs (if applicable).
- `.gitignore`: Skips unnecessary files in version control.

### **⚙️ Technologies Used**

- Python
- Google Colab
- Hugging Face Diffusers
- PyTorch
- Transformers

### **💬 How to Use**

1️⃣ Open the notebook in Google Colab: [🔗][https://colab.research.google.com/drive/1nJJjq8MRQQO0TiqLRm\_w2gy015cLVhFm#scrollTo=-\_asAOZyc\_u6]

✅ STEP 1: Install required library

```
!pip install diffusers transformers accelerate
```

✅ STEP 2: Import and Load Model

```
from diffusers import StableDiffusionPipeline

# Model id
model_id = "runwayml/stable-diffusion-v1-5"

# Load pipeline
pipe = StableDiffusionPipeline.from_pretrained(model_id)

# Move to GPU
pipe = pipe.to("cuda")
```

✅ STEP 3: Generate Image

```
# Text prompt for the image
prompt = "A beautiful landscape with mountains and a sunset"

# Generate image
image = pipe(prompt).images[0]

# Display the image in the notebook
image.show()
```

✅ (Optional) Save Image

```
image.save("generated_image.png")
```

2️⃣ Run all cells one by one.\
3️⃣ Enter your own prompt and generate beautiful AI images.

### **🎯 Objectives**

- Learn to generate AI images from text.
- Understand Diffusers and Stable Diffusion.
- Practice hands-on project using Google Colab.

### **👩‍💻 Author**

### **Anushka Kashyap**

### **⭐ Acknowledgements**

- Prodigy Infotech
- Hugging Face
- Google Colab
- Stable Diffusion model

**✨ Do ⭐ star the repo if you found it useful!**
