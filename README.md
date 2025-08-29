
Brain Tumor Classification with ResNet50
Overview
This project implements a deep learning model for classifying brain tumors using the ResNet50 architecture. The model is trained on a brain tumor dataset to identify different tumor types from MRI images. It leverages transfer learning, data augmentation, and fine-tuning to achieve robust performance, with a final test accuracy of 81.22%.
Features

Dataset: Brain tumor MRI images organized into training and testing sets.
Model: Pre-trained ResNet50 with custom classification layers.
Data Preprocessing: Images resized to 224x224, converted to RGB, and augmented with rotation, zoom, and flips.
Training: Three-phase training with initial training (30 epochs), fine-tuning (20 epochs), and ultra-low learning rate pass (5 epochs).
Techniques: Class weights for handling imbalance, early stopping, and learning rate reduction for optimized training.
Results: Achieved 81.22% test accuracy after final training.

Requirements

Python 3.x
TensorFlow/Keras
OpenCV
NumPy
Scikit-learn

Usage

Clone the repository:git clone https://github.com/MohamedAchraf22/Brain-Tumor-Classification-Using-Resnet50.git


Install dependencies:pip install -r requirements.txt


Update dataset paths in the notebook to point to your local dataset.
Run the Brain_Tumor_Classification.ipynb notebook to preprocess data, train the model, and evaluate results.

Dataset
The dataset should be organized as follows:
brain_tumor_dataset/
Training/
glioma_tumor/
meningioma_tumor/
...
 Testing/
 glioma_tumor/
 meningioma_tumor/
 ...

Results

Initial Training: Test accuracy of 75.38%.
Fine-Tuning: Test accuracy improved to 80.96%.
Final Training: Test accuracy reached 81.22% with a validation accuracy of 96.75%.

License
This project is licensed under the MIT License.
Acknowledgments

Dataset source: [Add dataset source or Kaggle link if applicable]
Built with TensorFlow and Keras.
