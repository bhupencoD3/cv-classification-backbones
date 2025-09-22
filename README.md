___

## CV Classification Backbones

 A hands-on learning repository implementing **classic and modern image classification backbones** from scratch in both **PyTorch** and **TensorFlow**. The goal of this repo is to build a solid understanding of how popular computer vision architectures are structured, trained, and compared across frameworks.

---

## Repository Contents

* **LeNet/**

  * `LeNet5_mnist_torch.ipynb` → LeNet implementation using PyTorch
  * `LeNet5_mnist_tf.ipynb` → LeNet implementation using TensorFlow

* **AlexNet/**

  * `AlexNet_tf.ipynb` → AlexNet implementation using TensorFlow trained on custom Daisy vs Dandelion dataset
  * `AlexNet_torch.ipynb` → AlexNet implementation using PyTorch trained on custom Daisy vs Dandelion dataset

* **VGG/**

  * `vgg_pretrained_tf.ipynb` → Pretrained VGG16 and VGG19 (TensorFlow/Keras) demonstration with ImageNet inference
  * `vgg_pretrained_torch.ipynb` → Pretrained VGG16 (PyTorch) demonstration with ImageNet inference

---

## Planned Architectures

This repo currently focuses on:

* ✅ **LeNet** (PyTorch & TensorFlow)
* ✅ **AlexNet** (PyTorch & TensorFlow)
* ✅ **VGG (Pretrained – TensorFlow & PyTorch)**
* 🔄 **Inception**
* 🔄 **ResNet**

Each architecture has **two versions**: one in **PyTorch** and one in **TensorFlow** for comparison.

---

## Results

### LeNet Results

* **PyTorch (10 epochs, MNIST)** → **99.15%** accuracy
* **TensorFlow (20 epochs, MNIST)** → **99.08%** accuracy

### AlexNet Results

* **TensorFlow (20 epochs, Daisy vs Dandelion Custom Dataset)** → **0.8102 accuracy**
* **PyTorch (5 epochs, Daisy vs Dandelion Custom Dataset)** → **82.42% accuracy**

### Results Table

| Model   | Framework  | Dataset                     | Epochs | Accuracy   | Best |
| ------- | ---------- | --------------------------- | ------ | ---------- | ---- |
| LeNet   | PyTorch    | MNIST                       | 10     | **99.15%** | ✅    |
| LeNet   | TensorFlow | MNIST                       | 20     | 99.08%     |      |
| AlexNet | TensorFlow | Daisy vs Dandelion (Custom) | 20     | 0.8102     |      |
| AlexNet | PyTorch    | Daisy vs Dandelion (Custom) | 5      | **82.42%** | ✅    |
| VGG16   | TensorFlow | Pretrained ImageNet         | N/A    | Inference  | ✅    |
| VGG16   | PyTorch    | Pretrained ImageNet         | N/A    | Inference  | ✅    |

---

## Tech Stack

* **Python 3**
* **PyTorch**
* **TensorFlow / Keras**
* **Torchvision**
* **NumPy**
* **Matplotlib**
* **PIL (Pillow)**

---

## Purpose

* To learn how classification backbones are built from scratch.
* To compare implementations across frameworks (PyTorch vs TensorFlow).
* To understand design choices behind classic and modern CNNs.
* To create a reference repo for interview prep and future projects.

---

## Usage Example (PyTorch VGG16)

```python
from vgg_pretrained_torch import infer, show_image

image_path = 'elephant.jpg'
show_image(image_path)
results = infer(image_path)
for label, prob in results:
    print(f'{label} {prob:.4f}')
```

This notebook demonstrates how to:

* Load a **pretrained VGG16 model** in PyTorch.
* Preprocess images and perform inference.
* Display the top-5 predictions for any input image.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Author

**bhupen** – Building and benchmarking deep learning backbones for computer vision
[LinkedIn](https://www.linkedin.com/in/bhupenparmar/) | [GitHub](https://github.com/bhupencoD3)
