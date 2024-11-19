# Dog-Cardiomegaly

Best Weights for this model are available at: [Google Drive Link](https://drive.google.com/file/d/1n6C0K-0h2NK95PqOSvoEKcXyE1-w2L-m/view?usp=sharing)

## Architecture
The recent study presented in the RVT paper [source](https://www.nature.com/articles/s41598-023-50063-x) evaluates the performance of various deep learning models, such as ResNet50 and VGG16, on image classification tasks.

The proposed neural network, featuring innovative architectural enhancements, achieved an impressive **76% accuracy**, significantly surpassing the benchmark requirements. The model's key advancements include:

1. **Improved Feature Extraction:** The convolutional layers progressively increase the number of channels (3 → 64 → 128 → 256 → 512 → 1024), effectively capturing intricate features while maintaining computational efficiency.
2. **Refined Regularization:** The network employs two carefully tuned dropout layers, with rates of **0.5** and **0.3**, to effectively reduce overfitting and improve generalization.
3. **Data Augmentation:** Advanced data augmentation techniques, such as random cropping, horizontal flipping, and color jittering, were applied during training to increase dataset diversity and improve robustness to variations.
4. **Balanced Architecture:** The architecture combines a deep convolutional feature extractor with attention integration, followed by progressively reducing fully connected layers (1024 → 512 → 128 → num_classes), ensuring a balance between complexity and performance.
5. **Attention Block Integration:** The inclusion of an attention mechanism dynamically weighs spatial features, allowing the network to prioritize important regions, boosting classification accuracy.

### Architecture Diagram

Below is the architecture diagram of the proposed model:

![Architecture Diagram](assets/Dog_Heart_Architecture.drawio (1).png)

#### Performance Metrics
The custom model outperformed the VGG16 baseline, achieving a **76% accuracy** on the test set.

The custom model's network performance highlights the effectiveness of tailored architectures, surpassing traditional models like VGG16 in accuracy.
