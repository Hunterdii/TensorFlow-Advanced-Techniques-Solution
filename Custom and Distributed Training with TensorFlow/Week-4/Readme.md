# Distributed Strategy

1. Which of the following is true about training your model using data parallelism technique? Check all that are true.

   - The same model architectures are used on different machines, and each machine processes the entire data set.
   - **_Weights from different machines are aggregated and updated into a single model.(Answer)_**
   - All of the data is on 1 master machine, and copies of the data are then distributed to machines having different model architectures based on their capacity of processing the data.
   - **_The full data set is split up and subsets of the data are stored across multiple machines(Answer)_**

2. In TensorFlow version 2, tf.distribute.Strategy class supports **\_\_\_**. Check all that apply.
   - **_Eager Mode(Answer)_**
   - **_Graph Mode(Answer)_**
3. Which of the following are true of both MirroredStrategy and TPU Strategy? Check all that are true.
   - Uses multiple machines
   - **_The same model is replicated on each core.(Answer)_**
   - **_Uses a single machine(Answer)_**
   - **_Variables are synchronized (mirrored) across each replica of the model(Answer)_**
   - Uses multiple machines
4. To modify training code to work with Mirrored Strategy, which of the following should we do? Choose all that apply.

   - Put the code that creates, compiles and fits the model inside the scope of “with strategy.scope()”.
   - **_Adjust the batch size to equal the batch size per replica times the number of replicas(Answer)_**
   - Increase the batch size as long as the number is 2^n (e.g. 64, 128, 256 etc).
   - **_Put code that creates the model object inside the scope of “with strategy.scope()”.(Answer)_**

5. To modify training code to work with distributed data, which of the following should we do? Choose all that apply.
   - **_Use strategy.experimental_distribute_dataset to convert training and test sets into distributed datasets.(Answer)_**
   - **_Use strategy.run to run the code that updates the model weights (calculating loss, calculating the gradients, and applying the gradients).(Answer)_**
   - Replace the code that updates the model weights (calculating loss, calculating gradients, and applying the gradients) so that each training step handles all replicas at once.
   - **_Use strategy.reduce to aggregate the losses across the replicas.(Answer)_**
6. To use the TPU strategy, there are some steps that you’ll take before running the training code. Please think about which line of code implements each step and choose the set of code that performs these steps in this order.

   1. Get the TPU address
   2. Find the TPU cluster
   3. Connect to the TPU cluster
   4. Initialize the TPU cluster
   5. Create your TPU strategy

   ```python
   tpu_address = 'grpc://' + os.environ['COLAB_TPU_ADDR']
   tf.distribute.cluster_resolver.TPUClusterResolver(tpu_address)
   tf.config.experimental_connect_to_cluster(tpu)
   tf.tpu.experimental.initialize_tpu_system(tpu)
   strategy = tf.distribute.experimental.TPUStrategy(tpu)
   ```
