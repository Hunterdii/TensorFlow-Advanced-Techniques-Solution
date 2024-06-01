# Visualization and Interpretation

1. Consider the following code for Class Activation Maps. Which layer(s) of the model do we choose as outputs to draw out the class activation map ? Check all that apply.

   - The layer which feeds input to the model
   - The layer which performs concatenation in the model
   - **_The layer which holds the extracted features in the model_(Answer)**
   - **_The layer which performs classification on the model_(Answer)**

2. To compute the Class Activation Map you \***\*\_\_\_\_\*\***.

   - Take the dot product of the features and the output of the classification vector.
   - **_Take the dot product of the features associated with the prediction on the image, with the weights that come from the last global average pooling layer._(Answer)**
   - Take the dot product of the weights associated with the prediction and the output of the classification vector.

3. In a Salience map you get to see parts of the image the model was paying attention to when deciding what class to assign to the image.

   - True
   - **_False_(Answer)**

4. In Saliency Maps, the pixels that most impact the final classification are found by looking at the gradients of the final layers to see which ones had the steepest curve, and figure out their location and plot them on the original image.

   - False
   - **_True_(Answer)**

5. Which of the following statements are not true about GradCAM? Check all that apply.
   - The gradients of the loss are computed with respect to the selected layer’s output and averaged out across all feature maps.
   - You stack the filter outputs on the final layer into a heatmap by calculating the mean of those values.
   - **_The model built to perform the task uses the last two layers of the original model as the outputs._(Answer)**
   - **_The negative values in the heatmapof the gradCAM are kept as they enhance the performance and accuracy of the gradCAM._(Answer)**
