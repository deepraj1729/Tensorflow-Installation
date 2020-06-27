# Tensorflow-Installation
Easy Installation of Tensorflow using CPU and GPU support

# Requirements:

1. Python (both using PIP and Conda)
2. NVIDIA GPU of Compute capability >= 6.0   (For GPU support) *optional for CPU support*
3. CPU RAM (8 GB or higher for efficient performance)
4. CUDA Drivers installed (Normally it's installed for NVIDIA Drivers) *optional for CPU support*

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
    
### 3. `TF <= 1.15.x` *Deprecated version*

    pip install tensorflow-cpu==1.15

# b. Tensorflow with GPU for CUDA >=10 and cuDNN>=7.6: (Virtual environment recommended for safety)

### 1. Using `pip`:
a. Create NVIDIA account:
    
    https://developer.nvidia.com/
    
b. Install cudatoolkit >= 10
        
        https://developer.nvidia.com/cuda-downloads
        
c. Install cuDNN >7.6 
         
        https://developer.nvidia.com/rdp/form/cudnn-download-survey
        
d. Install tensorflow GPU `TF >= 2.0` *Latest version*

    pip install tensorflow-gpu
    
   Install Tensorflow GPU  `== 2.x.x ` *Exact version say 2.0.0*
    
    pip install tensorflow-gpu==2.0.0
   
   Install Tensorflow GPU `<=1.15.x`  *Deprecated version say 1.15.0*
    
    pip install tensorflow-gpu==1.15.0
    

### 2. Using `conda`:
a. Install CUDA Toolkit (>= 10.0)
    
    conda install -c anaconda cudatoolkit

b. Install cuDNN (>= 7.6)
    
    conda install -c anaconda cudnn

c. Install Tensorflow GPU  `TF >= 2.0` *Latest version*
    
    conda install -c anaconda tensorflow-gpu
   
   
   Install Tensorflow GPU  `== 2.x.x ` *Exact version say 2.0.0*
    
    conda install -c anaconda tensorflow-gpu==2.0.0
   
   Install Tensorflow GPU  `<= 1.15.x ` *Exact version say 1.15.0*
    
    conda install -c anaconda tensorflow-gpu==1.15.0


### If there still exists an error like:
    
    dynamic cudartXX_xxx.dll library missing
    
   Install the correct cudartXX_xxx.dll dynamic library runtime from internet and add this to PATH variable (system/


## List of Tensorflow compatible versions with CUDA and cuDNN will be updated soon



    
