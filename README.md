# Computer Vision: Unsupervised Learning 🖼️🤖

This repository contains the implementation for the **Week 11 Assignment** of the course **DSA4050 - Deep Learning for Computer Vision** under the guidance of **Dr. Edward Ombui**.

## Assignment Overview 🎯

The objective of this assignment was to apply unsupervised learning techniques to computer vision problems, specifically in the context of image data. We used several unsupervised learning techniques to extract meaningful representations from an image dataset and evaluated their effectiveness in image categorization.

## Table of Contents 📚
- [Objective](#objective)
- [Assignment Tasks](#assignment-tasks)
  - [Task 1: Image Data Preprocessing](#task-1-image-data-preprocessing)
  - [Task 2: Clustering for Image Categorization](#task-2-clustering-for-image-categorization)
  - [Task 3: Dimensionality Reduction and Visualization](#task-3-dimensionality-reduction-and-visualization)
  - [Task 4: Contrastive Learning for Representation Learning](#task-4-contrastive-learning-for-representation-learning)
  - [Task 5: Evaluation and Comparative Analysis](#task-5-evaluation-and-comparative-analysis)
  - [Bonus Task (Optional)](#bonus-task-optional)
- [Technologies Used](#technologies-used)
- [Directory Structure](#directory-structure)
- [How to Run](#how-to-run)
- [Results and Report](#results-and-report)
- [License](#license)

## Objective 🎯

The goal of this assignment was to:
- Understand and apply unsupervised learning techniques in computer vision.
- Gain hands-on experience in clustering, dimensionality reduction, and contrastive learning.
- Evaluate and compare different representation learning methods.

---

## Assignment Tasks 📝

### Task 1: Image Data Preprocessing 🖼️

In this task, we:
- Loaded the **Road Crack Image Dataset**.
- Preprocessed the images by:
  - Converting them to grayscale 🖤.
  - Normalizing pixel values 🔄.
  - Applying data augmentation techniques such as rotation 🔄 and flipping 🔁 to enhance the dataset.

### Task 2: Clustering for Image Categorization 🧑‍🤝‍🧑

We performed clustering on the images using:
- **Histogram of Oriented Gradients (HOG)** or deep features extracted from a pretrained CNN 📸.
- Applied **K-Means** and **DBSCAN** clustering algorithms to group similar images.
- Evaluated the quality of the clustering using the **Silhouette Score** 📊.
- Visualized the results by plotting sample images from each cluster.

### Task 3: Dimensionality Reduction and Visualization 🔍

For dimensionality reduction, we:
- Applied **Principal Component Analysis (PCA)** to reduce the feature dimensions 🔽.
- Applied **t-SNE** to further visualize the data in 2D 🌐.
- Compared the results from PCA and t-SNE, providing insights on their effectiveness in clustering visualization.

### Task 4: Contrastive Learning for Representation Learning 🏆

In this task, we:
- Implemented **SimCLR** (a contrastive learning framework) 🧑‍🏫.
- Trained the SimCLR model using contrastive loss to learn image representations 🔍.
- Visualized the learned representations using **t-SNE** 🔬.
- Evaluated the learned representations by training a simple **logistic regression classifier** and comparing the accuracy with and without contrastive learning 📊.

### Task 5: Evaluation and Comparative Analysis 📈

We:
- Compared the performance of **clustering-based methods** (K-Means and DBSCAN) with **contrastive learning-based methods** (SimCLR) 🔍.
- Analyzed which method was more effective for image categorization and why 🔎.
- Provided a report summarizing findings, including methodology, key observations, and performance comparisons.

---

### Bonus Task (Optional) 🎉

For the bonus task, we:
- Explored a **GAN-based unsupervised learning approach** (such as **DeepCluster** or **SelfGAN**) 🎮.
- Compared its performance with **SimCLR** in feature learning ⚙️.

---

## Technologies Used 🛠️

- **Python** 🐍
- **NumPy** 🔢
- **scikit-learn** (for KMeans, DBSCAN, PCA, and t-SNE) 📚
- **PyTorch** (for SimCLR implementation) ⚡
- **OpenCV** (for image preprocessing) 🖼️
- **Matplotlib** (for visualizations) 📊
- **Jupyter Notebook** (for the report and analysis) 📓

---

## Directory Structure 📂

```
DSA4050_w11_Assignment/
├── data/                      # Dataset folder 📂
│   ├── Road Cracks/           # Road Crack dataset 🏞️
├── notebooks/                 # Jupyter notebook 📓
│   ├── DSA4050_W11_Assignment.ipynb
├── requirements.txt           # List of dependencies 📜
├── Week 11 Assignment.pdf     # Assignment Question 📑
```

---

## How to Run 🚀

To run the code:
1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/yourusername/Computer-Vision-Unsupervised-Learning.git
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open the Jupyter Notebook (`Assignment_Week_11.ipynb`) and run the cells to perform each task.
4. If you want to run the script directly, you can execute the corresponding Python files.

---

## Results and Report 📋

A full report and evaluation of the results are available in the **Jupyter Notebook** file `Assignment_Week_11.ipynb`. Key observations include:
- Contrastive learning provided better representations and higher classifier accuracy than clustering-based methods 🏅.
- K-Means and DBSCAN had poor clustering performance on the dataset, with K-Means achieving a low accuracy of 0.09, and DBSCAN failing to detect multiple clusters ❌.
- SimCLR, through contrastive learning, led to more discriminative feature learning, improving the classifier's performance 🔝.

---

## License 📝

For educational and non commercial use only. 

