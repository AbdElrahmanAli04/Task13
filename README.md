# Task 13 - NN Magic

## **About**

Neural Networks, inspired by the structure and functioning of the human brain, are powerful machine learning algorithms capable of handling complex data and learning from experience. They are widely used in areas like image recognition, speech processing, and autonomous systems. This task will explore the fundamentals of neural networks by constructing one from scratch and applying it to classify handwritten digits from the MNIST dataset.

## **Neural Networks: Chapter and Video Summary**

Based on:
- Michael Nielsen’s book *Neural Networks and Deep Learning* (Chapter 1)
- The YouTube video *But What is a Neural Network? | Chapter 1, Deep Learning* by 3Blue1Brown

### 1. What Are Neurons?

- Neurons, akin to the brain's neural system, act as points in a network with specific connections to other neurons.

### 2. How Do Neurons Work?

- Each neuron functions like a node, generating an output value between `[0.0, 1.0]` based on its input and connections.

### 3. How Does the Function Work?

- Neurons operate using a set of functions distributed across an array. Each neuron processes the data, applies a predefined method, and then passes the result to the next layer.

### 4. What Happens After Calculation?

- After processing, the neuron outputs are weighted and passed through a sigmoid function. This function adjusts the output to fit within the `[0.0, 1.0]` range before sending it to the next layer. This process continues until the final output is produced.

## **Comparison: Manual Implementation vs. PyTorch**

### 1. Ease of Use and Flexibility

- **From Scratch**: Building a neural network manually provides detailed control over every aspect, including parameter definitions and propagation methods. While this approach is highly flexible, it is more error-prone and requires careful handling of each component.

- **PyTorch**: Using PyTorch simplifies implementation significantly by automating forward and backward propagation, gradient computations, and weight updates. This framework makes integration and experimentation easier while reducing the potential for errors.

### 2. Performance

- **From Scratch**: A manually implemented neural network using NumPy runs on the CPU and lacks optimizations for large-scale operations. This can lead to slower performance, particularly with extensive datasets or complex networks, hence when the hidden layers were 40 and the epochs were the same the model manged to make a test with accuracy of : 9557 / 10000 (95.57%)



- **PyTorch**: PyTorch leverages GPU acceleration, resulting in substantial performance improvements, especially for large datasets like MNIST or more intricate models ,  and the efficiency for the same number of hidden layers and epochs was 85.02% , which indicates that the Scratch model provide more accurate results for this small model !
