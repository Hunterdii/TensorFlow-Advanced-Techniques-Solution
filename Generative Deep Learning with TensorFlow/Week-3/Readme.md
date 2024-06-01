# Variational AutoEncoders

1. For Variational AutoEncoders, which of the following are the correct operations performed in the latent space?

   - encoder mean + encoder STDev + gaussian distribution
   - **_encoder mean + encoder STDev \* gaussian distribution(Answer)_**
   - encoder mean _ encoder STDev _ gaussian distribution
   - encoder mean \* encoder STDev + gaussian distribution

2. Consider the following code, which is used in Variational AutoEncoder to represent the latent space. Fill in the missing piece of code.
   (Note:Use shape as shape=(batch, dim) )

   ```python
   tf.keras.backend.random_normal(shape=(batch, dim))
   ```

3. When building the architecture for the decoder for a convolutional Variational AutoEncoder, what type of layers will you use ? Below is a screenshot of the code with # layer name # written in place of the actual layer that you would use. What goes in place of # layer name #?

   - Global AveragePooling2D
   - Conv2D
   - MaxPooling2D.
   - **_Conv2DTranspose(Answer)_**

4. Fill in the missing code for Kullback-Leibler cost function.
   - mu - tf.square(sigma) - tf.math.exp(mu)
   - kl_loss = 1 + mu - tf.square(sigma) - tf.math.exp(mu)
   - **_kl_loss = 1 + sigma - tf.square(mu) - tf.math.exp(sigma)(Answer)_**
   - kl_loss = sigma - tf.square(mu) - tf.math.exp(sigma)
