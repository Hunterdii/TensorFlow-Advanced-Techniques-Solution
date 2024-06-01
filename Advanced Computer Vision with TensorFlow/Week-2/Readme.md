# Object Detection

1. Check all the techniques that can be used to improve the accuracy of detecting objects and encapsulating them entirely within a single bounding box.
   - **_Increase the size of the bounding box until the object fits entirely in it.(Answer)_**
   - Scale down the image and then detect the object within it using the bounding box
   - **_Use Selective Search technique(Answer)_**
2. Check all that are true for Selective Search.
   - **_It tries to identify larger objects by grouping together initially identified smaller objects(Answer)_**
   - The biggest bounding box detected of the smaller objects in the end becomes the final bounding box around the identified object.
   - **_Image segmentation is used in this technique(Answer)_**
3. The technique of selecting the best bounding box based on the highest intersection over union (IOU) between the true label and several predicted bounding boxes is called non-maximum ****\_\_\_\_**** (NMS).
   (Hint: it is a one word answer) \* **_suppression(Answer)_**
4. Consider the following image, according to the NMS technique which coloured bounding box will be eventually selected as the best bounding box around the football?
   - **_Purple (# 4)(Answer)_**
   - Green (# 1)
   - Yellow (# 2)
   - Red (# 3)
5. One of the differences between R-CNN and Fast R-CNN is that, Fast R-CNN proposes regions of interest to the input image (generates), whereas in R-CNN regions of interest are expected to be an input
   (as opposed to generating them) to the model. \* **_False(Answer)_** \* True
6. Consider the following code and check all that are true.
   - Setting use_normalized_coordinates=True indicates that your bounding box coordinates are not normalized, so you want them to be normalized.
   - **_label_id_offsetis an adjustment in case the ‘detection classes’ starting index and actual starting index have an offset between them.(Answer)_**
   - image_np_with_detections[0] is a numpy array containing the image, and 0 index shows there are multiple input images being passed to this function.
   - **_min_score_threshis used to leave out object labels and their bounding boxes if their score falls below the set threshold.(Answer)_**
7. The following code initializes a model and restores pre-trained weights, detection_model, using the .config file method
   - **_False(Answer)_**
   - True
8. Which of the following is the correct syntax to print a list of your trainable variables in a model ?
   - **_`for varName in myModel.trainable_variables:    
 print(varName.name)`(Answer)_**
   - `for varName in myModel.trainables:
 print(varName.name)`
   - `for varName in myModel.trainableVariables:
 print(varName.name)`
   - `for varName in myModel.Variables:
 print(varName.name)`
