# ✈️🚢Aircraft-and-Ship-Detection-using-Semantic-Segmentation
Aircraft and Ship Detection using Semantic Segmentation
A deep learning project for semantic segmentation of aircraft and ships from satellite imagery using U-Net and enhanced Attention U-Net architectures with deformable convolutional layers.

🔧**Tools & Technologies**
Python, TensorFlow, Keras

Roboflow (for dataset annotation and augmentation)

Google Colab (for training)

OpenCV, Matplotlib (for visualization)

📁**Dataset**
Custom annotated dataset created using **Roboflow**

**Classes**: aircraft, ship, background

Exported in COCO segmentation format

**Augmented using**:

**Rotation:** ±90°

**Flipping:** Horizontal & Vertical

**Brightness:** ±30%

**Zoom:** 10–20%

🧠**Model Architectures**
U-Net (Baseline)

Attention U-Net (Enhanced focus on relevant features)

Attention U-Net + Deformable Convolution (Improved segmentation of irregular/occluded objects)

⚙️ **Training Details**
**Loss Function**: Composite of Dice Loss + Sparse Categorical Crossentropy

Optimizer: Adam

Training Strategy:

Transfer learning with last 10 layers unfrozen

Early stopping to avoid overfitting

Learning rate scheduling for stable convergence

📊 Results
🔸 Attention U-Net (Without Early Stopping)
✅ Training Accuracy: 98.64%

✅ Validation Accuracy: 98.14%

📉 Training Loss: 0.168 → 0.0407

📉 Validation Loss improvement: 0.0513

⏱️ Epochs: 30

🔸 Attention U-Net (With Early Stopping)
✅ Training Accuracy: 99.07%

✅ Validation Accuracy: 98.88%

📉 Training Loss: 0.310 → 0.237

📉 Validation Loss: 0.291 → 0.270

⏱️ Epochs: 31 / 50

🔸 Attention U-Net + Deformable Convolution (Best Model)
✅ Training Accuracy: 99.44%

✅ Validation Accuracy: 99.00%

📉 Training Loss: 0.770 → 0.2087

📉 Validation Loss: 0.2529

⏱️ Epochs: 31

📌 Key Features
Multi-class segmentation (aircraft, ship, background)

Supports occlusion and irregular object boundaries

Highly accurate results on small and imbalanced datasets

Efficient training with fine-tuning and augmentation

Scalable for defense, maritime, and disaster response tasks

📷 Sample Output:
![image](https://github.com/user-attachments/assets/fd1f7341-beac-4ecf-a17c-fe7bfcc20241)
![image](https://github.com/user-attachments/assets/82a341f3-3956-4c1e-9f00-5c2b2c2776a9)

