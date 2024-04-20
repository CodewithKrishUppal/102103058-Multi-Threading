# 102103058-Multi-Threading
Methodology :
Matrix Size: Matrices of size NxN are used, where N is chosen to be sufficiently large to ensure a significant computation workload. Constant Matrix: A constant matrix of the same size as the input matrices is generated for multiplication. Thread Configuration: Matrix multiplication is performed using varying numbers of threads, ranging from 1 to 8. Performance Metrics: The time taken to perform matrix multiplication with each thread configuration is measured.

Implementation :
Matrix Generation: Random matrices of the specified size are generated using NumPy. Matrix Multiplication: The matrix multiplication operation is parallelized using Python's threading module. Each thread is responsible for computing a portion of the resulting matrix. Thread Management: Workload is divided among threads to ensure balanced computation. Performance Measurement: The time taken for matrix multiplication with each thread configuration is recorded. Visualization: The results are visualized using matplotlib to show the relationship between the number of threads and the time taken for matrix multiplication.

Results :
![image](https://github.com/Codelord2003/102103058-Multi-Threading/assets/95679005/b2e82bfb-16d1-4560-9961-0988fb8cad6c)

Analysis :

Performance Plateau and Overhead: From  processes 1 onwards, the time taken generally increases with each additional process. This indicates that the overhead of process management, context switching, and communication between processes becomes more significant as the number of processes increases. 

Diminishing Returns: Beyond a certain point  the performance improvement diminishes. In fact, the time taken starts to increase as the number of processes continues to increase. 

System Resource Limitations: The observed behavior could also be influenced by system resource limitations. As the number of processes increases, the system's CPU cores, memory bandwidth, and other resources may become saturated, leading to reduced efficiency and performance.

Graph :
<img width="565" alt="image" src="https://github.com/Codelord2003/102103058-Multi-Threading/assets/95679005/e5b0a6cd-c39b-4499-bb5e-19d4cd8c737c">

CPU USAGE :

