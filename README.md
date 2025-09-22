# 🧩 MNIST Denoising Autoencoder (PyTorch)

This project implements a **Convolutional Denoising Autoencoder** using **PyTorch** for the classic **MNIST digit dataset**.  
The model learns to remove noise from images, reconstructing clear digits from corrupted inputs.  

It’s a practical example of **Deep Learning for Computer Vision**, showcasing the use of **Autoencoders** for denoising tasks.


## 🚀 Features
- **Convolutional Autoencoder** built in PyTorch.  
- **Noise injection** with Gaussian noise.  
- **Image denoising** with clean reconstructions.  
- **Training pipeline** with MSE loss + PSNR metric.  
- **Visualization** of Original / Noisy / Reconstructed digits.  


## 📂 Project Structure
```
notebooks/
autoencoder_mnist.ipynb # main notebook (training & evaluation)
data/ # MNIST is downloaded automatically
requirements.txt # dependencies
README.md
```


## 🗃️ Dataset
The notebook automatically downloads **MNIST** using `torchvision.datasets.MNIST`.  
Each image is **28x28 grayscale**, with labels (0–9). Labels are not used in training (unsupervised).


## ▶️ How to Run
1. Create an environment and install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
2. Open the notebook:
   ```bash
   jupyter notebook notebooks/autoencoder_mnist.ipynb
   ```
3. Run all cells to train and visualize results.


## 🔍 Results
- Input digits are corrupted with random Gaussian noise.
- The Autoencoder reconstructs clean versions of the digits.
- Evaluation metrics:
    - MSE Loss
    - PSNR (Peak Signal-to-Noise Ratio)


## 🛠️ Tech Stack
- Python
- PyTorch 
- Torchvision 
- Matplotlib 
- NumPy


## ⚠️ Notes
- Training runs on CPU by default. If CUDA is available, the notebook uses it automatically.
- Results may vary slightly due to randomness in noise injection.
