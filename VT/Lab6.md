# Lab6: Ubuntu VM - Python虛擬環境介紹與應用

<a name="000"/>

#### 目錄

##### [6-1 虛擬環境? 創建 3 個虛擬環境](#001)
##### [6-2 使用Jupyter Notebook來快速複習Python程式](#002)

<a name="001"/>

## Lab 6-1 虛擬環境? 創建 3 個虛擬環境

### A.安裝一個方便開發的 Python 虛擬環境:使用 Pyenv 管理 Python 版本

![螢幕擷取畫面 2022-05-29 110444](https://user-images.githubusercontent.com/89327102/170852617-84650662-3e8f-4983-9a75-39b27e022cac.jpg)

### B.在虛擬環境(pyenv)安裝python 3.6.5, 3.7.9, 3.9.13, (需要安裝一段時間)

````c
安裝前，先確認版本為Ubuntu最新版；有些版本會產生失誤。
````

![螢幕擷取畫面 2022-05-29 120932](https://user-images.githubusercontent.com/89327102/170852663-94226229-8b7b-49a2-82ab-1a7802f16b70.jpg)

如何確認目前的Virtual Environment中有哪些Python版本可用? Ans: pyenv versions

![螢幕擷取畫面 2022-05-29 121013](https://user-images.githubusercontent.com/89327102/170852758-595f8a72-59d6-4cfd-bbf1-8adbf65872a8.jpg)


### C.在~之下, 建立一個vnu379 Folder, 並且指定此Folder下只使用Python 3.7.9; 之後, 在我們的Ubuntu VM安裝Jupyter Notebook

![螢幕擷取畫面 2022-05-29 121338](https://user-images.githubusercontent.com/89327102/170852793-8c53fff2-42e4-44f5-90c1-d173a0f759c5.jpg)

````c
# 1 建立一個vnu379 Folder
mkdir vnu379
pyenv virtualenv 3.7.9 vnu379
cd vnu379

# 2 指定此Folder下只使用Python 3.7.9
pyenv local vnu379
python --version

# 3 安裝我們的老朋友Jupyter Notebook
(vnu379) ta@ubuntu:~/vnu379$ sudo snap install jupyter
 
# 4 完成後, 請重新起重Ubuntu VM, 即可以開始體驗Jupyter Notebook

![螢幕擷取畫面 2022-05-29 121705](https://user-images.githubusercontent.com/89327102/170852826-cbde1757-144a-4a0f-acd8-ff8213278bbf.jpg)
