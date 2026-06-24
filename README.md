#  Fashion MNIST Classification Workflow

An end-to-end machine learning classification project implementing the complete Chapter 3 workflow from *Hands-On Machine Learning with Scikit-Learn, Keras & TensorFlow* by Aurélien Géron.

##  Objective

Build and evaluate multiple machine learning models on the Fashion MNIST dataset while exploring the complete classification pipeline, including model evaluation, threshold tuning, multiclass classification, and error analysis.

##  Repository Structure

fashion-mnist-classification-workflow/

├── README.md

├── fashion_mnist_classification.ipynb

├── images/

│   ├── fashion_samples.jpg

│   ├── roc_curve.jpg

│   ├── confusion_matrix.jpg

│   └── error_analysis.jpg

└── requirements.txt

##  Dataset

Fashion MNIST consists of 70,000 grayscale images of clothing items across 10 categories:

* T-shirt/top
* Trouser
* Pullover
* Dress
* Coat
* Sandal
* Shirt
* Sneaker
* Bag
* Ankle Boot

Each image is represented as a 28×28 pixel grayscale image.

##  Models Evaluated

* SGD Classifier
* Random Forest Classifier
* K-Nearest Neighbors (KNN)
* One-vs-Rest Support Vector Classifier (OvR SVC)

##  Topics Covered

### Binary Classification

* Shirt vs Rest classification
* Precision
* Recall
* F1 Score
* Precision–Recall Tradeoff

### Model Evaluation

* ROC Curves
* ROC AUC
* Cross Validation
* Confusion Matrix Analysis

### Multiclass Classification

* One-vs-Rest Strategy
* Model Comparison
* Error Analysis

### Hyperparameter Tuning

* GridSearchCV
* Random Forest Optimization

##  Results

| Model          | Accuracy |
| -------------- | -------: |
| Scaled OvR SVC |   86.33% |
| OvR SVC        |   86.15% |
| Random Forest  |   85.87% |
| KNN            |   81.92% |
| OvR SGD        |   81.95% |

Best Performing Model:

**Scaled OvR SVC — 86.33% Accuracy**

##  Key Findings

* Accuracy alone is insufficient for evaluating classifiers.
* ROC AUC provides deeper insight into ranking performance.
* Threshold tuning significantly affects precision and recall.
* The most challenging Fashion MNIST classes were:

  * Shirt ↔ T-shirt/top
  * Pullover ↔ Coat
  * Sneaker ↔ Ankle Boot
* Error analysis revealed semantically meaningful mistakes rather than random misclassifications.

##  Tech Stack

* Python
* NumPy
* Pandas
* Matplotlib
* Scikit-Learn
* Jupyter Notebook

##  Learning Outcome

This project strengthened my understanding of:

* Classification workflows
* Model evaluation metrics
* Hyperparameter tuning
* Multiclass classification strategies
* Error analysis and model interpretation

---

Built as part of my machine learning journey through *Hands-On Machine Learning* by Aurélien Géron.
