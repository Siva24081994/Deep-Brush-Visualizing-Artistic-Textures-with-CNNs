Deep Brush: Visualizing Artistic Textures with CNNs
📌 Project Overview
Deep Brush is a deep learning model that classifies and visualizes artistic textures, such as brushstrokes, using EfficientNet-B0. This project leverages CNNs to recognize patterns in artistic images and generates Grad-CAM heatmaps to interpret model decisions.

🎯 Objective
Develop a CNN-based model to classify artistic textures.

Improve model interpretability using Grad-CAM overlays.

Optimize training with data augmentation and hyperparameter tuning.

🛠️ Project Setup
1️⃣ Install Dependencies
Ensure you have Python installed and run the following commands in a Jupyter Notebook cell:

python
Copy
Edit
!pip install torch torchvision torchaudio
!pip install matplotlib numpy tqdm
!pip install opencv-python
2️⃣ Clone the Repository (Optional)
If the project is hosted on GitHub, clone it:

bash
Copy
Edit
git clone https://github.com/Siva24081994/Deep-Brush-Visualizing-Artistic-Textures-with-CNNs.git
cd Deep-Brush-Visualizing-Artistic-Textures-with-CNNs
Otherwise, directly open the Jupyter Notebook (.ipynb).

3️⃣ Open the Jupyter Notebook
If you are running it locally, navigate to the project folder and launch Jupyter:

bash
Copy
Edit
jupyter notebook
Then, open the Deep_Brush_CNN.ipynb file.

📊 Project Workflow
1️⃣ Dataset Preparation
Loaded 20+ artistic images provided by the company.

Resized and normalized images to 224×224 pixels to match EfficientNet input requirements.

Applied data augmentation (random rotation, flipping, color jitter) to improve generalization.

2️⃣ Model Training
Used EfficientNet-B0 as a pretrained model and modified the classifier layer.

Configured the training pipeline with:

Loss Function: Cross-Entropy Loss

Optimizer: Adam (learning rate = 0.0001)

Batch Size: 4

Epochs: 10

Tracked accuracy, loss, and F1 score during training.

Implemented checkpoint saving based on validation loss.

3️⃣ Model Evaluation & Interpretability
Evaluated on a validation set, achieving:
✅ Training Accuracy: 92.86%
✅ Validation Accuracy: 80%
✅ F1 Score: 0.8
![image](https://github.com/user-attachments/assets/5165f669-9686-4ff4-8e57-7848948ebe52)

Visualized Grad-CAM overlays to interpret how the model identifies artistic textures.

🔍 Results & Observations
The training loss steadily decreased, showing effective learning.

The validation accuracy stabilized at 80%, suggesting potential overfitting.

Grad-CAM heatmaps provided meaningful insights into how the model detected brushstrokes.

🔄 Future Improvements
🔹 Fine-tune hyperparameters to push validation accuracy beyond 80%.
🔹 Enhance data augmentation techniques for better model generalization.
🔹 Test alternative architectures (e.g., ResNet-50, Vision Transformer).

🖼️ Sample Grad-CAM Visualizations
![image](https://github.com/user-attachments/assets/4755e7aa-07a9-4519-8bd8-653cb003a973)


📜 Submission Format
The final project is provided as a Jupyter Notebook (.ipynb).

Includes code, training logs, visualizations, and insights for easy evaluation.

🤝 Contributions & Contact
For any improvements or discussions, feel free to connect:
📩 Email: gcms1994.gmail.com
🔗 GitHub: https://github.com/Siva24081994
