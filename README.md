# tensorflow-from-source

A small image that downloads and builds TensorFlow. Since TensorFlow 1.6.0, the official binary is compiled with AVX instructions. These cannot be executed on older Intel processors. This image downloads TensorFlow from git repository, downloads other build dependencies, and compiles TF from source for your CPU.

It is based on Ubuntu Bionic and updates the APT source.list to download and install Bazel (required for building TF). Once the script is started on the command-line the rest of the process is automated.

First time startup (docker run):

$ docker run --name tf_build -it jdonato1/tensorflow-from-source

