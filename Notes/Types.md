# Supervised Machine Learning – Quick Explanation

**Supervised Machine Learning (ML)** is a type of machine learning where we train a model using **labeled data**.

In simple words:

We give the machine:

1. Input data (questions).
2. Correct answers (labels).
3. The machine learns the relationship between inputs and outputs.
4. Later, it predicts answers for new, unseen data.

## 1. Simple example

Imagine we want to predict house prices.

| House size (sq. ft.) | Actual price |
| -------------------- | ------------ |
| 500                  | ₹20 lakh     |
| 800                  | ₹35 lakh     |
| 1000                 | ₹45 lakh     |
| 1500                 | ₹70 lakh     |

We give this data to a machine learning algorithm.

The model learns how house size relates to price.

Now, if we provide a new house size of 1200 sq. ft., the model predicts its price.

(Learning from examples with correct answers)

## 2. Types of Supervised Learning

There are two major types:

**1. Regression**

Used when we want to predict a **continuous numerical value**.

Examples:

- House price prediction.
- Salary prediction.
- Temperature prediction.

**2. Classification**

Used when we want to predict a **category or class**.

Examples:

- Email: Spam or Not Spam.
- Tumor: Benign or Malignant.
- Transaction: Fraud or Not Fraud.

## 3. Important terminology

| Term          | Simple meaning                   |
| ------------- | -------------------------------- |
| Features (X)  | Input variables                  |
| Label (y)     | Correct answer                   |
| Training data | Data used to teach the model     |
| Testing data  | Data used to evaluate the model  |
| Model         | What learns patterns from data   |
| Prediction    | Model's output                   |
| Accuracy      | How many predictions are correct |

## 4. How supervised learning works

**1. Collect labeled data**

Inputs + correct answers

**2. Split the data**

Training data + Testing data

**3. Train the model**

Learn patterns using an algorithm

**4. Make predictions**

**5. Evaluate performance**

## 5. Popular supervised learning algorithms

| Algorithm                    | Used for       |
| ---------------------------- | -------------- |
| Linear Regression            | Regression     |
| Logistic Regression          | Classification |
| Decision Tree                | Both           |
| Random Forest                | Both           |
| K-Nearest Neighbors (KNN)    | Both           |
| Support Vector Machine (SVM) | Both           |
| Naive Bayes                  | Classification |
| Gradient Boosting            | Both           |

# **Types of Machine Learning – Quick Notes**

There are **4 major types of Machine Learning** you should understand first:

**1. Supervised Learning**

Learns from labeled data

Input data is provided along with the correct answers.

Example: Predicting house prices, spam detection.

**2. Unsupervised Learning**

Learns from unlabeled data

The model tries to discover patterns, groups or relationships in data without being given the correct answers.

Example: Customer segmentation.


**3. Semi-Supervised Learning**

Learns from both labeled and unlabeled data

Uses a small amount of labeled data and a large amount of unlabeled data.

Example: Image classification with only a few labeled images.


**4. Reinforcement Learning**

Learns through rewards and penalties

An agent learns by taking actions and receiving feedback from its environment.

Example: Training a robot or a game-playing AI.

# **1. Unsupervised Learning**

## **What is Unsupervised Learning?**

Unsupervised learning is a type of machine learning where the model learns from **unlabeled data**.

We don't provide the model with the correct answer for every data point. Instead, the model tries to find hidden patterns, similarities, groups or relationships within the data.

### **Example: Customer segmentation**

Imagine an online shopping company has data about 10,000 customers.

| Customer | Monthly spending | Shopping frequency |
| -------- | ---------------- | ------------------ |
| A        | ₹5,000           | 20                 |
| B        | ₹500             | 2                  |
| C        | ₹4,500           | 18                 |
| D        | ₹800             | 3                  |
| E        | ₹10,000          | 30                 |

We don't tell the model which customer belongs to which group.

The model may discover:

- Group 1: Frequent shoppers who spend a lot.
- Group 2: Customers who shop occasionally and spend less.
- Group 3: Customers who spend very large amounts.

The model discovers these groups based on similarities in the data.

This process is called Clustering.

## **Types of Unsupervised Learning**

There are several important approaches.

### **1. Clustering**

Clustering means grouping similar data points together.

The algorithm identifies similarities in the data and places similar points into the same group.

**Example:**

A company groups customers based on:

- Age
- Spending
- Shopping frequency
- Product preferences

The company can use these groups for targeted marketing.

| Algorithm               | Simple explanation                                |
| ----------------------- | ------------------------------------------------- |
| K-Means                 | Divides data into K groups                        |
| Hierarchical Clustering | Creates groups in a hierarchy, like a tree        |
| DBSCAN                  | Groups nearby data points and identifies outliers |

Common algorithms: K-Means, Hierarchical Clustering, DBSCAN.

### **2. Dimensionality Reduction**

Dimensionality reduction means reducing the number of features (columns) in a dataset while trying to preserve the most important information.

Imagine a dataset containing 100 features.

Instead of working with all 100 features, we try to represent the data using fewer features, perhaps 10, while retaining as much useful information as possible.

**Why do we use it?**

- Reduce complexity.
- Speed up computation.
- Visualize high-dimensional data.
- Reduce noise and redundant information.

| Algorithm | Simple explanation                                                    |
| --------- | --------------------------------------------------------------------- |
| PCA       | Creates fewer new features that capture much of the data's variation  |
| t-SNE     | Helps visualize complex data in 2D or 3D                              |
| UMAP      | Reduces dimensions while often preserving local and broader structure |

Common algorithm: PCA (Principal Component Analysis).

### **3. Association Rule Learning**

Association learning discovers relationships between items.

**Example:**

A supermarket analyzes shopping transactions and discovers:

> Customers who buy bread frequently also buy butter.

The model discovers patterns in what items are purchased together.

This is also called **Market Basket Analysis**.

| Algorithm | Purpose                             |
| --------- | ----------------------------------- |
| Apriori   | Finds frequent item combinations    |
| FP-Growth | Finds frequent patterns efficiently |

Example application: Product recommendations.

### **4. Anomaly Detection**

Anomaly detection identifies data points that behave differently from normal data.

**Example: Fraud detection**

A customer usually spends ₹500–₹2,000 per transaction.

Suddenly, a transaction of ₹1,00,000 occurs in another location.

The system may identify this transaction as unusual.

| Algorithm        | Purpose                                          |
| ---------------- | ------------------------------------------------ |
| Isolation Forest | Identifies unusual data points                   |
| One-Class SVM    | Learns normal patterns and identifies deviations |

Applications: Fraud detection, network security, abnormal system behavior.

Note: Anomaly detection is often taught under unsupervised learning, but it can also use labeled or semi-supervised approaches.

# **2. Semi-Supervised Learning**

## **What is Semi-Supervised Learning?**

Semi-supervised learning uses a combination of:

- Small amount of labeled data
- Large amount of unlabeled data

It is useful when collecting data is easy but labeling that data is expensive or time-consuming.

### **Example: Image classification**

Imagine you have 10,000 images of animals.

| Data             | Quantity |
| ---------------- | -------- |
| Labeled images   | 500      |
| Unlabeled images | 9,500    |

Labeling images manually requires time.

Instead of labeling all 10,000 images, we label 500 images and use the unlabeled images to help the model learn additional patterns.
### **How it works**

**Small labeled dataset**

Images + correct labels

**Large unlabeled dataset**

Images without labels

**Semi-Supervised Model**

Uses both datasets to improve learning

### **Applications**

- Image recognition.
- Speech recognition.
- Medical image analysis.
- Text classification.

### **Why use Semi-Supervised Learning?**

| Supervised                               | Semi-Supervised                            |
| ---------------------------------------- | ------------------------------------------ |
| Requires labeled data for training       | Uses both labeled and unlabeled data       |
| Labeling large datasets can be expensive | Can reduce labeling requirements           |
| Learns from labeled examples             | Can use unlabeled data to improve learning |

The goal is to improve learning without labeling every data point.

# **3. Reinforcement Learning (RL)**

## **What is Reinforcement Learning?**

Reinforcement Learning is a type of machine learning where an **agent learns by interacting with an environment and receiving rewards or penalties**.

Instead of being given the correct answer directly, the agent tries actions, observes the results and learns which actions are better.

### **Example: Training a robot**

Imagine training a robot to walk.

- If it moves successfully → reward.
- If it falls → penalty.
- It tries different actions.
- Over time, it learns which actions help it walk successfully.

## **Important terms in Reinforcement Learning**

| Term        | Simple meaning                            |
| ----------- | ----------------------------------------- |
| Agent       | The learner or decision-maker             |
| Environment | The world in which the agent operates     |
| State       | The current situation                     |
| Action      | What the agent chooses to do              |
| Reward      | Feedback for an action                    |
| Policy      | Strategy the agent uses to choose actions |

## **How Reinforcement Learning works**

### **Agent**

Chooses an action

### **Environment**

Responds to the action

### **Reward + New State**

Agent receives feedback

**Agent improves its strategy**

It repeats this process to improve its future actions.

## **Example: Game-playing AI**

Imagine an AI playing a game.

| Action             | Outcome  | Reward |
| ------------------ | -------- | ------ |
| Moves toward goal  | Progress | +10    |
| Hits an obstacle   | Failure  | -5     |
| Completes the game | Success  | +100   |

The AI tries different actions and learns a strategy that maximizes its total reward over time.

## **Types / popular algorithms in Reinforcement Learning**

| Algorithm            | Simple explanation                                            |
| -------------------- | ------------------------------------------------------------- |
| Q-Learning           | Learns how valuable different actions are in different states |
| SARSA                | Learns using the action it actually takes next                |
| Deep Q-Network (DQN) | Uses a neural network to learn action values                  |
| Policy Gradient      | Learns a policy directly                                      |
| PPO                  | A popular method for improving policies more stably           |

### **Applications**

- Robotics.
- Game AI.
- Self-driving research.
- Resource optimization.
- AI agents.

# **4. Compare all four types**

| Type            | Data / feedback          | How it learns               | Example               |
| --------------- | ------------------------ | --------------------------- | --------------------- |
| Supervised      | Labeled data             | Learns from correct answers | Predict house prices  |
| Unsupervised    | Unlabeled data           | Finds patterns and groups   | Customer segmentation |
| Semi-Supervised | Labeled + unlabeled data | Uses both to learn          | Image classification  |
| Reinforcement   | Rewards and penalties    | Learns through interaction  | Game-playing agent    |

# **5. Interview-ready explanation**

**Q: Explain the four types of machine learning.**

"Machine learning is broadly divided into four types.

- Supervised learning learns from labeled data and is used for regression and classification.
- Unsupervised learning learns from unlabeled data and discovers patterns, clusters or relationships.
- Semi-supervised learning combines a small amount of labeled data with a large amount of unlabeled data.
- Reinforcement learning involves an agent interacting with an environment, taking actions and learning from rewards or penalties."

# **6. Quick revision cheat sheet**

**Supervised → Learn from answers**

Regression + Classification

**Unsupervised → Find hidden patterns**

Clustering + Dimensionality Reduction + Association + Anomaly Detection

**Semi-Supervised → Learn from few answers + many unanswered examples**

**Reinforcement → Learn through rewards**
