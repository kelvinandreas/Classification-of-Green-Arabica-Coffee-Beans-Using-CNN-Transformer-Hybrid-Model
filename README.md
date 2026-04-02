# Classification of Green Arabica Coffee Beans Using CNN-Transformer Hybrid Model

This research proposes a hybrid deep learning model combining CNN and Transformer architectures to enhance the classification accuracy of green arabica coffee beans. The model leverages both local feature extraction (via CNN) and global context capture (via Transformer) to improve classification performance.<br>

This research evaluated 8 different hybrid model configurations by combining four CNN-based models (ResNet-18, ResNet-50, MobileNetV3, and EfficientNetB4) with two Transformer-based models (Vision Transformer and Swin Transformer). Hyperparameter tuning was performed using grid search on learning rates and batch sizes, resulting in a total of 48 experiments.

Using the USK-Coffee dataset, the best-performing hybrid model (R50-V: ResNet-50 + Vision Transformer) achieved **91.88% accuracy**, outperforming previous single-model approaches. The full paper is available at **[this link](http://www.icicel.org/ell/contents/2026/4/el-20-04-12.pdf)**.

## Dataset & Experiment Results

- **Dataset**<br>
The USK-Coffee dataset contains 8,000 images of green arabica coffee beans categorized into four classes: **peaberry**, **longberry**, **premium**, and **defect**. The dataset is already divided into training (60%), validation (20%), and test (20%) sets, with each subset containing a balanced number of images from all classes. The original dataset is available from [Syiah Kuala University, Banda Aceh, Indonesia](https://coffee.comvislab-usk.org/).

- **Experiment Results**<br>
The hybrid model combining ResNet-50 and Vision Transformer (R50-V) achieved the best performance with:
    - **Accuracy**: 91.88%
    - **Precision**: 92.12%
    - **Recall**: 91.88%
    - **F1-Score**: 91.85%

## Implementation

The best-performing R50-V hybrid model has been deployed as a web-based application that accepts green arabica coffee bean images and classifies them into one of four categories in real-time.

### Live Demo
You can test the model live at: **[Try the demo here](https://coffeeclassification.kelvinandreas.tech/)**

### Access Model & Notebook
- **Best Model (R50-V)**: The trained model achieving 91.88% accuracy is available on [Hugging Face](https://huggingface.co/kelvinandreas/Green_Arabica_Coffee_Bean_Classification_R50-V)
- **Inference Notebook**: An inference implementation using the pre-trained model is available in this repository ([main.ipynb](main.ipynb))

## BibTeX Citation

If you use this work in a scientific publication, we would appreciate using the following citation:

```
(will be updated soon)
```

## Poster
*(will be updated soon)*
