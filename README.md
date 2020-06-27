# Tensorflow-Installation
Easy Installation of Tensorflow using CPU and GPU support

# Requirements:

1. Python (both using PIP and Conda)
2. NVIDIA GPU of Compute capability >= 6.0   (For GPU support) *optional*
3. CPU RAM (8 GB or higher for efficient performance)
4. CUDA Drivers installed (Normally it's installed for NVIDIA Drivers)

# Process:
a. Install Tensorflow using CPU support (By default)

b. Install Tensorflow using GPU support

# Recommended:
1. A Virtual Environment using virtualenv or Conda

# a. Tensorflow with CPU:
### 1. `TF >= 2.0` *latest version*
    
    pip install tensorflow-cpu

### 2. `TF == 2.x.x` *Exact version say 2.1.0*
  
    pip install tensorflow-cpu==2.1.0
    
### 3. `TF == 1.x.x` *Deprecated version*

    pip install tensorflow-cpu==1.15

# b. Tensorflow with GPU for CUDA >=10 and cuDNN>=7.6: (Virtual environment recommended for safety)

### 1. Using `pip`:
a. Install cudatoolkit >= 10
        
        https://developer.nvidia.com/cuda-downloads
        
b. Install cuDNN >7.6 
         
        https://developer.nvidia.com/rdp/form/cudnn-download-survey
        
c. Install tensorflow GPU 

    pip install tensorflow-gpu

### 2. Using `conda`:
a. Create NVIDIA account:
    
    https://developer.nvidia.com/
    
b. Install CUDA Toolkit (>= 10.0)
    
    conda install -c anaconda cudatoolkit

c. Install cuDNN (>= 7.6)
    
    conda install -c anaconda cudnn

d. Install Tensorflow GPU  `TF >= 2.0` *Latest version*
    
    conda install -c anaconda tensorflow-gpu
   
   
   Install Tensorflow GPU  `== 2.x.x ` *Exact version say 2.0.0*
    
    conda install -c anaconda tensorflow-gpu==2.0.0


### If there still exists an error like:
    
    dynamic cudartXX library missing
    
   Install the correct cudartXX.dll dynamic library from internet and add this to path


# List of Tensorflow compatible versions with CUDA and cuDNN will be updated soon



    
