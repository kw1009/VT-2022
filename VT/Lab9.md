# Lab9: Ubuntu VM -  作業系統層虛擬化的Docker

<a name="000"/>

#### 目錄

##### [Lab 9-1 What Is Docker?](#001)
##### [Lab 9-2 How To Install Docker on Ubuntu?Lab 9-2 How To Install Docker on Ubuntu?](#002)
##### [Lab 9-3 什麼是Docker 映像檔（image）? 容器（container）?倉庫（repository）? Docker初體驗](#003)
##### [Lab 9-4 進入Docker Image的世界: Ubuntu ](#004)
##### [Lab 9-5 進入Docker Image的世界: Python3](#005)
##### [Lab 9-6 最後, 來試試建立自己的Docker Image. Let’s go!!](#0036)

<a name="001"/>

## Lab 9-1 What Is Docker?

作業系統層虛擬化（Operating system–level virtualization），亦稱容器化（英語：Containerization），是一種虛擬化技術，這種技術將作業系統核心虛擬化，可以允許使用者空間軟體實體（instances）被分割成幾個獨立的單元，在核心中運行，而不是只有一個單一實體運行。這個軟體實體，也被稱為是一個容器（containers），虛擬引擎（Virtualization engine），虛擬專用伺服器（virtual private servers）或是 jails。對每個行程的擁有者與使用者來說，他們使用的伺服器程式，看起來就像是自己專用的; 因此, 相對於傳統的虛擬化（Virtualization），容器化的優勢在於佔用伺服器空間少，通常幾秒內即可啟動。同時容器的彈性可以在資源需求增加時瞬時複製增容，在資源需求減小時釋放空間以供其他使用者使用。由於在同一台伺服器上的容器實體共享同一個系統核心，因此在運行上不會存在實體與主機操作系統爭奪RAM的問題發生，從而能夠保證實體的效能。


![da2641c24bf7427189572b2fb0257b07](https://user-images.githubusercontent.com/89327102/178128488-8129b89f-f274-4c39-a6a6-ddc59a21f266.png)

[TOP](#000)

<a name="002"/>

## Lab 9-2 How To Install Docker on Ubuntu?

![螢幕擷取畫面 2022-07-10 102718](https://user-images.githubusercontent.com/89327102/178128864-278dba32-5e54-4f74-9c79-de5e34d78acc.jpg)

[TOP](#000)

<a name="003"/>

## Lab 9-3 什麼是Docker 映像檔（image）? 容器（container）?倉庫（repository）? Docker初體驗

![螢幕擷取畫面 2022-07-10 103647](https://user-images.githubusercontent.com/89327102/178129023-1f2db8fe-ee4f-47f2-b69f-c27114f7a5a6.jpg)

[TOP](#000)

<a name="004"/>

## Lab 9-4 進入Docker Image的世界: Ubuntu 

![螢幕擷取畫面 2022-07-10 114052](https://user-images.githubusercontent.com/89327102/178130349-00d3aa77-dbcc-4db9-8e0e-fd57f99d204a.jpg)

[TOP](#000)

<a name="005"/>

## Lab 9-5 進入Docker Image的世界: Python3

![螢幕擷取畫面 2022-07-10 120550](https://user-images.githubusercontent.com/89327102/178130872-fc81b7d0-088d-41ca-bc5b-c2f34f588b1e.jpg)

[TOP](#000)

<a name="006"/>

## Lab 9-6 最後, 來試試建立自己的Docker Image. Let’s go!!

[TOP](#000)
