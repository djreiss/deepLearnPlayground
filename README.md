# My playground for dinking around with deep learning.

* Notes:
1. Keras documentation: http://keras.io/layers/core

### To set up running using CPUs in parallel using intel re-compiled libs:

1. install [miniconda](https://conda.io/miniconda.html)
2. setenv CONDA_ENVS_PATH $MINICONDA/envs
3. conda config --add channels intel
4. conda create -n intelpython3 intelpython3_full python=3
5. source activate intelpython3
6. conda install keras tensorflow mkl-service

### Or to use GPU, replace 2-6 above with:

1. conda install matplotlib scikit-learn
2. conda install -c anaconda tensorflow-gpu=1.1.0
3. conda install -c anaconda keras-gpu=2.0.2


### Run times for notebook #1 on GPU vs. multi-CPU:

* GPU:
```
real	2m41.669s
user	2m54.096s
sys	0m12.324s
```

* CPU (16 cores):
```
real	11m14.149s
user	149m24.364s
sys	5m40.696s
```
