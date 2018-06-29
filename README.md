# tensorflow

* 一个变量 name shape dtype initializer trainable
	
```python
tf.strided_slice
t = tf.constant([[[1, 1, 1], [2, 2, 2]],
                 [[3, 3, 3], [4, 4, 4]],
                 [[5, 5, 5], [6, 6, 6]]])
tf.strided_slice(t, [1, 0, 0], [2, 1, 3], [1, 1, 1])  # [[[3, 3, 3]]]
tf.strided_slice(t, [1, 0, 0], [2, 2, 3], [1, 1, 1])  # [[[3, 3, 3],
                                                      #   [4, 4, 4]]]
                                                      # [2, 1, 3] - [1, 0, 0] = [1, 1, 3]
                                                      # [2, 2, 3] - [1, 0, 0] = [1, 2, 3]
```
