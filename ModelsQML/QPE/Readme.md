Data Loading and Preprocessing: We loaded seismic data from a CSV file, cropped the data to a specified time range, and normalized the seismic trace and impedance data.

Data Preparation for PyTorch: We converted the normalized data into PyTorch tensors and created a DataLoader for batching.

Quantum Phase Estimation (QPE): We defined and implemented a Quantum Phase Estimation circuit using PennyLane. This included applying Hadamard gates, phase shift gates, and a manual Quantum Fourier Transform.

Optimization: We optimized the QPE angles to minimize the cost function using the Adagrad optimizer and printed the progress at regular intervals.

Mapping QPE to Seismic Values: We mapped the QPE probabilities to seismic trace values using interpolation, ensuring the sizes of the QPE and original seismic data matched.

Visualization: We plotted the original seismic trace alongside the seismic values obtained from the QPE to compare their performance.

![QPEEEEE](https://github.com/user-attachments/assets/1b1adcd5-76de-41fa-90ee-65befeadfad8)
![QEPPPPPPEPPE](https://github.com/user-attachments/assets/fcc1e96d-db4e-483f-95fd-4f23015dd8ca)
![QEPPPSPPPPS](https://github.com/user-attachments/assets/90a120e6-25a0-43c9-bcb9-b92bc53368c2)

