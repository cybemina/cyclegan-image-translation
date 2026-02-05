 Project Title
CycleGAN for Unpaired Image-to-Image Translation

 Overview
This project implements a Cycle-Consistent Generative Adversarial Network (CycleGAN) for unpaired image-to-image translation.

CycleGAN enables learning a mapping between two visual domains without requiring paired training samples.

The model is capable of translating images between two domains (e.g., horses ↔ zebras, summer ↔ winter) while preserving content consistency.

 Dataset
The dataset consists of two unpaired image domains:

Domain A
Domain B
Images are preprocessed through resizing, normalization, and batching to ensure stable GAN training.

 Model Architecture
Two Generators
Generator A → B
Generator B → A
Two Discriminators
Discriminator A
Discriminator B
The architecture relies on:

Adversarial loss
Cycle-consistency loss
(Optional) Identity loss
 Training Strategy
Adversarial training between generators and discriminators
Cycle-consistency loss to preserve image structure
Optimized using Adam optimizer
Trained for multiple epochs to improve translation quality
Results
The model successfully translates images between domains while maintaining visual consistency.

Generated samples are visualized throughout training to assess convergence and realism.

 Technologies Used
Python
TensorFlow / PyTorch
NumPy
matplotlib
Jupyter Notebook
