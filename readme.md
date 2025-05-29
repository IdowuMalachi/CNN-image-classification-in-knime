# 🧠 CNN Image Classification using MNIST (Built in KNIME)

This project presents a deep learning workflow developed in **KNIME Analytics Platform** to classify handwritten digits from the **MNIST** dataset using a **Convolutional Neural Network (CNN)**. The goal was to compare the performance of CNNs with traditional image classification techniques using a low-code, visual interface.

---

## 🎯 Project Objectives

- To explore and understand **deep learning (CNN)** architecture in a low-code environment (KNIME)
- To classify grayscale images (0–9 digits) from the **MNIST dataset**
- To evaluate CNN’s performance using **accuracy**, **loss**, and **confusion matrix**
- To visualize and interpret the impact of different CNN components on classification quality

---

## 🏗️ Model Architecture (KNIME CNN Design)

The CNN was implemented using **Keras integration in KNIME**. Below is the layered architecture:

- **Input Layer**: 28x28 grayscale images
- **Image Normalizer** (Scale pixel values to [0,1])
- **Conv2D Layer 1**: 32 filters, kernel size 3x3, activation: ReLU
- **MaxPooling2D Layer 1**: pool size 2x2
- **Conv2D Layer 2**: 64 filters, kernel size 3x3, activation: ReLU
- **MaxPooling2D Layer 2**: pool size 2x2
- **Flatten Layer**
- **Dense Layer**: 128 neurons, activation: ReLU
- **Output Layer**: 10 neurons, activation: Softmax

---

## 🔄 Workflow Steps

1. **Load MNIST dataset**
2. **Split dataset** (70% training / 30% testing)
3. **Normalize images**
4. **Build CNN architecture using Keras Layer nodes**
5. **Train model using Keras Network Learner**
6. **Evaluate using:**
   - Accuracy Scorer
   - Confusion Matrix Scorer
   - ROC Curve (multiclass)
   - Loss Chart & Training Performance Visualizer

---

## 📊 Evaluation Results

| Metric     | Value     |
|------------|-----------|
| **Accuracy**   | 98.3%     |
| **Loss**       | 0.06      |
| **Precision**  | 98.1%     |
| **Recall**     | 98.2%     |
| **F1-Score**   | ~98.15%   |

🧪 **Confusion Matrix:**  
Clear diagonal dominance indicating high classification success with minimal misclassifications.

---

## 📂 Project Structure


---

## 🛠️ Tools & Technologies

- **KNIME Analytics Platform**
- **Keras Deep Learning Integration**
- **TensorFlow Backend**
- **MNIST Dataset (28x28 grayscale images)**
- Image Processing nodes
- Python Environment for Keras Execution

---

## 💡 Key Takeaways

- KNIME’s visual programming empowers users to implement deep learning without coding.
- CNNs outperformed traditional classifiers due to their spatial feature extraction power.
- Visual workflow nodes like Keras Layer Builder, Loss Viewer, and Confusion Matrix make KNIME suitable for education and experimentation in AI.

---

## 👤 Author

**Idowu Malachi**  
Senior Data Scientist | AI/ML Developer | BI & Governance Strategist

- 🔗 GitHub: [github.com/idowumalachi](https://github.com/idowumalachi)
- 💼 LinkedIn: [linkedin.com/in/idowumalachi](https://linkedin.com/in/idowumalachi)
- 📧 Email: idowumalachi2696@gmail.com

---

> “This project proves that deep learning workflows can be built, optimized, and interpreted effectively in low-code environments like KNIME — making AI accessible to more analysts and business users.”
