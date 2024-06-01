# Image Segmentation

1. At the heart of image segmentation with neural networks is an encoder/decoder architecture. What functionalities do they perform ?

   - The encoder extracts features from an image and the decoder takes those extracted features, and assigns class label to the entire image.
   - **_The encoder extracts features from an image and the decoder takes those extracted features, and assigns class labels to each pixel of the image._(Answer)**
   - The decoder extracts features from an image and the encoder takes those extracted features, and assigns class labels to each pixel of the image.
   - The decoder extracts features from an image and the encoder takes those extracted features, and assigns class label to the entire image.

2. Is the following statement true regarding SegNet, UNet and Fully Convolutional Neural Networks (FCNNs):
   Unlike the similarity between the architecture design of SegNet & UNet, FCNNs do not have a symmetric architecture design.

   - False
   - **_True_(Answer)**

3. What architectural difference does the numberrepresent in the names of FCN-32, FCN-16, FCN-8 ?

   - The number represents the total number of filters used in the final pooling layer in the architecture to make predictions.

   - **_The number represents the factor by which the final pooling layer in the architecture up-samples the image to make predictions._**
   - The number represents the total number of convolutional layers used in the final pooling layer in the architecture to make predictions.
   - The number represents the total number of pooling layers used in the architecture to help make predictions.

4. Take a look at the following code and select the type of scaling that will be performed

   - **_The upsampling of the image will be done by means of linear interpolation from the closest pixel values_(Answer)**
   - The upsampling of the image will be done by copying the value from the closest pixels.

5. What does the following code do?

   - **_It takes the pixel values and filters and tries to reverse the convolution process to return back a 3x3 array which could have been the original array of the image._(Answer)**
   - It takes pixel values in the image, in a 3x3 array, and using the specified filters, creates a transpose of that array.

6. The following is the code for the last layer of a FCN-8 decoder. What key change is required if we want this to be the last layer of a FCN-16 decoder ?

   - **_kernel_size=(16, 16)_(Answer)**
   - n_classes=16
   - strides=(16, 16)
   - Using sigmoid instead of softmax.

7. Which of the following is true about Intersection Over Union (IoU) and Dice Score, when it comes to evaluating image segmentation? (Choose all that apply.)

   - **_For IoU the numerator is the area of overlap for both the labels, predicted and ground truth, whereas for Dice Score the numerator is 2 times that._(Answer)**
   - For both, IoU & Dice Score the denominator is the total area of both the labels, predicted and ground truth
   - **_Both have a range between 0 and 1_(Answer)**
   - Unlike IoU, for Dice Score the closer the value is to 0 the closer the prediction is to the ground truth.

8. Consider the following code for building the encoder blocks for a U-Net. What should this function return?

   - after_dropout, after_pooling (you need to return after_pooling to be used in skip connections)
   - blocks
   - after_dropout
   - **_blocks, after_dropout_(Answer)**

9. For U-Net, on the decoder side you combine skip connections which come from the corresponding level of the encoder. Consider the following code and provide the missing line required to account for those skip connections with the upsampling.

(Important Notes: Use TensorFlow as tf, Keras as keras. And be mindful of python spacing convention, i.e (x, y) not (x,y) )

- **_tf.keras.layers.Concatenate()([upsampling_layer, conv_output])_**
