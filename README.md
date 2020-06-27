# Tensorflow-Installation
Easy Installation of Tensorflow for both `CPU` and `GPU` support

# Requirements:

1. Python (both using `pip` and `conda`)
2. `CPU RAM 8 GB or higher` for efficient performance  (Recommended for both supports)
3. `CUDA enabled GPU` having Compute capability >= 3.0    (For GPU support)    *optional for CPU support*
4. `Microsoft Visual Studio` >=2015 (for compatibility)

# Check your NVIDIA GPU's Compute Capability here:
https://developer.nvidia.com/cuda-gpus#compute

# Installation Options:
a. Install Tensorflow using `CPU` support  (By Default)

b. Install Tensorflow using `GPU` support

# Recommended (optional):
### A Virtual Environment with `virtualenv` or `conda`

## a. Install Tensorflow with CPU support:
### 1. `TF >= 2.0` *latest version*
    
    pip install tensorflow-cpu

### 2. `TF == 2.x.x`   *Exact version say 2.1.0*
  
    pip install tensorflow-cpu==2.1.0
    
### 3. `TF <= 1.15.x`   *Deprecated version*

    pip install tensorflow-cpu==1.15

## Check all releases of `tensorflow-cpu` on PyPi here:
https://pypi.org/project/tensorflow-cpu/#history


## b. Install Tensorflow with GPU support with CUDA >=10.0 and cuDNN>=7.6:  (Virtual environment recommended for safety)

### 1. Using `pip`:
a. Create NVIDIA account:
https://developer.nvidia.com/
    
b. Install cudatoolkit >= 10    
https://developer.nvidia.com/cuda-downloads
        
c. Install cuDNN >7.6         
https://developer.nvidia.com/rdp/form/cudnn-download-survey

Helping Guide for setting up cuDNN and Cudatoolkit for different `OS platforms`:

[For Windows](https://docs.nvidia.com/deeplearning/sdk/cudnn-install/index.html#install-windows)

[For Linux](https://docs.nvidia.com/deeplearning/sdk/cudnn-install/index.html#install-linux)

[For Mac](https://docs.nvidia.com/deeplearning/sdk/cudnn-archived/cudnn_741/cudnn-install/index.html#install-mac)

d. Install tensorflow GPU `TF >= 2.0`    *Latest version*

    pip install tensorflow-gpu
    
   Install Tensorflow GPU  `== 2.x.x `   *Exact version say 2.0.0*
    
    pip install tensorflow-gpu==2.0.0
   
   Install Tensorflow GPU `<=1.15.x`     *Deprecated version say 1.15.0*
    
    pip install tensorflow-gpu==1.15.0
    

### 2. Using `conda`:
a. Install CUDA Toolkit (>= 10.0) (recommended)
    
    conda install -c anaconda cudatoolkit

b. Install cuDNN (>= 7.6.5)
    
    conda install -c anaconda cudnn

c. Install Tensorflow GPU  `TF >= 2.0`    *Latest version*
    
    conda install -c anaconda tensorflow-gpu
   
   
   Install Tensorflow GPU  `== 2.x.x `    *Exact version say 2.0.0*
    
    conda install -c anaconda tensorflow-gpu==2.0.0
   
   Install Tensorflow GPU  `<= 1.15.x `   *Exact version say 1.15.0*
    
    conda install -c anaconda tensorflow-gpu==1.15.0


### If there still exists an error like:
    
    dynamic cudartXX_xxx.dll library missing
    
   Install the correct cudartXX_xxx.dll dynamic library runtime from internet and add this to PATH variable (system/


## List of Tensorflow compatible versions with CUDA and cuDNN:

### Tensorflow CPU Support configurations:

            Version	        Python version	        Compiler   
        
        tensorflow-2.2.0	    3.5-3.8	            MSVC 2019	
        tensorflow-2.1.0	    3.5-3.7	            MSVC 2019	
        tensorflow-2.0.0	    3.5-3.7	            MSVC 2017	
        tensorflow-1.15.0	    3.5-3.7	            MSVC 2017	
        tensorflow-1.14.0	    3.5-3.7	            MSVC 2017 
        tensorflow-1.13.0	    3.5-3.7	            MSVC 2015 update 3	
        tensorflow-1.12.0	    3.5-3.6	            MSVC 2015 update 3	
        tensorflow-1.11.0	    3.5-3.6	            MSVC 2015 update 3	
        tensorflow-1.10.0	    3.5-3.6	            MSVC 2015 update 3	
        tensorflow-1.9.0	    3.5-3.6	            MSVC 2015 update 3	
        tensorflow-1.8.0	    3.5-3.6	            MSVC 2015 update 3	
        tensorflow-1.7.0	    3.5-3.6	            MSVC 2015 update 3	
        tensorflow-1.6.0	    3.5-3.6	            MSVC 2015 update 3	
        tensorflow-1.5.0	    3.5-3.6	            MSVC 2015 update 3	
        tensorflow-1.4.0	    3.5-3.6	            MSVC 2015 update 3	
        tensorflow-1.3.0	    3.5-3.6	            MSVC 2015 update 3	
        tensorflow-1.2.0	    3.5-3.6	            MSVC 2015 update 3	
        tensorflow-1.1.0	    3.5	                MSVC 2015 update 3	
        tensorflow-1.0.0	    3.5	                MSVC 2015 update 3	


### Tensorflow GPU Support configurations:

            Version	        Python version	        Compiler	            cuDNN	    CUDA

        tensorflow_gpu-2.2.0	3.5-3.8	            MSVC 2019		        7.4	        10.1
        tensorflow_gpu-2.1.0	3.5-3.7	            MSVC 2019		        7.4	        10.1
        tensorflow_gpu-2.0.0	3.5-3.7	            MSVC 2017		        7.4	        10
        tensorflow_gpu-1.15.0	3.5-3.7	            MSVC 2017		        7.4	        10
        tensorflow_gpu-1.14.0	3.5-3.7	            MSVC 2017		        7.4	        10
        tensorflow_gpu-1.13.0	3.5-3.7	            MSVC 2015 update 3		7.4	        10
        tensorflow_gpu-1.12.0	3.5-3.6	            MSVC 2015 update 3		7	        9
        tensorflow_gpu-1.11.0	3.5-3.6	            MSVC 2015 update 3		7	        9
        tensorflow_gpu-1.10.0	3.5-3.6	            MSVC 2015 update 3		7	        9
        tensorflow_gpu-1.9.0	3.5-3.6	            MSVC 2015 update 3		7	        9
        tensorflow_gpu-1.8.0	3.5-3.6	            MSVC 2015 update 3		7	        9
        tensorflow_gpu-1.7.0	3.5-3.6	            MSVC 2015 update 3		7	        9
        tensorflow_gpu-1.6.0	3.5-3.6	            MSVC 2015 update 3		7	        9
        tensorflow_gpu-1.5.0	3.5-3.6	            MSVC 2015 update 3		7	        9
        tensorflow_gpu-1.4.0	3.5-3.6	            MSVC 2015 update 3		6	        8
        tensorflow_gpu-1.3.0	3.5-3.6	            MSVC 2015 update 3		6	        8
        tensorflow_gpu-1.2.0	3.5-3.6	            MSVC 2015 update 3		5.1	        8
        tensorflow_gpu-1.1.0	3.5	                MSVC 2015 update 3		5.1	        8
        tensorflow_gpu-1.0.0	3.5	                MSVC 2015 update 3		5.1	        8



