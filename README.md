# My playground for dinking around with deep learning.

* Notes:
1. Keras documentation: http://keras.io/layers/core

### To set up running in parallel using intel re-compiled libs:

1. install miniconda
2. setenv CONDA_ENVS_PATH $MINICONDA/envs
3. conda config --add channels intel
4. conda create -n intelpython3 intelpython3_full python=3
5. source activate intelpython3
6. conda install keras tensorflow mkl-service
