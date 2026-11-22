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

[What is the definition and intuition behind PAC learning? | by Samiran Pal | FAQK like Socrates | Medium](https://images.openai.com/static-rsc-4/95ahm6Vt21OOuNatAr7fU7mQ3PiHbzm68sFvtRC_nXt3LiEhWtUQ233_ik1yhnJC8f6TJz_QnDMjMikADu616uswfFMa8s25xVEIX-u0tNJN7_fFF4bT-bED30qowerFnDJR9eWgvgvjuzmR_V7MD1ve0Kyje6eDtKynCnWu0VU?purpose=inline)

**1. Supervised Learning**

Learns from labeled data

Input data is provided along with the correct answers.

Example: Predicting house prices, spam detection.

[Discovering the Unknown: Clustering in Unsupervised Learning | by LoryneJoy | Medium](https://images.openai.com/static-rsc-4/Jkht1XsY0J2ZmRcnvrCocg2cecVpbc5T69_OTQ9oIjXR6nGlFk9kJ0Wal1upxMrEwnZvlN63wVlsaMiPhqtzGe47HFJCpW-cs5NaJ-RNoOnq-qQ49C-Izu9PGsxkjgiaM_0ywX_2ITJ7tWtpXkKYjBCK9LEvb4IPV6zn3_Q857g?purpose=inline)

**2. Unsupervised Learning**

Learns from unlabeled data

The model tries to discover patterns, groups or relationships in data without being given the correct answers.

Example: Customer segmentation.

[Semi-Supervised Learning: The Bridge Between Supervised and Unsupervised Learning | by Dr. Fatih Hattatoglu | Academy Team | Medium](https://images.openai.com/static-rsc-4/l91Z8-IsIyUr9keQeRDglZLsfogEjl2DQqUIUfvA1tzDH9AnqcmJB13WTTO4opsxkanloPhLucjoZkRHpwFAxp9FoNho0ZQaghp8oJ0nt4v83WFxndg4hhDvQje9GK3alGDnYULrYZISpwPWJhao35vUvljHuRi7Ppm2kKoSBkI?purpose=inline)

**3. Semi-Supervised Learning**

Learns from both labeled and unlabeled data

Uses a small amount of labeled data and a large amount of unlabeled data.

Example: Image classification with only a few labeled images.

[Reinforcement Learning: The Future of Intelligent Decision-Making](https://images.openai.com/static-rsc-4/_VWbANmsop6aEHFRrqu78ZlCEIHd_LJGfULKFY-JW9T9wu1MbGHMmRwcwkQoc8raFZ7GT6bfNlfET1if2inKHPY4DPw7jIDqzmXAwGXqufq2sJ8Dd7jRvUxGnRQogT2loHf233wdyX1DRwyYLxHofGyqrth0YUZPfAQTQo_BXJA?purpose=inline)

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

[How to use Data Science to better understand your customers](https://images.openai.com/static-rsc-4/oaskavKJgjH1pxubI9zy1r1gBl_WHSTGYrKW0hwNslwsoK8UF0fvbHErLApAa6pWz0zsd2QI8Hsrs32zUT1akdFTYCoghUd1IQ5-iw-D3vtd4EVTUmyZpPgz1wPszQ1UT_313wWSAJIKDLhWChksKGxA0GmNEtzwrq2Za8gqyOY?purpose=inline)

[A Workflow for Segmenting Customers with Clustering](https://images.openai.com/static-rsc-4/RVWB1R6xNDgn2PBpY4_-aTbUbPyLCaL7nTdlIM6uFfw2V_G-coaYdNlFvhhcyezbt27eMytQqbgLHB1TCBt4Jlt2319G0nqp7zxAJC8Dvq7F2IFI7t8Tt_JjG4MpUVGDMAqqfaGqZsEyf7Hr3hPaYtxe03B4fKmEh5WodBb5XtI?purpose=inline)

[Customer Segmentation and Analysis Project](https://images.openai.com/static-rsc-4/dsiC7yAB8YVS-fOSwDZTsmywl1Y9aF_yopGpnhXNkbLh6MUZeA3Cn1f6mmM3528L9BDcQqwk8jOifm-HP2SIUfvBLbSEKuWeHTKT3e3GztQTgMnrH47B9z2zQ-ux2egZMIuC6oBPL_vOlE7rhbhAHGZiu_x1etm2P1mHRCrvLfU?purpose=inline)

6

This process is called Clustering.

## **Types of Unsupervised Learning**

There are several important approaches.

### **1. Clustering**

[K-means and Hierarchical Clustering](https://images.openai.com/static-rsc-4/u3dehJyTM5Rh8h1uWXSWrc5tcV-pdsuqsxeSuI-laa7QQ8G29LMMNUvDtFgtg4D-xJX3hySuC9vhd-LTBYbBXGJifL9isZwL8BHEuUanmROTot-SJV8uWFlNgl491NuN9IyAJq1Hk3SkrtHInatT4pOKfDd3UDKncpQQ6J3H_jg?purpose=inline)

[Display K-Means Cluster at Justin Northcote blog](https://images.openai.com/static-rsc-4/1UhhDcqj8jl6ZcCYys5F0PK4X3onkiZO0v9zfZuUutaQTwNZZgk0KGswugcKcGgw3bq9TvVODwz747Strh2nm3bC-pvSkK6Cre4G6vwkA_RXQ7KFvWIm7p47Rmh_g7DNAD-yXNMrzLVfaYSZJC88HQw0KHht0ecawxlsp3k_VOk?purpose=inline)

[Machine Learning Algorithms Explained: Clustering - StrataScratch](https://images.openai.com/static-rsc-4/SdLwrsXP4R-nQ0Q8xMJDIW5KaVu_ItQrtKNoFbWDm6sQnGP8UYAsARNz_a4eehAdE_E9cf4juagE3B0tF2I6WJfr69pRCG6_AvapFzPIDTxG28fJqYpPaiRzpioG0Z00QE2C32kNlVtRIu2u6ytoWbIvs5g_SNbU1QKtsQU8SmM?purpose=inline)

6

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

[Semantic Analysis of Moby-Dick with TF‑IDF | by Roblesjeison | Medium](https://images.openai.com/static-rsc-4/cMiaUZsrvBvrqjTIyG4YSDRj0G3lMnhJ6DxINkRKpXenkcO9PO-vZugRZFwrUPBHZSXek2chD8mmWZde0Tw7cuiQvwWRYgyTeeLEMHWcmL5RR6PM9QLvx91y3ZMqGrYgrwoW5Tqix9Sjid2REpFfsIOs7peEYOIfNxWjD1RXV4I?purpose=inline)

[UMAP: The Fast, Powerful Technique Behind Modern Dimensionality Reduction | by Roshmita Dey | Medium](https://images.openai.com/static-rsc-4/XKzVtuflSiQ1LGSHqE_0L0jx9KDfbWs1LvgSgut5f-K_q748vkQHiQUZtfqwzy6FyYe-TtW3KdaCNSvsMzTqcYILMJCgvfIGMLKlQLn-eJktahrj8sv4IPbZFX68UtULnTSA3yJ7QDtnOqypfE6IQVHwHTx3k-9kCSpEIEunwMQ?purpose=inline)

[Principal Component Analysis (PCA): Understanding High-Dimensional Data Through Projection](https://images.openai.com/static-rsc-4/FFhsXlsD_CB5Ql1MSW2q5qGGIph9eKPPAlFHI3Z8WnJuNLD4CWSPy00RB2JyaOC3zSj94tJmjdimb5ojb7mUj8a1X6-b27eidkBrUYisYrEU8fWd78ErqyScitGeQtd193l0VsVczF0I57SmPwQ8ng4podUoClNY4l61xlZ0lXU?purpose=inline)

7

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

[Market Basket Analysis using Apriori Algorithm | by Dhaval Bagal | Medium](https://images.openai.com/static-rsc-4/5OblIyyF46IqXw7tV-F9I-74wwe-l_4_mgcpEkt34OxdzZapOa1iPqLbkbIIrTu_ve8qUAF2JWiY3mEQ-Cj0XnfP-iE8DOdByiw-xRrmvsGWI7ng1zzI2Y3-IWLb9eelelIXy0iSuIBj6pNgm6527m_y6XQnjY9GDqzMQ3XZ6PE?purpose=inline)

[Conditional Probability Application: Association Rule Learning](https://images.openai.com/static-rsc-4/0II0gytflLYgBacXb8LAGWpQBksiuQLhtngTAMcXPs-oQwx0okWMFPV8LpJVRZRgOSdoHe6igtvZOEPc3xl9NV4HXKHpGpqGABEXu2L2JUvT1lH4dzSJjyjJgftX6X8AGLkXVFXApZstJ0y-eMIqd5Su7fsGyhe8g2BR8ebpSCs?purpose=inline)

[PPT - MIS2502: Data Analytics Association Rule Mining PowerPoint Presentation - ID:2833458](https://images.openai.com/static-rsc-4/1hzVBdp8-gdfMnBAg1gcj-9iVvEM4dxAXKe6nYizlUH91YdX2FajvB66rv4QfpR15KoZsNIOhQYW7XcXdeb6tkIgOrCP3PiT4lIJwZO00pAL2lHn9poAGs5NqKpJHwFs6uZAP7Pezpjwmyz3qTVoK_zFde-UHYbfxNlL7IX-kPM?purpose=inline)

9

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

[5.3.4 Anomaly Detection | AI Roads](https://images.openai.com/static-rsc-4/dGxe5nj8VutITz_3DLkfSblTEv_RLMU08UFxsmzITmhMQMsJLg8C2JtNZHFtF1N-kjW8YTjktwNUE99lqVl42ZLPyf6EfMlGYUogrPGOzQFxu07VIbAOZu9qlf9vElXEP01pIV7S00r56LPOi4EIgHR3a4ZuJPehAbLFUk5fYh8?purpose=inline)

[Medium](https://images.openai.com/static-rsc-4/vREeT4v5Ely7Fshq6Ugdm0K4s-DVVa2Bbsay8tuH3ZQYHYK6Sh1Qg7mviczv70pYTCrmEWzijIvtVvQ2ONI5COv3qS0HRR64sNqYVkPgJR3B6rYDA5vD-d87Q0W8S7Ukkc-cttuekZkU78gyeqyNpSHOJm8lpyzcCbY_dkuVRn0?purpose=inline)

[Machine Learning Overview – CS 307 Notes](https://images.openai.com/static-rsc-4/PuzA8PURUe2A8RjqrsuK6cyMqWBlt00k2JvTOxKAMm0FVaXV8CEd50boLDLQPYR7tJgnouRawjrednr70zP5OT5002n4FmukA0DbfuJH28oMpRzyp72XKe18kQk7K1FgvStZQftG5B474w7Cp3MlT22Fb_R0O5lipksoittPv_E?purpose=inline)

7

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

[Deep Learning Exploiting Unlabeled Data Hungyi Lee Introduction](https://images.openai.com/static-rsc-4/sFpOLGA4uqbzYH_yNQ0gyDFJmA4QdiNxKhKc-dqPDlAmLZaGsnuCyYtviYnN-DMxRCJ6bzfF4yPAToSeuEKz7A-KXzl8Lg7GBUDyKGUOartdundv9GRbjh2tJhyP6ZsL0Q1nbgV6cDN5jVkOC5I6Jm0r065faGPhX-AaiifvJNY?purpose=inline)

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

[AI and ML](https://images.openai.com/static-rsc-4/FjMzDxLY3XXaAdKNkISmWIIbGZ0pLSx085_HjBvIoGPyqNT1bPvWcz7xKXIq2Ou8Y79Hk4imM6wKQumNfENHZAFvoew6E5X5Mk-l8AWO-Cd4tZCTxOTlh7Ip7ZTPOf4E51Ue5fyqZucNQMhXsJlxLYFVga6PtTcFAGHDGL_gc6c?purpose=inline)

[Reinforcement Learning Made Clear: States, Rewards, and the Agent’s First Steps | by Nikhil Malkari | Medium](https://images.openai.com/static-rsc-4/CHahpaqOFMPes7Itwn_b_PwvPDnw79Sk9dikSQnmoRRzqTaEPIjfjKd7GO0nq3Ip-lRPKj2DW9nLL-yl39iogVn-lss6wZs0icGENLZiaY_L8f4etTYsfx2w6k6kMvzYBdb91VOyDyN1K1FDBWKl3dBoX1ZcPSMnP1hm3ThLTHU?purpose=inline)

[AI learns to follow predefined norms through a combination of logic and machine learning](https://images.openai.com/static-rsc-4/PwghlMMeI6rISRIStgFEUmHWLJfrikiJAYRLH6V2GzMHpFyM-MPsqRDpx1s44tOIuGuBzsga2_jdngt_moSORYU84sSGfv02KwlqhhGIEpUZuve3YwIse9BbAA_CiIFbliZTDs3oo1h-BLvYi-k9PB0DVe18w_WrLNTl0zfp3h8?purpose=inline)

7

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
