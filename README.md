# Flatfish-Benchmark 

Flatfish-Benchmark(Flatfish-BM) is a benchmark of different DRAM access patterns.

# Details
We choose five typical memory access patterns: Sequential, Random, Stride, Non-overlap Window and Overlap Window. According to the paper Exploiting memory access patterns to improve memory performance in data-parallel architectures, these memory access patterns can cover over 95\% applications. We choose one representative application for each memory access pattern, and design the following benchmarks:

We choose three typical neural network models as benchmarks. These neural network models include ResNet-34 (Convolutional Neural Network), Seq2Seq (Recurrent Neural Network) and GGS-NN (Graph Neural Network). 

### Sequential
We use small-scale matrix multiplication as the representative application for Sequential

### Random
We use Sorting algorithms on randomly generated data as the representative application for Random. 

### Stride
We choose image rotation for Stride pattern. Image rotation is a very typical and important application in image processing.

### Non-overlap Window
We use tile-based matrix multiplication as the representative application. Matrix multiplication is an important operation in massive applications, and tile-based processing is a common technique for large-scale matrix multiplication.

### Overlap Window
We use two-dimensional convolution as the representative application, which is one of the most important operations in convolutional neural networks.

### ResNet-34
ResNet is a widely used network architecture in the area of computer vision. We chose the memory access of inference for ResNet-34, which contains convolutional layers, fully-connected layers, pooling layers and so on.

### Seq2Seq
Sequence to sequence(Seq2Seq) is a widely used network architecture in the area of NLP. We chose the memory access of inference for a network containing the GRU layers, fully-connected layers and so on.

### GGS-NN
GGS-NN is a widely used graph neural network architecture for graph processing. We chose the memory access of inference for a Residual Gated Graph ConvNets.
