# Synthetic-Pistachio-Image-Generation-using-GAN
## Project Overview
This project focuses on generating **synthetic pistachio images** using **Generative Adversarial Networks (GANs)**.  
The goal is to create images that closely resemble the original dataset, with performance evaluated using the **Fréchet Inception Distance (FID)** metric.  
Two models were compared: a **Baseline GAN** and a **Modified GAN** with architectural or training improvements.

---

## Model Performance (FID Score)

### Baseline GAN
- Best FID achieved: **233.5430** at epoch 160.  
- FID trends remained high and fluctuating between **250–350** throughout training.  
- Indicates that generated images are still far from the quality of real data.

### Modified GAN
- Best FID achieved: **12.10** at epoch 1000.  
- FID dropped sharply during training and stabilized at a low value, showing significant improvement in image realism.  
- Demonstrates that the modified GAN successfully learned to generate images closely matching the real data distribution.


## Training Considerations
- GANs require **long training times** (many epochs) to reach optimal performance.  
- Modified GAN only reached its best FID after **1000 epochs**, highlighting the slow convergence typical of GANs.  
- Adequate training is crucial for balancing the generator and discriminator and producing high-quality images.


##  Visual Insights
- FID trends show that the **Modified GAN (orange line)** consistently outperforms the **Baseline GAN (blue line)** at all checkpoints.  
- Low FID score (**12.10**) after sufficient training indicates high-quality, realistic synthetic images.  
- Reinforces that **training duration and model configuration** are critical for GAN performance.


## Tech Stack
- **Languages & Frameworks:** Python, TensorFlow / Keras  
- **Libraries:** NumPy, Matplotlib, Pandas  

