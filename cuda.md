# CUDA

[link](https://linuxconfig.org/how-to-install-nvidia-cuda-toolkit-on-centos-7-linux)

Most recent version of cuda is 10.1 as of 2019/05/17. But tensorflow is tuned for 10.0 version only. So install 10.0 version.

```
export CUDA_HOME=/usr/local/cuda-10.0
```

Make sure you are setting the correct CUDA_HOME so that system use the correct cuda version

In most cases, cuda toolkit is installed under `CUDA_HOME`

## remove all installed packages

```
yum list installed | grep "cuda-" | awk '{print $1}'
yum remove packages
```

## pkg-config

to compile correctly, you need to set pkgconfig

```
export PKG_CONFIG_PATH=/usr/local/lib/pkgconfig:/usr/local/cuda/pkgconfig:/usr/local/lib64/pkgconfig:/usr/share/pkgconfig:/usr/lib64/pkgconfig:/usr/lib/pkgconfig
```

## tsne-cuda

- download 2.0 version and compile. It works on cuda 10.0.
- depends on gflags, faiss, glog; use old version

## Nvidia driver

Download driver files

```
> _ sh NVIDIA-Linux-x86_64.418.74.run
> _ sh NVIDIA-Linux-x86_64.430.50.run
```

## CUDA toolkit 10.0

Save files to `/projects/SharedFolder/Software/cuda` and install using

```
> _ sh cuda_10.0.130_410.48_linux.run
> _ sh cuda_10.0.130.1_linux.run
```

## CUDA toolkit 9.0

[Download link](https://developer.nvidia.com/cuda-90-download-archive?target_os=Linux&target_arch=x86_64&target_distro=RHEL&target_version=7&target_type=runfilelocal)

Save files to `/projects/SharedFolder/Software/cuda` and install using

```
> _ sh cuda_9.0.176_384.81_linux.run
> _ sh cuda_9.0.176_1_linux.run
> _ sh cuda_9.0.176_2_linux.run
> _ sh cuda_9.0.176_3_linux.run
> _ sh cuda_9.0.176_4_linux.run
```

package will be install in `/usr/local/cuda-9.0`

## CUDA toolkit 9.2

Save files to `/projects/SharedFolder/Software/cuda` and install using

```
> _ sh cuda_9.2.148_396.37_linux.run
> _ sh cuda_9.2.148.1_linux.run
```


