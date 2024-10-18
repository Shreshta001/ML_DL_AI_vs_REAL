# 📄 Identification of AI-Generated Synthetic Images (on CIFAKE dataset) 


**Authors:** Jordan J. Bird, Ahmad Lotfi

---

## 🧠 Overview of the Research

> ### 🎯 **Purpose**
> The main goal of this study is to enhance the detection of AI-generated images, which have become so realistic that humans often cannot tell them apart from actual photographs. This ability is crucial for ensuring the authenticity of visual data in various fields, including journalism, law, and social media.

---

## 🗂️ Dataset Creation

- **📚 CIFAR-10 Dataset:**  
  The researchers used an existing dataset called **CIFAR-10**, which contains 60,000 small images divided into 10 categories (like 🐱 cats, 🐶 dogs, 🚗 cars, etc.). They utilized 50,000 images for training their model and 10,000 for testing it.
  
- **🖼️ Synthetic Image Generation:**  
  An additional 60,000 synthetic images were generated using a technique called **Latent Diffusion Models (LDMs)**. This method creates new images based on textual prompts (like "a photograph of a cat") and random noise. The resulting dataset is named **CIFAKE**, which combines both real and synthetic images.

---

## 🧠 Classification Method

The researchers employed a **Convolutional Neural Network (CNN)** for image classification. A CNN is a type of machine learning model designed to process visual data. Here's how it works step-by-step:

1. **🖼️ Input Layer:** The CNN takes an image as input.
2. **🔍 Convolutional Layers:** These layers apply filters to the image to detect features like edges or textures. Each filter looks for specific patterns.
3. **⚡ Activation Function (ReLU):** After applying filters, an activation function is used to introduce non-linearity into the model, helping it learn complex patterns.
4. **🤖 Fully Connected Layers:** The features extracted by the convolutional layers are then passed through fully connected layers that make the final decision about whether the image is real or fake.

---

## 🎓 Training Process

- The researchers trained **36 different versions** (topologies) of their CNN model to find the best-performing one.
- They used a process called **hyperparameter tuning**, which involves adjusting settings in the model to improve its accuracy.

---

## 📊 Results

> The best model achieved an impressive accuracy score of **92.98%** 🎯, meaning it correctly classified nearly 93 out of every 100 images as either real or AI-generated.

---

## 💡 Explainable AI

To understand how the model made its decisions, the researchers implemented a technique called **Gradient Class Activation Mapping (Grad-CAM)**. This method highlights parts of an image that were important for the model's classification decision. Interestingly, they found that the model relied on small imperfections in the background rather than the main subject of the image to determine if it was real or fake.

---

## 🔑 Key Technical Terms Explained

- **🧠 Artificial Intelligence (AI):**  
  The simulation of human intelligence processes by machines, especially computer systems.
- **🖼️ Synthetic Images:**  
  Images created by algorithms rather than captured by cameras.
- **🤖 Convolutional Neural Network (CNN):**  
  A type of deep learning model specifically designed for processing structured grid data like images.
- **🌌 Latent Diffusion Models (LDMs):**  
  A generative model that creates new data points from existing data by reversing a process that adds noise to images.
- **⚙️ Hyperparameter Tuning:**  
  The process of optimizing parameters within a machine learning algorithm to improve performance.
- **🔍 Explainable AI (XAI):**  
  Techniques that make it easier to understand how AI models make decisions.

---

## 🏁 Conclusion

This research represents a significant step forward in distinguishing between real and AI-generated images. By creating a robust dataset and employing advanced machine learning techniques, Bird and Lotfi provide valuable insights into the capabilities and limitations of current AI technologies in image generation and classification. Their findings underscore the importance of developing reliable methods for verifying image authenticity in an era where synthetic imagery is increasingly prevalent.
