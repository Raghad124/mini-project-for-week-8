Mini Project – Week 8: Linear Transformation Pipeline
📌 Project Overview

This mini-project demonstrates a complete linear transformation pipeline using NumPy, covering the core computations behind dense layers in neural networks and linear regression.

🚀 Pipeline Steps

🟢 Data Creation

Generate a batch of input samples 
𝑋
X with multiple features.

🔵 Standardization

Standardize each feature column to have mean = 0 and std = 1.

Formula:

𝑋
std
=
𝑋
−
mean
(
𝑋
)
std
(
𝑋
)
+
𝜖
X
std
	​

=
std(X)+ϵ
X−mean(X)
	​


🟡 Linear Transformation

Apply a linear layer using matrix multiplication:

𝑌
=
𝑋
std
@
𝑊
+
𝑏
Y=X
std
	​

@W+b

𝑊
W = weight matrix

𝑏
b = bias vector

Maps input features to output features for each sample.

🟣 Normalization (Optional)

Normalize each row of 
𝑌
Y to unit length for downstream tasks or visualization:

𝑌
norm
=
𝑌
∥
𝑌
∥
row
+
𝜖
Y
norm
	​

=
∥Y∥
row
	​

+ϵ
Y
	​


⚡ Vectorized Implementation

All operations are vectorized using NumPy (no Python loops) for speed and readability.

🛠️ Shape Debugging

Check shapes at each step.

Ensure proper broadcasting to prevent errors.

🎯 Learning Objectives

Understand matrix multiplication for linear transformations.

Apply standardization and normalization in feature processing.

Use broadcasting for bias addition and row-wise operations.

Recognize and debug shape errors in ML pipelines.

Build a fully vectorized linear transformation pipeline
