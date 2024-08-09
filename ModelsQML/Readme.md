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
