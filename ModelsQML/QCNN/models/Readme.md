Data Preparation: We loaded and preprocessed seismic data, including normalizing the seismic trace and impedance data. We added noise to the seismic data to simulate real-world conditions.

Data Splitting: We split the data into training, validation, and test sets, converting them into PyTorch tensors for model training.

Quantum Convolutional Layer: We defined a quantum convolutional layer using PennyLane, incorporating angle embedding and strongly entangling layers.

Model Definition: We built a Variational Quantum Classifier Neural Network (VQCNN) that combines the quantum layer with traditional neural network layers.

Training: We trained the VQCNN model using the training data, and tracked both training and validation losses.

Evaluation: We evaluated the model on a test set and visualized performance using metrics such as confusion matrix, training and validation losses, and seismic trace plots.

Visualization: We plotted the noisy and original seismic traces, as well as the normalized impedance traces, to visualize the data and model results.
