# 💻 Micro ResNet and Squeeze-and-Excitation Implementations from Scratch

This repository contains a series of Jupyter notebooks that explore the implementation and training of various simplified or "micro" Residual Network (ResNet) architectures, built completely **from scratch** using fundamental libraries like PyTorch to understand the internal architecture.

---

## 📂 Repository Contents

The repository is organized into the following notebooks, each focusing on a specific implementation:

### 1\. 🏗️ `Deep_Learning_Micro_Resnet.ipynb`

This notebook lays the groundwork, showcasing the construction and training of a **Basic Micro ResNet**.

* **Main Objective:** To understand the fundamental concept of the **residual block** and its implementation to mitigate the *vanishing gradient* problem in deep networks.
* **Architecture:** Implementation of the **identity shortcut** path and basic convolutional layers for a shallow ResNet.

---

### 2\. 🚀 `Deep_Learning_Resnet_34.ipynb`

An extension of the previous notebook, this one implements a deeper architecture, similar in principle to the well-known **ResNet-34**.

* **Main Objective:** To build and stack **multiple residual blocks** (basic two-layer block) to create a deeper network, managing **downsampling** using *strides* or projection blocks.
* **Architecture:** Design of a 34-layer model, exploring the different stages of the network and the transition between them.

---

### 3\. 👑 `Deep_Learning_SE_Resnet_50.ipynb`

This notebook introduces an additional complexity: the implementation of the **Bottleneck Block** (used in ResNet-50) along with the **Squeeze-and-Excitation (SE)** attention mechanism.

* **Main Objective:**
    1.  To implement the **Bottleneck Block** (1x1, 3x3, 1x1) which reduces computational complexity.
    2.  To integrate the **Squeeze-and-Excitation** module, which allows the network to perform adaptive recalibration of the feature channels (**channel-wise attention**).
* **Architecture:** Construction of a 50-layer network with *bottleneck* blocks and the SE module integrated into each residual block.

---

## 🤝 Contributions

If you have suggestions, corrections, or want to propose an extension, you are welcome! Please open an *Issue* or send a *Pull Request*.

---

## Author

* **Juan Guillermo Gómez**
* Linkedin: [@jggomezt](https://www.linkedin.com/in/jggomezt/)

***
