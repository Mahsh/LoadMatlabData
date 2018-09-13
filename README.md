# LoadMatlabData

This script loads .mat file in python, transfers matrix to python ndarray type data. 

```
import scipy.io as sio
import numpy as np

if __name__ == "__main__":
    mat = sio.loadmat('./smallworld256_sourcedata_SI.mat')  # mat is a dictionary
    print(type(mat))
    print(mat)
    print(mat['smallworld256_label_SI_block'].shape)
    new_data1 = mat['smallworld256_label_SI_block']   # smallworld256_label_SI_block and smallworld256_observedata_SI are two variables store in smallworld256_sourcedata_SI.mat.
    new_data2 = mat['smallworld256_observedata_SI']
    print(type(new_data1))
    print(new_data1)
```


running result shows below

![image](https://github.com/Mahsh/LoadMatlabData/blob/master/images/running%20result.png?raw=true)
