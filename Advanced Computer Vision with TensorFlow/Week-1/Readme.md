# Introduction and Concepts of Computer Vision

1. In a Multi-Class classification scenario, your model can identify all the different items and people that are present in a given input image.

   - **_False(Answer)_**
   - True

2. Which of the following statements correctly describes the difference between object detection and object localization?
   - **_Object localization is where you get a bounding box around the main subject of the image, while in object detection you get a bounding box around all of the objects  
     within an image.(Answer)_**
   - Object detectionis where you get a bounding box around the main subject of the image, while in object localization you get a bounding box around all of the objects within an image.
   - They both are the same.
   - Object detection refers to detecting the object within an image, while object localization gives us the bounding box around that object.
3. What is the method that locates an object(s) by labelling the pixels, where each similar object(s) is assigned to the same class? Type your response here
   (two words, all lower case).
   - **\_**semantic segmentation**(Answer)\_**
4. In the context of Transfer Learning, the initial training task where the model learns reusable patterns is called a downstream task.

   - True
   - **_False(Answer)_**

5. Check all the scenarios in which Transfer Learning could be beneficial.
   - To ensure better performance
   - **_To reduce computation and processing cost(Answer)_**
   - **_When the task you want to perform is a sub-task of an already trained, larger, model.(Answer)_**
   - **_When you don’t have enough data for the task you want to perform, which resembles another same or similar, already trained task.(Answer)_**
6. What is the name of the built-in TensorFlow layer-type which you can use to increase the dimensions of a 2D image ?

   - **_UpSampling2D(Answer)_**
   - UpSampling
   - SampleUp2D
   - SampleIncrease

7. You have an image of dimensions 48 x 48, and you want to upscale it to 240 x 240 using the built-in TensorFlow layer-type which is used to perform such a task
   (mentioned in Question 6). What will you pass in as size=\_\_\_\_? \* **_(5,5)(Answer)_**
8. Consider the following code:

   ```python
   mylayer = tf.keras.applications.resnet.ResNet50(include_top=False , input_shape=(224,224,3) , weights="imagenet")(inputs)
   ```

   - **_It discards the top most layers of ResNet50 when initializing my_layer using ResNet50.(Answer)_**
   - It discards the first layer of ResNet50 when initializing my_layer using it.
   - It sets the top most layers as untrainable of ResNet50 when initializing my_layer using it.
   - It randomly sets up the weights, instead of using that of ImageNet, for the top most dense layers of ResNet50 when initializing my_layer using it.

9. What is the name of the technique used in the output dense layer that is used to predict Bounding Boxes ? (Hint: It is a one word answer)
   - **_regression(Answer)_**
10. Check all the statements that are true regarding Intersection Over Union (IoU), with regards to Bounding Boxes.
    - The values of IoU range from 0 to all possible positive values.
    - **_IoU is the area of intersection of the two boxes (true and predicted) divided by the total union area of the two boxes.(Answer)_**
    - The closer the value of IoU is to 0 the better is the prediction of the bounding box.
    - **_The closer the value of IoU is to 0 the poorer is the prediction of the bounding box.(Answer)_**
