# GANs

1. In GANs, the network learns to improve on creating data by the way of knowledge flowing back from the discriminator to the generator.

   - **_True(Answer)_**
   - False

2. In the process of training a GAN, the generator is trained by getting it to produce a batch of fake images, and also labelling them as real images despite them being fake. While this happens the evaluation performed by the discriminator helps in updating the parameters for the discriminator.

   - **_False(Answer)_**
   - True

3. Consider the following piece of code for a generator, what is the purpose of using the selu activation function instead of ReLU?

   - **_ReLU removes the noise within your data, but your intention is to keep it which is why selu is used.(Answer)_**
   - You want to remove the negative values which cancel out the positive values.

4. Consider the following code for training the generator and check all that are true.

   - You set the trainable parameters of the discriminator to false because updating the discriminator weights after every epoch is costly in the phase 2 of the training.
   - **_You set all of the generator_labels=1 and pass in only the fake images in phase 2 of the training.(Answer)_**
   - **_You set the trainable parameters of the discriminator to false because updating the discriminator weights will corrupt the training process.(Answer)_**
   - You set all of the generator_labels=1 and pass in only the real images in phase 2 of the training.

5. With regards to GANs, what does the term mode collapse mean?

   - When the discriminator is no longer able to distinguish between real and fake data.
   - When the generator is no longer able to fool the discriminator with the generated data.
   - When the quality of the generated data stops to improve as the number of epochs increase.
   - **_When the model starts to generate more and more of the same data with which it was able to fool the discriminator.(Answer)_**

6. Which of the following are some of the best practices when building GANs (DCGans) which help us avoid the problem of mode collapse ? Check all that apply.

   - In the generator’s architecture you should use pooling layers or Conv2D instead of Conv2DTranspose layers.
   - **_Avoid the use of Dense layer in both the discriminator and the generator.(Answer)_**
   - **_Batch normalization should be used in the generator except in the output layer.(Answer)_**
   - All activation layers in the generator’s architecture should be selu and in the discriminator’s all activation layers should be ReLU.

7. You can apply a 3x3 stride filter of 1 on a 3x3 image using Conv2DTranspose (Process of deconvolution).

   - False
   - **_True(Answer)_**

8. Following is the code of a discriminator. According to best practices, which activation function should be used ?
   - **_LeakyReLU(Answer)_**
   - selu
   - tanh
   - ReLU
