# Lab7: Ubuntu VM - Python虛擬環境應用: AI自駕車路徑預測

<a name="000"/>

#### 目錄

##### [Lab 7-1 Folk我們想要研究的Respository, 並且來點小修改, 最後再克隆一份到我們的VM Ubuntu](#001)
##### [Lab 7-2 AI Self Driving Car - Lane and Path Detection](#002)
##### [Lab 7-3 程式架構簡介與說明, 如何將影像與路徑結合? ](#003)

<a name="001"/>

## Lab 7-1 Folk我們想要研究的Respository, 並且來點小修改, 最後再克隆一份到我們的VM Ubuntu


git clone from our Ubuntu VM

![螢幕擷取畫面 2022-06-19 104210](https://user-images.githubusercontent.com/89327102/174463668-b61443f9-0e55-44da-9e49-888c158984b4.jpg)

<a name="002"/>

## Lab 7-2 AI Self Driving Car - Lane and Path Detection

sudo apt update
sudo pip3 install --upgrade tensorflow requests

pip install -r requirements.txt
pip3 install PyQt5==5.9.2

pip install --upgrade pip

![螢幕擷取畫面 2022-06-19 104951](https://user-images.githubusercontent.com/89327102/174464283-27022a86-40d5-478b-9ac4-ddf4f566a4c8.jpg)

![螢幕擷取畫面 2022-06-19 110412](https://user-images.githubusercontent.com/89327102/174464287-35ec415a-1d98-42f6-9f2e-e8e0c40f9737.jpg)

![螢幕擷取畫面 2022-06-19 110502](https://user-images.githubusercontent.com/89327102/174464290-235d3029-5b52-4a38-99f1-2765f24f360f.jpg)

![螢幕擷取畫面 2022-06-19 110535](https://user-images.githubusercontent.com/89327102/174464295-d223434b-d892-4702-80e5-1cbfd94b6991.jpg)

![螢幕擷取畫面 2022-06-19 110624](https://user-images.githubusercontent.com/89327102/174464298-19d5631f-6e7c-4092-be69-a24435ecc1e4.jpg)

![螢幕擷取畫面 2022-06-19 110838](https://user-images.githubusercontent.com/89327102/174464301-ab49591f-1d62-421b-b702-ac42af863df5.jpg)

測試影片必須從虛擬機端下載

python3 main.py sample.hevc

![螢幕擷取畫面 2022-06-19 120546](https://user-images.githubusercontent.com/89327102/174465441-7590083c-4dfe-4337-8275-40a30b8190be.jpg)

<a name="003"/>

## Lab 7-3 程式架構簡介與說明, 如何將影像與路徑結合?

python3 lane_visulaizer_dynamic.py sample.hevc

![螢幕擷取畫面 2022-06-19 121147](https://user-images.githubusercontent.com/89327102/174465526-d7c65fb7-a3a9-467e-b6ca-ba674d82ae9a.jpg)

