# Mixture Density Networks in pure keras, with explanations (Work in progress)

I have been studying Mixture Density Networks recently, based on fantastic resources from the following in-depth articles:
+ http://blog.otoro.net/2015/11/24/mixture-density-networks-with-tensorflow/
+ http://cbonnett.github.io/MDN.html
+ http://cbonnett.github.io/MDN_EDWARD_KERAS_TF.html

Given thre great work done by these authors above, we're not going into detail on MDNs here. Just to summarize, MDNs are literally mixture models expressed in neural network form. Instead of outputting point estimates for an expected outcome, MDNs output a probabilistically weighted combination of most likely probability distributions. The estimated values are then sampled from this mixture of distributions. 

MDN implementations I've seen online thus far rely on `pytorch` or `tensorflow`. I thought it would be interesting to explore implementing MDNs in pure `keras` without requiring `import tensorflow as tf` at some point. And also document my thoughts along the way.

Note: If you just want to use MDNs, https://github.com/cpmpercussion/keras-mdn-layer provides an MDN layer for `keras`.

TODO: Put in link to notebook or just tldr it