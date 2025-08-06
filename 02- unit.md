# 🧠 UNIT 2: Artificial Neural Networks (ANN)

---

## 🔹 McCulloch-Pitts Neuron Model

### 🧠 Basic Architecture:

McCulloch-Pitts neuron ek basic model hai jisme inputs, weights (generally +1/-1), ek threshold aur ek binary output hota hai.

### ✅ Formula:

```
Y = 1, agar Σ(wi × xi) ≥ θ
Y = 0, agar Σ(wi × xi) < θ
```

### 🔧 Realization: 3-Input NAND Gate

* Inputs: X1, X2, X3
* NAND ka matlab: agar sab 1 honge, tabhi output 0 hoga, baaki sab me output 1
* Weight (w) = -1 for all inputs
* Threshold (θ) = -2.5

```
Σ = -(X1 + X2 + X3) >= -2.5 → output = 1
Agar X1 = X2 = X3 = 1,
Σ = -3 < -2.5 → output = 0 ✅
```

### 🔧 Realization: 3-Input NOR Gate

* Inputs: X1, X2, X3
* NOR ka matlab: sab inputs 0 hon tabhi output 1, warna 0
* Weight = -1 for all inputs
* Threshold (θ) = -0.5

```
Σ = -(X1 + X2 + X3) >= -0.5
Agar X1=X2=X3=0,
Σ = 0 ≥ -0.5 → output = 1 ✅
```

---

## 🔹 Activation Functions

### 💡 Activation function ka kaam:

Ye decide karta hai ki neuron active hoga ya nahi. Har function ka output style alag hota hai.

| Function | Range    | Graph Shape | Use Case                         |
| -------- | -------- | ----------- | -------------------------------- |
| Step     | 0 or 1   | Threshold   | Simple binary classification     |
| Sigmoid  | 0 to 1   | S-shaped    | Smooth binary outputs            |
| Tanh     | -1 to +1 | S-shaped    | Centered output, faster learning |
| ReLU     | 0 to ∞   | Linear+     | Deep learning (fast & simple)    |

---

## 🔹 Importance of Activation Functions

* Complex patterns learn karne ke liye non-linearity zaroori hai.
* Without activation, NN becomes just a linear model.
* Learning curve smooth hota hai with sigmoid/tanh
* ReLU fast train karta hai deep layers

---

## 🔹 Weight Update Formula (Backpropagation)

### 🔁 Formula:

```
Δw = η × error × input
```

Alternate detailed form:

```
Δw_ij = η × δ_j × o_i
```

* η = Learning rate
* δ\_j = Error term for output neuron j
* o\_i = Output from neuron i

Backpropagation me weights backward adjust hote hain taaki error minimum ho jaye.

---

## 🔹 Architecture of Backpropagation Network

### Layers:

1. **Input Layer** – Features
2. **Hidden Layer(s)** – Pattern recognize karta hai
3. **Output Layer** – Final prediction

### Training Steps:

1. Forward pass – inputs se output generate
2. Error calculate – actual vs predicted
3. Backward pass – error ko back spread karo
4. Weight update – formula se adjustment karo

---

## 🔹 Perceptron Training (With & Without Bias)

### 🧠 What is Perceptron?

Ek simple NN jisme 1 output neuron hota hai. Linear classifier hota hai.

### ✅ Training Rule:

```
w_new = w_old + η × (target - output) × input
```

### ⚙️ With Bias:

Bias ek extra input hota hai jiska weight bhi update hota hai.
Bias help karta hai decision boundary ko shift karne me.

### ⚙️ Without Bias:

Output only depends on weighted sum of inputs.

### Example (AND gate):

```
Inputs: X1, X2 | Target: X1 AND X2
```

Initial weights = 0, Learning rate = 1 → update karte jao till correct output

---

## 🔹 Learning Types

### 1️⃣ Supervised Learning:

* Input ke saath correct output diya jata hai
* Example: Email → Spam or Not Spam

### 2️⃣ Unsupervised Learning:

* Sirf input hota hai, no output
* Goal: Grouping/Clustering
* Example: Market segmentation

### 3️⃣ Incremental Learning:

* Data gradually milta hai
* Model ko baar-baar retrain nahi karna padta
* Example: AI games jisme model game khelte-khelte smarter hota hai

---
