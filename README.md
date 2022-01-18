# virtualenv

pip install virtualenv

# 方法1 ----- 下語法創建資料夾
$ virtualenv xxx_env

# 方法2 ----- 創建資料夾後 加入venv資料夾
$ python3 -m venv tutorial-env


# Mac:
$ source xxx_env/bin/activate

# window:
自己測試可運行指令:
$ .venv\Scripts\activate
<img width="314" alt="2022-01-07_16h32_11" src="https://user-images.githubusercontent.com/66947341/148515442-ab017d65-6e21-4925-a385-db3f7d6e4fcd.png">
<img width="276" alt="2022-01-07_16h34_57" src="https://user-images.githubusercontent.com/66947341/148515789-e26fb991-e623-4b80-a132-e0fd9de5fe2f.png">


#原來之前使用pycharm中有看到 venv這個資料夾 就是pycharm有內建virtualenv的服務
<img width="357" alt="2022-01-07_16h33_41" src="https://user-images.githubusercontent.com/66947341/148515623-c449aee0-08a8-48c5-9326-82f1e1b86bea.png">
<img width="128" alt="2022-01-07_16h34_02" src="https://user-images.githubusercontent.com/66947341/148515677-7cc2baa4-79b9-4539-8409-c3afa485617f.png">


# pycharm直接用綠色箭頭無法run -> interpreter找不到
1. setting中 ~ 在原有專案目錄加入interpreter
2. 再到 run/edit configurations選擇剛剛新增的interpreter就好囉
<img width="775" alt="2022-01-18_17h24_33" src="https://user-images.githubusercontent.com/66947341/149908495-38786a09-fb28-4dd9-8edb-20c71de32722.png">

# phcharm在Terminal和interpreter目錄不同. Terminal沒有進入虛擬環境
下 venv\Scripts\activate 或 venv\Scripts\activate.bat 或 venv\Scripts\activate.ps1 都沒反應
右鍵~以系統管理員身分~執行power shell
<img width="951" alt="2022-01-18_17h54_08" src="https://user-images.githubusercontent.com/66947341/149913988-8edbb0c8-2c80-49ec-a03d-51ecd921a14b.png">
ref:
https://docs.microsoft.com/zh-tw/powershell/module/microsoft.powershell.core/about/about_signing?view=powershell-7.2

# 改專案資料夾名稱的時候, 內部路徑都沒改到
<img width="566" alt="2022-01-18_17h35_14" src="https://user-images.githubusercontent.com/66947341/149910571-9ad9361a-3bcd-4b05-8162-9e6f3e9e3e16.png">
對專案資料夾按右鍵-> replace in file -> 全部修改
<img width="211" alt="2022-01-18_17h42_11" src="https://user-images.githubusercontent.com/66947341/149911826-aad29792-2dbf-4636-89d7-e886f01a2ff0.png">
<img width="773" alt="2022-01-18_17h40_48" src="https://user-images.githubusercontent.com/66947341/149911866-22c0769a-5957-4478-8d03-7d1afc5e5b53.png">



# 注意
需要使用power shell才能執行. 勿在終端機中下語法
安裝requirements.txt之類的記得在power shell前面要看到(venv)
<img width="254" alt="2022-01-07_16h36_15" src="https://user-images.githubusercontent.com/66947341/148515963-082f53f0-c3c9-4256-9b1d-306cce3b9c0e.png">
<img width="228" alt="2022-01-07_16h36_34" src="https://user-images.githubusercontent.com/66947341/148515997-1cab7cfd-73e8-4746-ba91-e65d26aae61c.png">

#參考
It's django 2.3虛擬環境 p.76
