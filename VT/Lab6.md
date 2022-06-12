# Lab6: Ubuntu VM - Python虛擬環境介紹與應用

<a name="000"/>

#### 目錄

##### [6-1 虛擬環境? 創建 3 個虛擬環境](#001)
##### [6-2 使用Jupyter Notebook來快速複習Python程式，來點挑戰](#002)

<a name="001"/>

## Lab 6-1 虛擬環境? 創建 3 個虛擬環境

### A.安裝一個方便開發的 Python 虛擬環境:使用 Pyenv 管理 Python 版本

安裝前，先確認版本為Ubuntu最新版；有些版本會產生失誤。

![螢幕擷取畫面 2022-05-29 110444](https://user-images.githubusercontent.com/89327102/170852617-84650662-3e8f-4983-9a75-39b27e022cac.jpg)

````c
## Install Python packages (About N minutes)
python3 --version

Python 3.8.10

sudo apt-get install -y make build-essential libssl-dev zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm libncurses5-dev libncursesw5-dev xz-utils tk-dev libffi-dev liblzma-dev python-openssl python-dev

sudo apt-get install python3-pip

## --- install pyenv
 
sudo apt install curl 

curl -L https://raw.githubusercontent.com/yyuu/pyenv-installer/master/bin/pyenv-installer | bash

gedit ~/.bashrc

--- 將以下 4 行添加到 .bashrc 的底部

export PYENV_ROOT="$HOME/.pyenv"
export PATH="$PYENV_ROOT/bin:$PATH"
eval "$(pyenv init --path)"
eval "$(pyenv virtualenv-init -)"

--- 完成後, 記得儲存後, 關閉終端並再次打開一個新的Terminal
````

### B.在虛擬環境(pyenv)安裝python 3.6.5, 3.7.9, 3.9.13, (需要安裝一段時間)

安裝前，先確認版本為Ubuntu最新版；有些版本會產生失誤。

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

````
![螢幕擷取畫面 2022-05-29 121705](https://user-images.githubusercontent.com/89327102/170852826-cbde1757-144a-4a0f-acd8-ff8213278bbf.jpg)
![螢幕擷取畫面 2022-05-29 123524](https://user-images.githubusercontent.com/89327102/170852873-ced1da8c-a5a1-4b88-af1d-17f2eb03d47b.jpg)


### D.請參考以上作法, 再試試建立一個vnu365 Folder, 並且指定此Folder下只使用Python 3.6.5

![螢幕擷取畫面 2022-06-05 235703](https://user-images.githubusercontent.com/89327102/172059283-e37d906e-f985-4b12-af0e-30ea4136c708.jpg)


<a name="002"/>

## Lab 6-2 使用Jupyter Notebook來快速複習Python程式，來點挑戰其他題目!!


![螢幕擷取畫面 2022-06-06 002244](https://user-images.githubusercontent.com/89327102/172063746-dfa908b8-18f8-4d6d-b112-4ee8e8514f8a.jpg)

![螢幕擷取畫面 2022-06-12 122303](https://user-images.githubusercontent.com/89327102/173214364-1cdd3bed-9316-44be-a3bd-a8bc65c2aebb.jpg)

![螢幕擷取畫面 2022-06-06 004427](https://user-images.githubusercontent.com/89327102/172063751-3257bec7-b994-4fcc-8c37-43ec701c8ed0.jpg)

![螢幕擷取畫面 2022-06-06 012259](https://user-images.githubusercontent.com/89327102/172063758-32c83ff9-4bb7-435b-b758-4376c8dfa159.jpg)

![螢幕擷取畫面 2022-06-12 114151](https://user-images.githubusercontent.com/89327102/173213947-d04557e9-8ce6-4589-93e0-01a51edff3f9.jpg)

![螢幕擷取畫面 2022-06-12 115206](https://user-images.githubusercontent.com/89327102/173213948-ef414bd9-b888-4be7-bd31-1dd8df9a580b.jpg)

![螢幕擷取畫面 2022-06-12 115317](https://user-images.githubusercontent.com/89327102/173213952-220585df-1437-4957-9f4a-90321158ef9a.jpg)

![螢幕擷取畫面 2022-06-12 120026](https://user-images.githubusercontent.com/89327102/173213955-30484737-1960-407c-8398-8623a0d0e2f6.jpg)

![螢幕擷取畫面 2022-06-12 120235](https://user-images.githubusercontent.com/89327102/173213956-c12100bb-60e5-4905-9630-90ed4a18e3d0.jpg)

![螢幕擷取畫面 2022-06-12 120538](https://user-images.githubusercontent.com/89327102/173213964-a977d1ed-0cf1-44ba-be04-47357b9546b5.jpg)






