## Quantum Enhanced Seismic Data Analysis
This model involves data preprocessing, quantum circuit design, and clustering using Kernel Principal Component Analysis (KPCA). The steps are outlined below:

Data Preparation
Data Cropping: Selecting a specific time range for analysis.

Normalization: Scaling seismic and impedance traces between 0 and 1.


Quantum Circuit Design
A quantum circuit is designed using PennyLane for processing the seismic data. The quantum circuit involves a series of rotation gates and CNOT gates.


Quantum Circuit Processing
The processed data through the quantum circuit generates outputs for further analysis. An enhanced quantum circuit with noise layers is also introduced:

Clustering and Visualization
After processing, the data undergoes Kernel PCA for dimensionality reduction and clustering.


Pairwise Distance Matrix: To visualize the distances between data points.

Clustering Metrics:

Silhouette Score:
Silhouette Score= 
max(a,b)
b−a
​
 

where $a$ is the mean distance to the nearest cluster, and $b$ is the mean distance to the farthest cluster.
![kernelPCA](https://github.com/user-attachments/assets/8b2c1860-38c5-4f0d-801e-9b2d8a072521)

## Quantum Autoencoder (QAE) for Seismic Impedance Inversion
Data Preparation:

Loading Data: Seismic and impedance trace data are loaded from CSV and text files.
Cropping Data: The seismic data is cropped to a specific time range for focused analysis.
Normalization: The seismic and impedance traces are scaled between 0 and 1.
Data Segmentation:

The normalized data is segmented into smaller chunks to match the number of qubits used in the quantum model.
Quantum Circuit Design:

Quantum Autoencoder: A quantum circuit is designed using PennyLane, incorporating rotation and CNOT gates. The circuit encodes and decodes the seismic data.
Model Training:

Loss Function: A loss function is defined to measure the difference between original and reconstructed data.
Optimization: The quantum autoencoder is optimized using JAX and Optax. Training includes tracking metrics such as loss, Mean Squared Error (MSE), and Mean Absolute Error (MAE).
Visualization:

Reconstructed Data: The original and reconstructed seismic traces are plotted to visualize the model’s performance.
Impedance Trace: The normalized impedance trace is plotted.
Metrics: The training loss, MSE, and MAE histories are plotted to monitor the training process.
Model Saving and Loading:

The trained model parameters are saved to a file and can be reloaded for future use.

![autoencoder](https://github.com/user-attachments/assets/92a156dc-3b54-4939-895b-eaad8586559e)

