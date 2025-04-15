# ML
Machine Learning Transformers - Explanation
<br>
1️⃣ Introduction to ML Transformers
In Machine Learning, transformers are tools that help modify or process data before training a model.
🔹 They prepare data to improve accuracy.
🔹 They convert raw data into a better format for the ML model.
<br>
For example:

If the data has big and small numbers, transformers can scale them so they are balanced.

If there are text labels, transformers can convert them into numbers so that ML models can understand them.

2️⃣ Types of ML Transformers
📌 Feature Scaling (Making Data Balanced)
Some data has very big numbers (like 1000, 5000) and some have small numbers (like 0.5, 1.2). This can confuse ML models. Scaling helps fix this problem.
<br>
🚀 Types of Scaling Transformers:

StandardScaler – Converts data so that it has mean = 0 and standard deviation = 1.

MinMaxScaler – Converts all values between 0 and 1.

RobustScaler – Useful when data has outliers (extreme values).
<br>
📌 Power Transformation (Making Data Normal)
Sometimes, data is not normal (it has too many extreme values). Power Transformers convert data into a normal distribution, which helps ML models perform better.

🚀 Types of Power Transformers:

Box-Cox Transformation – Works for positive values.

Yeo-Johnson Transformation – Works for both positive and negative values.
<br>
🔹 Why is this useful? Some ML models (like Linear Regression) work best with normal data.

📌 Encoding (Converting Text into Numbers)
ML models cannot understand words, so we need to convert them into numbers.

🚀 Types of Encoding:

Label Encoding – Assigns a unique number to each category. Example: "Red" → 0, "Blue" → 1, "Green" → 2.

One-Hot Encoding – Creates separate columns for each category with 0 and 1.

🔹 Why is this useful? ML models only work with numbers, so we must convert text into a numeric form.

📌 Dimensionality Reduction (Making Data Simpler)
If a dataset has too many columns, it can make ML models slow and inefficient. Dimensionality reduction removes unnecessary features while keeping the most important ones.

🚀 Types of Dimensionality Reduction:

PCA (Principal Component Analysis) – Reduces columns while keeping important information.

t-SNE (t-Distributed Stochastic Neighbor Embedding) – Helps visualize high-dimensional data.

LDA (Linear Discriminant Analysis) – Useful for classification problems.

🔹 Why is this useful? It makes data faster to process and improves model performance.

3️⃣ How ML Transformers Work?
ML transformers follow a simple process:

🔹 Step 1 – fit(): The transformer learns from the data.
🔹 Step 2 – transform(): The transformer modifies the data.
🔹 Step 3 – fit_transform(): Does both fit() and transform() in one step.
