# **Online Learning – Quick Revision Notes**

## **1. What is Online Learning?**

Online Learning is a machine learning approach where a model **learns continuously from new data** instead of training again on the complete dataset.

- Model learns from individual data points or small batches.
- New data updates the existing model.
- Useful when data changes frequently.

**Example:** A fraud detection model learns from new transaction patterns.

## **2. How does it work?**

**Initial Training**

**Deploy Model**

**New Data Arrives**

**Incremental Training**

**Updated Model → Repeat**

## **3. When should we use it?**

1. **Changing data patterns:** When user behaviour or data changes frequently.
2. **Very large datasets:** When the entire dataset cannot fit into RAM.
3. **Continuous data:** When new data keeps arriving, such as transactions.

## **4. Important concepts**

| Concept                 | Meaning                                                           |
| ----------------------- | ----------------------------------------------------------------- |
| Incremental Learning    | Learning from new data without starting from scratch              |
| Concept Drift           | Data patterns change over time                                    |
| Learning Rate           | Controls how much the model updates its parameters                |
| Catastrophic Forgetting | Model forgets previously learned patterns while learning new ones |
| RAM                     | Memory used to store data while processing                        |

### **Learning Rate**

- High learning rate → Learns quickly but may become unstable.
- Low learning rate → Learns slowly but makes smaller updates.

## **5. Python implementation**

Scikit-learn supports incremental learning using `partial_fit()`.

```
from sklearn.linear_model import SGDClassifiermodel = SGDClassifier()# First batchmodel.partial_fit(    X_batch1,    y_batch1,    classes=[0, 1])# Second batchmodel.partial_fit(X_batch2, y_batch2)# Third batchmodel.partial_fit(X_batch3, y_batch3)
```

**Remember:**

- `partial_fit()` updates the existing model.
- `classes` specifies all possible target classes on the first call.

## **6. Libraries**

- **River:** Python library for online machine learning.
- **Vowpal Wabbit:** Efficient library for large-scale online learning.

## **7. Advantages and Disadvantages**

| Advantages                        | Disadvantages                   |
| --------------------------------- | ------------------------------- |
| Learns from new data              | More complex to implement       |
| Adapts to changing patterns       | Needs continuous monitoring     |
| Handles large datasets in batches | Bad data can affect the model   |
| Can reduce repeated training cost | Risk of catastrophic forgetting |

## **8. Batch Learning vs Online Learning**

| Batch Learning                 | Online Learning             |
| ------------------------------ | --------------------------- |
| Trains on the complete dataset | Learns incrementally        |
| Retrains periodically          | Updates as new data arrives |
| Suitable for stable data       | Suitable for changing data  |
| Simpler to manage              | Needs more monitoring       |

## **9. Important interview question**

**What is the difference between Online Learning and Partial Training?**

- Online Learning is a machine learning approach where the model learns continuously from incoming data.
- Partial Training means training a model using portions of a dataset.
- Partial training alone does not mean online learning. It can also happen during offline training.

## **Last-minute revision**

**Remember these 8 points:**

1. Online Learning = Continuous learning.
2. Learns from new data or small batches.
3. `partial_fit()` updates an existing model.
4. Concept Drift = Changing data patterns.
5. Learning Rate = Controls the size of updates.
6. Catastrophic Forgetting = Forgetting old patterns.
7. Libraries = River and Vowpal Wabbit.
8. Monitor data quality and model performance.

   **Easy memory trick:**

Batch: Complete Data → Train → Deploy → Retrain

Online: New Data → Learn → Update → Repeat
