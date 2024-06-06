因為檔案太大，多個檔案進行內部壓縮，請自行解壓縮，因為訓練的模型過大，只留了一個最小的模型結果(剩下的放不上去，壓縮後依舊檔案過大)。
1. Install python(> 3.7) on Windows.
2. Use venv to run project.
   2.1 open cmd windows.  
   2.2 assume working folder is D:\test.  
   2.3 python -m venv venv, this step is to create venv environment folder in D:\test, all packages are installed here.  
   **2.4 .\venv\Scripts\activate.bat  
   2.5 git clone this github  
   **2.6 cd yolov5  
   2.7 pip install -r requirements.txt  
   2.8 install the weights you want and put in folder(ex: yolov5n.pt)  
   //train 
   2.9 python train.py  --batch 26 --epochs 500  --data datasets/hur.yaml --weights yolov5n.pt  
   //detect  
   **2.10 python detect.py --weight runs/train/exp/weights/best.pt  --source datasets\test  
