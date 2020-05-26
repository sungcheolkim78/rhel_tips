# magma

For pytorch, this package should be installed first. To compile magma,
CUDA toolkit is installed and openblas or MKL is necessary.

Using cmake, I could not success to install. So I tried to use make.inc
file and Makefile. But for that case, it will be better to modify cuda
file to set sm50 architecture only. And check gcc to be ccache cc.

```
export CUDADIR=/usr/local/cuda
source /opt/intel/bin/compilervars.sh intel64
export OPENBLASDIR=/projects/SharedFolder/Software/install/openblas
```
copy make.inc and compile. It worked. (2019/10/17)

[link](https://icl.cs.utk.edu/projectsfiles/magma/doxygen/installing.html)

for MKL, MKLROOT variable should be set. MKL make errors now.

```
export CUDADIR=/usr/local/cuda
source /opt/intel/bin/compilervars.sh intel64
./run_tests.py --lu --precision s --small > lu.txt
./run_tests.py --lu --precision s --small --interactive
```

check ccmake and confirm cuda-10.0 directory path, especially libcuda.so

This will set environmental variables for MKL

