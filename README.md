# model-free-robotics
This section trains and evaluates various machine learning models to optimize the control of bionic tendon-driven robots, comparing their accuracy and computational efficiency.

## Performance of Robot Motions Using Orginial Transfer Function
### Deviations between desired and actual yaw angles (horizontal movements)
![image](https://github.com/poyuhs/model-free-robotics/blob/main/result/fig_yawAngByTime_n4.png)

## Training Data Collection (based on physics simulations in Grasshopper)

### Pitch and yaw angle (traing input X)
![image](https://github.com/poyuhs/model-free-robotics/blob/main/result/fig_dataCollection_pitchYaw_2D.png)
### Length variations of tendon actuators (training output Y)
![image](https://github.com/poyuhs/model-free-robotics/blob/main/result/fig_dataCollection_lengthVar_2D.png)


## Training and Evaluation of Model-Free Method Using Machine Learning Models
In this section, we utilize four types of learning models: 
ensemble learning models (Random Forest, Gradient Boosting),
regularization-based models (Ridge, Lasso Regression),
kernel-based models (Support Vector Regressor, Gaussian Process Regressor), and 
neural network models (Bayesian Neural Network, Recurrent Neural Network)

### Gradient Boosting
![image](https://github.com/poyuhs/model-free-robotics/blob/main/result/fig_Gradient_Boosting_results.png)

### Recurrent Neural Network
![image](https://github.com/poyuhs/model-free-robotics/blob/main/result/fig_Recurrent_Neural_Network_results.png)


## Non-linear Transfer Function Identification
We use polynomial regression to identify optimized tranfer functions for bionic robot control.
Let's visualize in 3D and compare it with the original ones.

### Optimized transfer functions
![image](https://github.com/poyuhs/model-free-robotics/blob/main/result/fig_Polynomial_Transfer_Functions_3D.png)
### Original transfer functions
![image](https://github.com/poyuhs/model-free-robotics/blob/main/result/fig_Original_Transfer_Functions_3D.png)
