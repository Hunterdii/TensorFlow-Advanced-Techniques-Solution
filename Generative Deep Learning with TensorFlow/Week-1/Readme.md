1. In Neural Style Transfer when initializing the generated image from the content image,which of the following is true? Check all that apply.

   - Initially the style loss will be equal or close to zero because both, the content and generated, images are the same.
   - **_Initially the content loss will be equal or close to zero because both the content image and generated image are the same image.(Answer)_**
   - **_Your goal for the generated image is to increase the content loss and decrease the style loss, while keeping the overall accumulated loss low.(Answer)_**
   - Your goal for the generated image is to increase the style loss and decrease the content loss while keeping the overall accumulated loss low.

2. What does tf.keras.applications.vgg19.preprocess_input do?

   - **_The function centers the distribution of pixel values of an image around zero._(Answer)**
   - The function sets the pixel values of an image between 0 and 1.

3. From which part of a CNN architecture can you extract the “content” of an image?

   - **_From the deeper layers of the architecture.(Answer)_**
   - The initial layers of the architecture.

4. Consider the values given in the image below and calculate the content loss value.

   - **_19(Answer)_**

5. Fill in the missing code below:

   - tf.reduce_sum(tf.square(generated_image - content_image))
   - tf.reduce_sum(tf.square(content_image - generated_image))
   - **_0.5 \* tf.reduce_sum(tf.square(generated_image - content_image))(Answer)_**
   - **_0.5 \* tf.reduce_sum(tf.square(content_image - generated_image))(Answer)_**

6. Consider the following code snippet. How will you include Total Loss Variation in it? Use TensorFlow as tf.
   (Answer in the format, x + y(z), considering python’s spacing convention)
   - **_total_variation_weight \* tf.image.total_variation(image)(Answer)_**
