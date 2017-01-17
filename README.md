# Better reservoir sampling, using random Fourier features!

This code implements the online algorithm for selecting a representative subset from streaming data,
as described in [this paper](http://auai.org/uai2016/proceedings/papers/293.pdf):

Paige, B., Sejdinovic, D., & Wood, F. (2016). Super-sampling with a Reservoir.
In *Proceedings of the 32nd Annual Conference on Uncertainty in Artificial Intelligence*, UAI 32: 567–576.

For usage, see the example notebooks:

* [MNIST Summarization](notebooks/MNIST-Summarization.ipynb)
* [Weighted Data](notebooks/Weighted-Data.ipynb)
* [Gaussian Mixtures](notebooks/Gaussian-Mixture-Example.ipynb)

The code is *not* particularly optimized at this point.
In particular, overhead from explicit looping over data structures in python 
means the online algorithm can be slower than a batch algorithm for moderately-sized data.
