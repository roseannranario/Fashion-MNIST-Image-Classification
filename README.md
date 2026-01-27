# Fashion-MNIST-Image-Classification
Fashion-MNIST-Image-Classification


Fashion-MNIST-Image-Classification

GOOGLE COLAB LINK :

QUESTIONS ***********

1. What is the Fashion MNIST dataset?
Answer : The Fashion MNIST dataset is a collection of 70,000 grayscale images of clothing items across 10 distinct categories, such as shirts, dresses, and sneakers. It was designed by Zalando Research as a more challenging drop-in replacement for the original MNIST digit dataset. Each image is $28 \times 28$ pixels, making it an ideal benchmark for testing basic computer vision and machine learning models.

2. Why do we normalize image pixel values before training?
Answer : Normalization scales the pixel values from their original range of 0–255 down to a range of 0–1. This process ensures that the input data has a consistent scale, which helps the gradient descent algorithm converge much faster during training. Without it, the model might struggle with numerical instability or take significantly longer to find the optimal weights for the neural network.

3. List the layers used in the neural network and their functions.
Answer: The model uses a Flatten layer to convert the 2D $28 \times 28$ image grid into a 1D array of 784 pixels. This is followed by a Dense (Hidden) layer with 128 neurons and a ReLU activation function, which learns complex patterns and non-linear relationships within the data. Finally, a Dense (Output) layer with 10 neurons provides the raw scores (logits) for each of the 10 possible clothing classes.

4. What does an epoch mean in model training?
Answer : An epoch represents one complete pass of the entire training dataset through the neural network. During a single epoch, the model looks at every training image once, calculates the error (loss), and updates its internal weights to improve its performance. Multiple epochs are usually required because the model needs several iterations to gradually minimize the loss and "learn" the distinguishing features of the images.

5. Compare the predicted label and actual label for the first test image.
Answer : In Step 2.6 of the lab, the predicted label for the first test image is typically 9, which corresponds to an "Ankle boot." When compared to the test_labels[0] value, we find that the actual label is also 9, indicating a successful classification. This high confidence match (often over 95%) demonstrates that the model has effectively learned to recognize the specific features that define an ankle boot.

6. What could be done to improve the model’s accuracy?
Answer : To improve accuracy, you could increase the number of epochs to give the model more time to learn, or add more neurons and hidden layers to increase the model's capacity. Implementing Convolutional Neural Networks (CNNs) instead of simple Dense layers would also significantly boost performance by better capturing spatial hierarchies in the images. Additionally, using techniques like Dropout or Data Augmentation could help the model generalize better to unseen data and reduce overfitting.

