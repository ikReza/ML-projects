# Image classification using cifar10 data from keras API. Using functional API

1. Load the cifar10 data from keras API

```
tf.keras.datasets.cifar10
```

2. normalizing the X_values(train & test) by 255.0 and flatten the y_values(target) since the API expects 1D target value.

3. keras functional API
	- 1 Input layer(expects 3D input)
	- 3 Conv2D layer
	- 1 Flatten
	- 1 Dropout, 1 Dense, 1 Dropout, 1 Dense
	- model = Model(i, x)

4. model compile & fit
	- optimizer: adam
	- loss: sparse-cross-entropy
	- metrics: accuracy