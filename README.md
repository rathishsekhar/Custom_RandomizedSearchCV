# Custom_RandomizedSearchCV README

Project Name: Custom RandomizedSearchCV Implementation - Building a custom RandomizedSearchCV with its functions similar to that of sklearn.model_selection.RandomizedSearchCV

# Table of Contents
1. Overview
2. Prerequisites
3. Project Structure
4. Input
5. Model
6. Setup
7. Usage
8. Results
9. Contributing
10. License

# Overview

This project represents the author's attempt to create custom code for Randomized Search Cross-Validation (RandomizedSearchCV), similar to `sklearn.model_selection.RandomizedSearchCV`. The primary goal is to use this custom code to determine the optimal hyperparameters for the K-Nearest Neighbors (K-NN) algorithm.

The author undertakes this exercise for the purpose of practice and gaining a deeper understanding of the concepts related to RandomizedSearchCV and hyperparameter selection. By implementing the code personally, the author aims to grasp the fundamentals of hyperparameter tuning and how a simple hyperparameter can be generated.

It's important to note that this custom RandomizedSearchCV implementation serves as a personal exploration and does not introduce additional features beyond what is available in the `scikit-learn` module.

The objectives of this project are:

1. Write custom code for RandomiZedSearchCV.
2. Utilize the custom RandomizedSearchCV code to discover the best hyperparameter for a K-NN classifier applied to self-generated classification data.
3. Visualize the classification hyperplanes using the best hyperparameter.


# Prerequisites

Python 3.6 or later preferably
Jupyter Notebook
Libraries listed in requirements.txt

# Project Structure

The project structure is organized as follows: \
├── notebooks \
│─├── CountVectorizer.ipynb \
├── README.md \
├── requirements.txt \
└── LICENSE \


# Input

This project involves working with self-generated classified data using the 'sklearn.datasets.make_classification' module, therefore no external data is used. The dataset comprises 10,000 data points, each with two features, making it suitable for easy visualization. While some parameters for generating the classification data have been preconfigured, users have the flexibility to modify these values as needed.

The dataset is generated using 'sklearn.datasets.make_classification. A total of 10,000 data points with two features are inputted.

## Customization

One of the key features of this project is the ability for users to customize the dataset generation process. The user of this code is therefore encouraged to explore different sample sizes, feature dimensions, or class configurations,


# Model
1. K-NN (k-Nearest Neighbour Classifier)
2. Accuracy score (Sci-kit learn)

# Setup

1. Clone this repository to your local machine:
git clone https://github.com/rathishsekhar/Custom_RandomizedSearchCV.git

2. Navigate to the project directory:
cd Custom_RandomizedSearchCV

3. Install the required Python packages:
pip install -r requirements.txt

# Usage

For exploring the tasks, refer to the jupyter notebook - notebooks/RandomizedSearchCV.ipynb

# Ethical Considerations
This project strictly adheres to ethical guidelines and practices:

1. **No User Data Used:** We want to emphasize that no user data has been used in the development or testing of this project. We are committed to safeguarding user privacy and ensuring that any data used is anonymized and ethically sourced.

2. **For Learning Purposes:** This project is created solely for educational purposes. Our primary goal is to provide a resource for learning and understanding the inner workings of RandomizedSearchCV. We encourage responsible and ethical use of this knowledge in real-world applications.

3. **Transparency:** We are dedicated to transparency in our project's goals and functionality. We encourage open discussion and feedback to ensure that our project aligns with ethical best practices.

We welcome collaboration and contributions from the community to help improve this project's ethical stance and effectiveness.

# Results

This project has achieved the significant results:
1. **Customized RandomizedSearchCV Implementation**: We have successfully implemented a custom RandomizedSearchCV, offering flexibility and control over hyperparameter tuning for machine learning models.

2. **Optimal Hyperparameter for K-NN Classifier**: Utilizing our custom code, we identified and applied the best hyperparameter configuration for the K-Nearest Neighbors (K-NN) classifier. This optimization enhances the classifier's performance.

3. **Visualization of Classification Hyperplanes**: With the best hyperparameter in hand, we have created visualizations of the classification hyperplanes. These visualizations provide insights into how the K-NN classifier distinguishes between different classes in the generated dataset.

Feedback and contributions are highly encouraged. 


# Maintainance and Updates

This project is a product of continuous learning and improvement. For now, there are no updates required howevever, your feedback, suggestions, and contributions are highly valued. If you have ideas, encounter issues, or want to collaborate, please don't hesitate to reach out. Together, we can continue to improve and refine this project.

# Contributions
Contributions to this project are welcome. To contribute:

Fork the repository.
Create a new branch for your feature: git checkout -b feature-name
Make your changes and commit them: git commit -m 'Add feature-name'
Push to your branch: git push origin feature-name
Create a pull request.

# License

This project is licensed under the MIT License. Feel free to use and modify the code as needed.
Feel free to adapt this README template to your specific data science project. It provides a clear structure and information for users and collaborators to understand and contribute to your project effectively