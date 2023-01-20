# Linear Regression using Neural Network

----------------------------------------------------------------

### What I learned from this project

There are three types of layer in neural network:
1. Input Layer
2. Output Layer
3. Hidden Layer

Example: If there is an 28x28 image then we would have 784 pixels. Each pixel will be fed to a single neuron in the input layer. Neurons of one layer is connected to the neuron of the next layer through **Channels** and each channel has assigned a numerical value known as the **weight** . Equation we follow :
                x1*w1 + x2*w2 = neuron of the next layer

Each of the neuron is associated with a numerical value known as the **bias** so the equation after considering the bias becomes

                (x1*w1 + x2*w2) + bias = neuron of the next layer
            
then this value is send to a threshold function known as the **activation function** , Result of the activation function tells if the neuron will be activated or not. Then activated neuron transmits the data to the next layer over the channels. This way we propogate in the network and know as **Forward propogation** . 

Neuron with the highest value in the output layer becomes the final output.

![neural network image](https://github.com/lakshikaparihar/End-to-End-ML-UseCase/blob/main/images/neural-network.png)

Then we calculate the error rate of each output neuron and this information goes backward to the first layer and this is known as the **backward propagation** . Based on  this information weights are adjusted