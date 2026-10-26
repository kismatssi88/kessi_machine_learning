# Topics learned
types of ml on how the model generalizes.

# key concepts:-
# Instance-Based and Model-Based Learning

In machine learning, there are different ways a model can learn from data. Two common approaches are **Instance-Based Learning** and **Model-Based Learning**.

## 1. Instance-Based Learning

Instance-based learning is a type of learning where the algorithm mainly **stores the training examples** instead of trying to build a general model from them.

When a new data point comes, the algorithm compares it with the stored training examples and finds the most similar ones. Based on those similar examples, it makes a prediction.

A common example of instance-based learning is **K-Nearest Neighbors (KNN)**.

### Example

Suppose we have data about students:

```text
Study Hours    Result
2              Fail
4              Pass
6              Pass
8              Pass
```

If a new student studies for 5 hours, KNN looks at the closest examples and uses them to decide whether the student is likely to pass or fail.

### Advantages

* Simple and easy to understand.
* Very little training is required.
* Works well when similar examples usually have similar outputs.

### Disadvantages

* Can require a lot of memory because training examples are stored.
* Prediction can become slow with large datasets.
* Sensitive to the choice of distance measure and irrelevant features.

### Example Algorithm

* K-Nearest Neighbors (KNN)

---

## 2. Model-Based Learning

In model-based learning, the algorithm tries to **learn a general pattern or relationship from the training data**.

Instead of comparing every new data point with all the old examples, the algorithm creates a model using the training data. That model is then used to make predictions on new data.

For example, **Linear Regression** learns a relationship between input and output.

### Example

Suppose we have:

```text
Study Hours    Marks
1              40
2              50
3              60
4              70
```

A linear regression model can learn that marks generally increase as study hours increase.

It may learn a relationship like:

```text
Marks = 30 + 10 × Study Hours
```

Now, if a student studies for 5 hours, the model can use the learned relationship to predict the marks.

### Advantages

* Learns a general pattern from the data.
* Prediction is usually fast after training.
* Usually doesn't need to store all training examples for prediction.
* Can generalize well to new data when the model captures the underlying pattern.

### Disadvantages

* Training can take more time.
* A model that is too simple can **underfit**.
* A model that is too complex can **overfit**.

### Examples

* Linear Regression
* Logistic Regression
* Decision Trees
* Support Vector Machines
* Neural Networks

---

## Main Difference

The easiest way to remember the difference is:

> **Instance-Based Learning:** "Find similar examples and use them."

> **Model-Based Learning:** "Learn a general rule and use that rule."

| Feature        | Instance-Based Learning               | Model-Based Learning                |
| -------------- | ------------------------------------- | ----------------------------------- |
| Main idea      | Uses stored examples                  | Learns a general model              |
| Training       | Mostly stores data                    | Learns parameters/patterns          |
| Prediction     | Compares with examples                | Uses the learned model              |
| Memory         | Can require more memory               | Usually requires less memory        |
| Example        | KNN                                   | Linear Regression                   |
| Generalization | Based on similarity to known examples | Based on patterns learned from data |

## In Short

Both approaches try to solve the same basic problem:

```text
Training Data
      ↓
   Learning
      ↓
Learn something useful
      ↓
   New Data
      ↓
   Prediction
```
-------------------------

# tomorrow:
  Chanllanges in ML.