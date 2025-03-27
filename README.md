# Transfer-Learning-for-Grapevine-Leaves-Detection
Grapevine Leaf Classification with Modified DenseNet-121
This project leverages Convolutional Neural Networks (CNNs) to classify different varieties of grapevine leaves in controlled environments. By utilizing transfer learning with a modified DenseNet-121 architecture, the model achieves efficient and accurate identification of five distinct grapevine leaf types, which can significantly enhance sorting, grading, and quality assessment processes in agricultural applications.

Key Features
Dataset
The model is trained on a curated dataset containing high-quality images of grapevine leaves. The dataset comprises five unique classes:

Ak

Ala_Idris

Buzgulu

Dimnit

Nazli

Model Architecture
This project employs a Modified DenseNet-121 model:

Transfer Learning: Leverages pretrained ImageNet weights for robust feature extraction.

Custom Classification Head: A global average pooling layer followed by fully connected layers, fine-tuned to the grapevine leaf classification task.

Optimized for Small Datasets: Adaptations to the DenseNet-121 architecture ensure excellent performance even with a relatively small dataset.

Preprocessing & Augmentation
Images are resized (e.g., to 224×224) to meet the model's input requirements, normalized, and converted to RGB format. Data augmentation (random rotations, shifts, zoom, etc.) is applied to enhance the diversity of the training data and improve generalization.

Training
The model is trained for 25 epochs using an Adam optimizer with a learning rate fine-tuned for convergence. The training process incorporates a validation split to monitor performance and mitigate overfitting.
