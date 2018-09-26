### Tensorflow-GPU prebuild binaries with Dockerfile for Linux + CUDA 8.0/9.0/9.2 which is not provided by official Tensorflow pip repository.

The list of all wheel-format downloads can be found in the [download page](https://github.com/ghostplant/tensorflow-cuda-optimized/releases).

Note that CUDNN will be automatically included into binary packages, and the extra installation of CUDNN is not needed.

### Examples of Installation from online prebuilt binary:

```sh
# Install Tensorflow-GPU 1.10 on `Ubuntu 16.04` with CUDA 8.0:
pip3 install https://github.com/ghostplant/tensorflow-cuda-optimized/releases/download/tf-1.10-ubuntu/tensorflow-1.10_cuda8.0_ubu1604-cp35-cp35m-linux_x86_64.whl
```

```sh
# Install Tensorflow-GPU 1.10 on `Ubuntu 16.04` with CUDA 9.0:
pip3 install https://github.com/ghostplant/tensorflow-cuda-optimized/releases/download/tf-1.10-ubuntu/tensorflow-1.10_cuda9.0_ubu1604-cp35-cp35m-linux_x86_64.whl
```

```sh
# Install Tensorflow-GPU 1.10 on `Ubuntu 16.04` with CUDA 9.2:
pip3 install https://github.com/ghostplant/tensorflow-cuda-optimized/releases/download/tf-1.10-ubuntu/tensorflow-1.10_cuda9.2_ubu1604-cp35-cp35m-linux_x86_64.whl
```


### How to Compile Tensorflow-GPU packages on Ubuntu from Source Code:

```sh
git clone https://github.com/ghostplant/tensorflow-cuda-optimized
cd tensorflow-cuda-optimized

# For example:
CUDA_VERSION=10.0 ./make-tensorflow1.10-ubuntu.sh

# or:
CUDA_VERSION=9.2 ./make-tensorflow1.10-ubuntu.sh

# or:
CUDA_VERSION=9.0 ./make-tensorflow1.10-ubuntu.sh

# or:
CUDA_VERSION=8.0 ./make-tensorflow1.10-ubuntu.sh
```
