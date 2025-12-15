AlexNet Code Modifications Summary
. Changed Model Construction Method
Modified Code
def AlexNet(input_shape=(224, 224, 3), num_classes=1000):
    inputs = Input(shape=input_shape)

Explanation

Switched from the Sequential API to the Functional API.

The Functional API allows explicit definition of input and output tensors.

Provides greater flexibility than Sequential.

Easier to extend for advanced architectures such as:

Skip connections

Multi-input or multi-output models
