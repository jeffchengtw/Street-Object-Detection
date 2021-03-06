# HW2
 yolov5

# Device
```
+-----------------------------------------------------------------------------+
| NVIDIA-SMI 456.71       Driver Version: 456.71       CUDA Version: 11.1     |
|-------------------------------+----------------------+----------------------+
| GPU  Name            TCC/WDDM | Bus-Id        Disp.A | Volatile Uncorr. ECC |
| Fan  Temp  Perf  Pwr:Usage/Cap|         Memory-Usage | GPU-Util  Compute M. |
|===============================+======================+======================|
|   0  GeForce RTX 2070   WDDM  | 00000000:01:00.0  On |                  N/A |
| 57%   48C    P2    43W / 175W |   1733MiB /  8192MiB |     11%      Default |
+-------------------------------+----------------------+----------------------+
```
# Env
torch==1.10.0+cu102 <br>
torchvision==0.11.1+cu102 <br>
```
pip install -r requirements.txt
```
# Inference
download best.pt
https://github.com/jeffchengtw/HW2/blob/main/best.pt
```
cd to path
python infer.py
```

# Inference on colab screenshot
data sorting in dataset.py<br>
```
class LoadImage:
   elif os.path.isdir(p):
              files = []
              data_listdir = os.listdir(path)
              data_listdir.sort(key = lambda x: int(x[:-4]))
              for name in data_listdir:
                  imgname = path + name
                  files.append(imgname)
```
![image](https://github.com/jeffchengtw/HW2/blob/main/screenshot/inference_colab2.PNG)

# Reference
https://github.com/chia56028/Street-View-House-Numbers-Detection<br>
https://github.com/ultralytics/yolov5<br>
https://github.com/penny4860<br>
