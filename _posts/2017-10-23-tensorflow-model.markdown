---
layout: post
title:  "Tensorflow MNIST"
date:   2017-10-23 17:24:08 -0400
categories: study
---


Learnning ml with tensorflow [GitHub](https://github.com/DavidTai1/TF) 

# **Updates:** 
[trained model](https://github.com/DavidTai1/tensorflow/tree/master/model)

**Second approach 4 layers**

	AdagradOptimizer rate:0.2
	#: 0 accuracy: 0.9463
	#: 1 accuracy: 0.9607
	#: 2 accuracy: 0.9659
	#: 3 accuracy: 0.9702
	...
	#: 17 accuracy: 0.9778
	#: 18 accuracy: 0.9776

	#---------------------

	GradientDescentOptimizer rate:0.2
	#: 0 accuracy: 0.9496
	#: 1 accuracy: 0.9589
	#: 2 accuracy: 0.9626
	#: 3 accuracy: 0.9672
	...
	#: 6 accuracy: 0.9701
	#: 7 accuracy: 0.9697
	#: 8 accuracy: 0.9706
	#: 9 accuracy: 0.9713
	#: 10 accuracy: 0.9707
	#: 11 accuracy: 0.9714
	#: 12 accuracy: 0.971
	#: 13 accuracy: 0.9717

**First approach 1 layer inout**

	AdagradOptimizer rate:0.2

	#: 0 accuracy: 0.9156
	...
	#: 20 accuracy: 0.9304

	#---------------------

	GradientDescentOptimizer rate:0.2

	#: 0 accuracy: 0.9037
	...
	#: 20 accuracy: 0.9289

	#---------------------

References:

[Install Tensorflow](https://www.tensorflow.org/install/install_mac)

[Install Tensorboard](https://github.com/dmlc/tensorboard/blob/master/docs/tutorial/understanding-vanish-gradient.ipynb)

Youtube:
[ML1](https://www.youtube.com/watch?v=lAaCeiqE6CE&list=PLXO45tsB95cKI5AIlf5TxxFPzb-0zeVZ8)
[ML2](https://www.youtube.com/watch?v=yZAmA00mF7s)
[RL](https://www.youtube.com/watch?v=vCNkQREqd2k&list=PLjSwXXbVlK6K2enbNmPGjnmB8QBRgCv5s)







