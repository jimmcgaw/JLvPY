# Julia vs Python

I'm exploring the possibility of using Julia for machine learning, namely doing deep learing for computer vision. I'm interested in it as an option since the contenders are:

* Python
* Java
* C++
* MATLAB / Octave
* Julia

Python is the most widely used (arguably), but it is "slow" compared to the others. I'd rather not go down the rabbit hole of learning C++, I don't want to start messing with the JVM, and to hell with the paid commerical option of MATLAB. (I might look at the open source alternative to the latter, ie Octave, in near future.)

So, I'm doing some very unscientific benchmarking between Python and Julia. The first task will be to create two idential convolutional neural networks with Tensorflow in Python and Flux.jl in Julia, and see how each of them perform when training on the classic MNIST digits dataset, as well as how fast they each perform at inference.

This is structured as a Julia project, with some Python scripts and a venv tossed into the mix.

## Set Up

Create a Python virtualenv. (I'm using Python 3.11.9)

```
python -m venv env
```

```
source env/bin/activate
```

```
pip install -r requirements.txt
```

## Starting

```
jupyter notebook
```