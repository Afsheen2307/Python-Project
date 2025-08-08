***********Generative AI Model***********

## 🚀 What is This?
This project walks you through **building a Generative Adversarial Network (GAN) from scratch** using Python and Keras.  
The model learns to **generate images of handwritten digits** from the MNIST dataset — starting as random blobs and ending with crisp digits.  

You’ll learn:
- How **generators** and **discriminators** work together
- How to structure, train, and evaluate a GAN
- How to visualize your model’s progress


## 📂 Project Structure
.
├── README.md # You're reading this
├── gan_mnist.py / .ipynb # Main script or Jupyter Notebook
├── images/ # Training output snapshots
└── requirements.txt # Dependencies



---

## 🧠 How It Works
**1. The Generator** 🖌️  
Takes random noise → outputs a 28×28 pixel image.  
Uses:
- Dense layers
- LeakyReLU activations
- BatchNormalization
- `tanh` output to normalize pixel range

**2. The Discriminator** 🔍  
Classifies an image as **real** (from dataset) or **fake** (from generator).  
Uses:
- Flatten layer
- Dense + LeakyReLU
- Sigmoid output for probability

**3. The GAN** ⚔️  
We combine them so the generator learns to fool the discriminator while the discriminator gets better at spotting fakes.

---
<img width="1201" height="511" alt="image" src="https://github.com/user-attachments/assets/af2a8186-a45a-4486-8ec7-1c08ff161298" />

## 📸 Training Evolution
| Epoch 0 | Epoch 1000 | Epoch 5000 |
|---------|------------|------------|


> _From pure noise to recognizable digits!_

---

## 🧠 How It Works
**1. The Generator** 🖌️  
Takes random noise → outputs a 28×28 pixel image.  
Uses:
- Dense layers
- LeakyReLU activations
- BatchNormalization
- `tanh` output to normalize pixel range

**2. The Discriminator** 🔍  
Classifies an image as **real** (from dataset) or **fake** (from generator).  
Uses:
- Flatten layer
- Dense + LeakyReLU
- Sigmoid output for probability

**3. The GAN** ⚔️  
We combine them so the generator learns to fool the discriminator while the discriminator gets better at spotting fakes.

---

## 📸 Training Evolution
| Epoch 0 | Epoch 1000 | Epoch 5000 |
|---------|------------|------------|
| ![](images/gan_images_0.png) | ![](images/gan_images_1000.png) | ![](images/gan_images_5000.png) |

> _From pure noise to recognizable digits!_

---

## 🛠️ Installation & Usage
1. **Clone this repository**
   ```bash
   git clone https://github.com/Afsheen2307/generative-ai-gan.git
   cd generative-ai-gan

2. Install dependencies

   pip install -r requirements.txt

3. Run the model

   python gan_mnist.py

4. Generated images will appear in the images/ folder every few epochs.

 ----------------------------------------------------------------------------------------------------------
📦 Requirements

Python 3.8+
NumPy
Matplotlib
TensorFlow / Keras
  
