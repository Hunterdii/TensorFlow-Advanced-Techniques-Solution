# AutoGraph

1. Which of the following statements is false about Graph approach?
   - Faster compilation
   - Parallelism
   - **_Easier debugging(Answer)_**
   - Portability
2. Which of the following statements is true for tf.cond ?

   - tf.cond is an alternative to using if/else statements in Graphs, as its execution is much faster than if/else statements.
   - **_Graph execution does not support if/else statements. To replicate that effect you use tf.cond(Answer)_**

3. Consider the following code:

   - By adding the decorator, @tf.function, only above the function definition of increment_by_two
   - **_By adding the decorator, @tf.function, above the definitions of both of the functions.(Answer)_**
   - By adding the decorator, @tf.autograph, above the definitions of both of the functions.
   - **_By adding the decorator, @tf.function, only above the function definition of multiple_increment(Answer)_**

4. Function written in Eager mode when converted to Graph accommodates different data types all in one, so you don’t have to define similar functions for different data types.

   - **_True(Answer)_**
   - False

5. Which of the following is the correct syntax to display the auto-generated AutoGraph code if your function name is my_function?
   - tf.autograph.code(my_function)
   - tf.autograph.to_code(my_function)
   - **_tf.autograph.to_code(my_function.python_function)(Answer)_**
   - tf.autograph.code(my_function.python_function)
6. Consider the following code, what will be the output?
   - **_6times Hello World(Answer)_**
