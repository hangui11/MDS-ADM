# Backpropagation Project

### 📦 Required Python Libraries

Make sure the following libraries are installed to run the provided Python code:

* `tensorflow==2.13.1`
* `pandas==2.2.3`
* `numpy==1.24.3`
* `networkx==3.2.1`
* `matplotlib==3.10.1`
* `scikit-learn==1.6.0`

---

## 📂 Contents

This projet assignment includes Jupyter notebooks to execute the code associated with each question (Logic Learning and Gradient Flow):

---

### **`logic_learning.ipynb`**

This notebook demonstrates how a simple neural network can learn basic logic functions (AND, OR, XOR) using TensorFlow/Keras. It covers data generation, model training, evaluation, and visualization of both the decision boundaries and the internal representations of the network:

1. **Importing Libraries and Generating Synthetic Data**
    - Essential libraries are imported: TensorFlow, NumPy, pandas, matplotlib, networkx, and scikit-learn.
    - 10,000 random points are generated for two input variables (x1, x2) in the range [-5, 5].
    - Binary outputs for the logic functions AND, OR, and XOR are created based on the input values.

2. **Preparing Training and Test Sets**
    - The data is organized into a pandas DataFrame.
    - The dataset is split into training (80%) and test (20%) sets.

3. **Defining and Visualizing the Neural Network Architecture**
    - A function is defined to create a simple neural network.
    - Another function visualizes the network architecture and the learned weights/biases using NetworkX.

4. **Training and Evaluating Models for Each Logic Function**
    - For each logic function (AND, OR, XOR):
        - An independent model is trained.
        - Class weights are adjusted to balance the dataset.
        - The model is evaluated on both training and test sets.
        - Results and learned weights/biases are stored.

5. **Visualizing Results**
    - The decision boundary learned by the network is plotted for each logic function.
    - The hidden layer activations are projected using t-SNE to analyze how the network internally separates the classes.
    - The learned weights and biases are visualized on the network architecture.

6. **Saving Results**
    - Final results (accuracy, loss, weights, and biases) are saved to a CSV file.

---

### **`gradient_flow.ipynb`**

This notebook visualizes the gradient flow in a simple neural network learning the XOR function:

1. **Importing Libraries and Generating Data**  
   - TensorFlow, NumPy, matplotlib, and NetworkX are imported.  
   - A synthetic XOR dataset (100 points) is generated and batched using `tf.data.Dataset`.

2. **Defining the Model**  
   - A small feed-forward network with one hidden Dense layer (2 units, ReLU) and an output Dense layer (1 unit, sigmoid).

3. **Fixed Graph Layout**  
   - Node positions for inputs, hidden units, and output are precomputed for consistent visualization of the network structure.

4. **Animating Gradient Flow**  
   - The `animate_gradient_flow` function trains the model while recording per-epoch gradient norms for both hidden and output weights.  
   - A NetworkX-directed graph animates edge colors based on gradient magnitudes alongside a log-scale plot of gradient norms over epochs.

5. **Saving the Animation**  
   - The animation can be saved as an MP4 (via FFmpeg) or a GIF (via Pillow), with configurable frame rate and resolution.

---

### **Report**

* **`ADM___Backpropagation_Project.pdf`**
  The full lab report explaining the theoretical background, methodology, implementation, and results of the project work.

---

> **Note:** It is recommended to run **`gradient_flow.ipynb`** in **Google Colab**, as it requires external software installation that is easier to manage in that environment. Additionally, you may need to adjust the file path where the `.mp4` animation is saved to ensure it matches the Colab directory structure.


