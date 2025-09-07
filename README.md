# PRISM- Privacy-preserving Inference System with Homomorphic Encryption and Modular Activation

# Overview

This repository contains the code and research paper for the work titled "Privacy-Preserving CNNs with Homomorphic Encryption-Compatible Activations". The project proposes a framework that restructures CNNs and introduces efficient activation function approximations, enabling secure computations on encrypted data while reducing overhead

# Abstract
 
With the rapid advancements in machine learning, models have become increasingly capable of learning and making predictions in various industries. However, deploying these models in critical infrastructures presents a major challenge, as concerns about data privacy prevent unrestricted data sharing. Homomorphic encryption (HE) offers a solution by enabling computations on encrypted data, but it remains incompatible with machine learning models like convolutional neural networks (CNNs), due to their reliance on non-linear activation functions. To bridge this gap, this work proposes an optimized framework that replaces standard non-linear functions with homomorphically compatible approximations, ensuring secure computations while minimizing computational overhead. The proposed approach restructures the CNN architecture and introduces an efficient activation function approximation method to mitigate the performance trade-offs introduced by encryption. Experimental results using the CIFAR-10 dataset validate the effectiveness of the proposed framework with an accuracy of 94.4% with 2.4s per inference, demonstrating its ability to preserve accuracy while significantly reducing computational complexity in encrypted environments.

# Contents

training: Notebook used to train the CNN with homomorphic encryption-compatible activations.

testing: Evaluation code for encrypted inference and benchmarking performance.

weights: Pretrained model weights for reproduction and quick testing.

research paper: Full research paper detailing methodoligical approach and results


# Features

Homomorphic encryption–compatible CNN architecture design
Efficient activation function approximation for encrypted computation
Training and evaluation pipeline on CIFAR-10 dataset
Pretrained weights for reproducibility and benchmarking

# Requirements

numpy==2.1.2
pandas==2.3.1
torch==2.5.1+cu121
torchvision==0.20.1+cu121
torchaudio==2.5.1+cu121
tqdm==4.67.1
Pillow==11.0.0
tenseal==0.3.16
sympy==1.13.1


# Results

This work presented an optimized framework for privacy-
preserving convolutional neural network inference on the
CIFAR-10 dataset using homomorphic encryption. By em-
ploying a degree-4 polynomial approximation of the Softplus
activation function and carefully designing the CNN architec-
ture to balance expressiveness with computational constraints,
the system achieved 94.4% accuracy with efficient inference
times. The results demonstrate that it is possible to achieve
competitive performance without resorting to excessively deep
networks or high-degree polynomial approximations, which
would otherwise introduce significant computational overhead
in the encrypted domain

# Future Work

While CIFAR-10 provides a controlled benchmark, future work will evaluate the framework on real-world datasets to validate practical utility and robustness. Targets include (i) higher-resolution vision (e.g., ImageNet subsets), (ii) privacy-sensitive domains such as de-identified medical imaging (X-ray/CT) and smart-grid/IoT sensor streams, and (iii) autonomous driving frames (e.g., BDD100K subsets). This will assess accuracy–latency trade-offs under realistic distributions, quantify HE parameter impacts across devices, and guide tuning of our activation approximations for domain shift and deployment constraints.

# Ongoing

This work has been submitted to the IEEE CCNC 2026 Conference.

# Contact

For questions or collaborations, please contact:

Zeinab Elkhatib - zelkhati@tnstate.edu Kamrul Hasan - mhasan1@tnstate.edu