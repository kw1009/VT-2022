# Lab 5-1 安裝, 測試Apache Server, 並且架設自己的網站

<a name="000"/>

#### 目錄
##### [5-1 安裝, 測試Apache Server, 並且架設自己的網站](#001)
##### [5-2 Apache 網頁伺服器起手式](#002)
##### [5-3 Apache 網頁伺服器應用](#003)

<a name="001"/>

### A.安裝

sudo apt update && sudo apt install apache2

![螢幕擷取畫面 2022-05-08 110216](https://user-images.githubusercontent.com/89327102/167280033-4d0dfd44-8d5e-4b3b-b4c8-799fa981a807.jpg)

### B.測試: 確認是否有active (running) ?

sudo service apache2 status

![螢幕擷取畫面 2022-05-08 110503](https://user-images.githubusercontent.com/89327102/167280039-8b423edb-4e7c-4f89-8520-794c8e9a59af.jpg)

### C.從你的Ubuntu Browser和Windows Browser來連到你的Web Site看看囉

sudo apt install net-tools
ifconfig

![螢幕擷取畫面 2022-05-08 112202](https://user-images.githubusercontent.com/89327102/167280370-1506ed21-ded0-4676-aa96-caa55adbeac6.jpg)
![螢幕擷取畫面 2022-05-08 112218](https://user-images.githubusercontent.com/89327102/167280375-e7fb7d3a-afee-45f4-9157-76f6b2adcf6b.jpg)

[TOP](#000)

<a name="002"/>

# 5-2 Apache 網頁伺服器起手式

## 1.你在Apache Server的第1個Web Page

### A.我們的網頁存在哪呢 ?? 該如何編輯呢??

![螢幕擷取畫面 2022-05-08 114252](https://user-images.githubusercontent.com/89327102/167281146-7f5c93a7-03dd-428e-9a31-7ad7d02e65da.jpg)

### B.修改前, 記得先備份! 怎麼做呢?

sudo cp index.html index_bkup.html

![螢幕擷取畫面 2022-05-08 120418](https://user-images.githubusercontent.com/89327102/167281292-5c1ea409-157e-4ec8-a790-33b9c443a2de.jpg)

### C. 參考結果與作法:

sudo gedit /var/www/html/index.html

![螢幕擷取畫面 2022-05-09 013016](https://user-images.githubusercontent.com/89327102/167308166-6d8042ea-b53a-4b79-8eef-33f6dbbadb24.jpg)


## 2.再來玩第2個Web Page

### A.參考作法&結果

![螢幕擷取畫面 2022-05-09 015059](https://user-images.githubusercontent.com/89327102/167308980-5d066b2e-cf88-446c-81e6-eda45eacb31d.jpg)

## 3.再來玩第3個Web Page

### A.該如何用目錄來管理不同的網頁呢? 

![螢幕擷取畫面 2022-05-09 020245](https://user-images.githubusercontent.com/89327102/167309520-6a8f24be-973d-43f1-9a9b-6c6d01943e87.jpg)

### B.參考作法&結果

![螢幕擷取畫面 2022-05-09 020927](https://user-images.githubusercontent.com/89327102/167309558-de0d9920-f470-477d-8efd-7866738d76cf.jpg)

## 4.最後, 來玩點不一樣的, 可否把校網搬過來試試呢?

### A.參考作法&結果

![螢幕擷取畫面 2022-05-09 025201](https://user-images.githubusercontent.com/89327102/167311184-7942fe70-d011-4492-a497-9659f37e6a4b.jpg)

[TOP](#000)

<a name="003"/>

# 5-3 Apache 網頁伺服器應用

````
sudo apt install git            先安裝 git 命令
git clone 擷取網頁路徑           copy 網頁路徑內容
sudo cp -r clock /var/www/html  將 網頁路徑內容 copy 至 html 目錄下 。 #先確定此路徑沒東西在copy 有東西則會出現錯誤訊息
cd /var/www/html/clock          路徑變更
sudo chmod 777 index.html       權限變更
gedit index.html                編輯此網頁
````

## 實戰1

### A.Clock

![螢幕擷取畫面 2022-05-22 120503](https://user-images.githubusercontent.com/89327102/169678086-562dafe7-3d95-477c-aed9-b40137195b72.jpg)

### B.BMI Calculator

![螢幕擷取畫面 2022-05-22 121552](https://user-images.githubusercontent.com/89327102/169678342-5e511fbe-3c9f-4e77-99bb-78420a7c9a26.jpg)

## 實戰2

![螢幕擷取畫面 2022-05-22 123820](https://user-images.githubusercontent.com/89327102/169678936-206f0909-0f4b-4005-98c5-ebde0b7ece5f.jpg)



[TOP](#000)
