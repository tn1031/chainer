Standard Function implementations
=================================

.. module:: chainer.functions

Chainer provides basic :class:`~chainer.Function` implementations in
:mod:`chainer.functions` package.

Non-parameterized functions are provided as plain Python functions. These can be
directly used in forward computation without explicit handling of
:class:`~chainer.Function` objects. On the other hand, parameterized functions
should be used with explicit handling of :class:`~chainer.Function` objects.

Parameterized function classes
------------------------------
.. autoclass:: BatchNormalization
   :members: __call__

.. autoclass:: Convolution2D
.. autoclass:: EmbedID
.. autoclass:: Linear
.. autoclass:: Parameter
.. autoclass:: PReLU

Array manipulation functions
----------------------------
.. autofunction:: concat
.. autofunction:: copy
.. autofunction:: dropout
.. autofunction:: identity

Activation functions
--------------------
.. autofunction:: exp
.. autofunction:: leaky_relu
.. autofunction:: log
.. autofunction:: lstm
.. autofunction:: relu
.. autofunction:: sigmoid
.. autofunction:: softmax
.. autofunction:: tanh

Pooling functions
-----------------
.. autofunction:: average_pooling_2d
.. autofunction:: max_pooling_2d

Loss, evaluation and aggregation
--------------------------------
.. autofunction:: accuracy
.. autofunction:: mean_squared_error
.. autofunction:: softmax_cross_entropy
.. autofunction:: sum