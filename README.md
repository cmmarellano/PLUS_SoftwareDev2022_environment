# PLUS_SoftwareDev2022_environment
For [PLUS Software Development](https://github.com/cmmarellano/PLUS_softwaredev_2022), __A2_conda update__ <br><br>

Task: Go through the process of creating an environment from the requirements file from someone else in the course, modify the environment, and share the changes <br>

### 1. Environment.yml
----
[Py37_mldl.yml](https://github.com/cmmarellano/PLUS_SoftwareDev2022_environment/blob/main/Py37_mldl.yml)

A Python 3.7 environment fit for Machine Learning and Deep Learning practice:
- numpy
- GDAL
- Tensorflow
- sci-kit 



#### Some screenshots while making this environment

![image](https://user-images.githubusercontent.com/93019319/165269474-adf699f6-ef39-413f-9cb3-7cc46bd2d1c4.png)
![image](https://user-images.githubusercontent.com/93019319/165270053-d4cf0476-268d-416b-afe1-dcca7a595afb.png)
![image](https://user-images.githubusercontent.com/93019319/165270305-33fb4f41-83e7-4006-9424-16f5cf46c13f.png)
![image](https://user-images.githubusercontent.com/93019319/165290414-82d6ff4c-bb32-4f4b-8662-681ebf428d12.png)


Some notes
- GDAL will require a compatible Microsoft C++ Build Tools. Download from https://visualstudio.microsoft.com/downloads/
- Need to set-up ipykernel and nb_conda_kernels (I want to be able to use this new virtual env on Jupyter Notebook)



### 2. Commit on others environment.yml
------


```
(Py37_mldl_clone) C:\Users\Arellano\Documents\GitHub\PLUS_softwaredev_2022-3>conda env create -f environment.yml
Collecting package metadata (repodata.json): done
Solving environment: done

Downloading and Extracting Packages
setuptools-58.0.4    | 784 KB    | ############################################################################ | 100%
debugpy-1.5.1        | 2.6 MB    | ############################################################################ | 100%
mkl_fft-1.3.1        | 136 KB    | ############################################################################ | 100%
gdal-3.4.1           | 1.3 MB    | ############################################################################ | 100%
jedi-0.18.1          | 983 KB    | ############################################################################ | 100%
mkl_random-1.2.2     | 221 KB    | ############################################################################ | 100%
entrypoints-0.3      | 10 KB     | ############################################################################ | 100%
libcurl-7.80.0       | 295 KB    | ############################################################################ | 100%
certifi-2021.5.30    | 148 KB    | ############################################################################ | 100%
ipykernel-6.9.1      | 203 KB    | ############################################################################ | 100%
mkl-service-2.4.0    | 48 KB     | ############################################################################ | 100%
curl-7.80.0          | 137 KB    | ############################################################################ | 100%
numpy-base-1.21.5    | 4.4 MB    | ############################################################################ | 100%
tornado-6.1          | 607 KB    | ############################################################################ | 100%
zlib-1.2.11          | 114 KB    | ############################################################################ | 100%
jupyter_core-4.9.2   | 96 KB     | ############################################################################ | 100%
numpy-1.21.5         | 9 KB      | ############################################################################ | 100%
pyzmq-22.3.0         | 626 KB    | ############################################################################ | 100%
ipython-8.2.0        | 1012 KB   | ############################################################################ | 100%
pywin32-302          | 5.6 MB    | ############################################################################ | 100%
Preparing transaction: done
Verifying transaction: done
Executing transaction: done
#
# To activate this environment, use
#
#     $ conda activate geoenv
#
# To deactivate an active environment, use
#
#     $ conda deactivate


(Py37_mldl_clone) C:\Users\Arellano\Documents\GitHub\PLUS_softwaredev_2022-3>conda env list
# conda environments:
#
base                     C:\ProgramData\Miniconda3
Py37_mldl                C:\ProgramData\Miniconda3\envs\Py37_mldl
Py37_mldl_clone       *  C:\ProgramData\Miniconda3\envs\Py37_mldl_clone
Python3                  C:\Users\Arellano\.conda\envs\Python3
geoenv                   C:\Users\Arellano\.conda\envs\geoenv
                         C:\Users\Arellano\miniconda3


(Py37_mldl_clone) C:\Users\Arellano\Documents\GitHub\PLUS_softwaredev_2022-3>conda activate geoenv

(geoenv) C:\Users\Arellano\Documents\GitHub\PLUS_softwaredev_2022-3>conda list
# packages in environment at C:\Users\Arellano\.conda\envs\geoenv:
#
# Name                    Version                   Build  Channel
asttokens                 2.0.5              pyhd3eb1b0_0
aws-c-common              0.4.57               ha925a31_1
aws-c-event-stream        0.1.6                hd77b12b_5
aws-checksums             0.1.9                ha925a31_0
aws-sdk-cpp               1.8.185              hd77b12b_0
backcall                  0.2.0              pyhd3eb1b0_0
blas                      1.0                         mkl
bzip2                     1.0.8                he774522_0
ca-certificates           2022.3.29            haa95532_0
certifi                   2021.5.30       py310haa95532_0
cfitsio                   3.470                he774522_6
colorama                  0.4.4              pyhd3eb1b0_0
curl                      7.80.0               h2bbff1b_0
debugpy                   1.5.1           py310hd77b12b_0
decorator                 5.1.1              pyhd3eb1b0_0
entrypoints               0.3             py310haa95532_0
executing                 0.8.3              pyhd3eb1b0_0
expat                     2.4.4                h6c2663c_0
freexl                    1.0.6                h2bbff1b_0
gdal                      3.4.1           py310h0fae465_0
geos                      3.8.0                h33f27b4_0
geotiff                   1.7.0                h4545760_0
hdf4                      4.2.13               h712560f_2
hdf5                      1.10.6               h7ebc959_0
icc_rt                    2019.0.0             h0cc432a_1
intel-openmp              2021.4.0          haa95532_3556
ipykernel                 6.9.1           py310haa95532_0
ipython                   8.2.0           py310haa95532_0
jedi                      0.18.1          py310haa95532_1
jpeg                      9d                   h2bbff1b_0
jupyter_client            7.1.2              pyhd3eb1b0_0
jupyter_core              4.9.2           py310haa95532_0
kealib                    1.4.14               hde4a422_1
krb5                      1.19.2               h5b6d351_0
libcurl                   7.80.0               h86230a5_0
libffi                    3.4.2                h604cdb4_1
libgdal                   3.4.1                h9b24a9a_0
libiconv                  1.15                 h1df5818_7
libnetcdf                 4.8.1                h6685c40_1
libpng                    1.6.37               h2a8f88b_0
libpq                     12.9                 hb652d5d_1
libspatialite             4.3.0a              h14feca5_20
libssh2                   1.9.0                h7a1dbc1_1
libtiff                   4.2.0                hd0e1b90_0
libxml2                   2.9.12               h0ad7f3c_0
libzip                    1.5.1             h05fb217_1003
lz4-c                     1.9.3                h2bbff1b_1
m2w64-expat               2.1.1                         2
m2w64-gcc-libgfortran     5.3.0                         6
m2w64-gcc-libs            5.3.0                         7
m2w64-gcc-libs-core       5.3.0                         7
m2w64-gettext             0.19.7                        2
m2w64-gmp                 6.1.0                         2
m2w64-libiconv            1.14                          6
m2w64-libwinpthread-git   5.0.0.4634.697f757               2
m2w64-xz                  5.2.2                         2
matplotlib-inline         0.1.2              pyhd3eb1b0_2
mkl                       2021.4.0           haa95532_640
mkl-service               2.4.0           py310h2bbff1b_0
mkl_fft                   1.3.1           py310ha0764ea_0
mkl_random                1.2.2           py310h4ed8f06_0
msys2-conda-epoch         20160418                      1
nest-asyncio              1.5.1              pyhd3eb1b0_0
numpy                     1.21.5          py310h4c31df0_0
numpy-base                1.21.5          py310hedd7904_0
openjpeg                  2.4.0                h4fc8c34_0
openssl                   1.1.1n               h2bbff1b_0
parso                     0.8.3              pyhd3eb1b0_0
pickleshare               0.7.5           pyhd3eb1b0_1003
pip                       21.2.4          py310haa95532_0
proj                      6.2.1                h3758d61_0
prompt-toolkit            3.0.20             pyhd3eb1b0_0
pure_eval                 0.2.2              pyhd3eb1b0_0
pygments                  2.11.2             pyhd3eb1b0_0
python                    3.10.4               hbb2ffb3_0
python-dateutil           2.8.2              pyhd3eb1b0_0
pywin32                   302             py310h827c3e9_1
pyzmq                     22.3.0          py310hd77b12b_2
setuptools                58.0.4          py310haa95532_0
six                       1.16.0             pyhd3eb1b0_1
sqlite                    3.38.2               h2bbff1b_0
stack_data                0.2.0              pyhd3eb1b0_0
tiledb                    2.2.9                hf7ce2e6_0
tk                        8.6.11               h2bbff1b_0
tornado                   6.1             py310h2bbff1b_0
traitlets                 5.1.1              pyhd3eb1b0_0
tzdata                    2022a                hda174b7_0
vc                        14.2                 h21ff451_1
vs2015_runtime            14.27.29016          h5e58377_2
wcwidth                   0.2.5              pyhd3eb1b0_0
wheel                     0.37.1             pyhd3eb1b0_0
wincertstore              0.2             py310haa95532_2
xerces-c                  3.2.3                ha925a31_0
xz                        5.2.5                h62dcd97_0
zlib                      1.2.11               hbd8134f_5
zstd                      1.4.9                h19a0ad4_0

(geoenv) C:\Users\Arellano\Documents\GitHub\PLUS_softwaredev_2022-3>conda config --add channels conda-forge

(geoenv) C:\Users\Arellano\Documents\GitHub\PLUS_softwaredev_2022-3>conda config --set channel_priority strict

(geoenv) C:\Users\Arellano\Documents\GitHub\PLUS_softwaredev_2022-3>conda install conda-forge::rasterio

```
