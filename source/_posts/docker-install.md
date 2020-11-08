---
title: Docker安裝
categories:
  - Docker
tags:
  - docker
abbrlink: 2017388798
date: 2020-11-07 12:59:48
---

, 

## MAC 安裝
+ 硬體版本 2010年之後出廠的Mac 
  可以使用命令行檢查 `sysctl kern.hv_support` ，可以安裝Docker會看到`kern.hv_support: 1`
+ 系統版本 最低 macOS OS X El Capitan 10.11
+ RAM     4G以上 

#### HomeBrew 安裝
`brew cask install docker`

#### 手動安裝
[安裝包下載](https://www.docker.com/get-started)  

下載後將Docker拉到Applications
![image](/image/post/docker-logo.jpg)  


## 啟用Docker  
安裝後直接打開命令行執行`docker run -d -p 80:80 docker/getting-started`  

+ 點擊工作面板上的小鯨魚，點擊Dashboard就可以打開Docker管理畫面
+ 再點擊Open In Browser就可以在瀏覽器看到Docker已經快速的架起第一個網站   
![image](/image/post/docker-logo.jpg)  


----------------------------------------------------------------------------------

## Window 10 專業版 安裝
+ 64bit   處理器  
+ RAM     4G以上  
+ BIOS 啟用虛擬化 

[安裝包下載](https://www.docker.com/get-started)   
下載後直接安裝就可以


Windows 10 專業版因為有Hyper-V，可以直接下載Docker後安裝，如果windows沒有啟用Hyper-V，可以參考
[Hyper-V啟用教學](https://docs.microsoft.com/zh-tw/virtualization/hyper-v-on-windows/quick-start/enable-hyper-v)  

> Hyper-V 可讓您在 Windows 上將多個作業系統執行為虛擬機器

## Windows 10 家庭版, windows 8, windows 7 安裝
+ 硬體需求與Windows 專業版相同  

> Hyper-V 適用於 64 位元版的 Windows 10 專業版、企業版和教育版。 但不適用於家用版。  

因為這些版本沒有Hyper-V，因此需要先在windows建立一個虛擬機，然後在虛擬機上面執行Docker。 
我們可以用Docker Toolbox來安裝，或是在Windows 10 家用版啟用Hyper-V，因為我手上也沒這些版本的window電腦，  
請自行google `window10 家用版安裝` 或是參考以下安裝方法     

以下為簡體中文網站，不喜勿近  
[Docker Toolbox安裝Docker教學](https://www.runoob.com/docker/windows-docker-install.html)   
[Docker Toolbox 下載](http://mirrors.aliyun.com/docker-toolbox/windows/docker-toolbox/)


## Ｄocker官方安裝教學
##### [官網安裝教學 Mac](https://docs.docker.com/docker-for-mac/install/)  
##### [官網安裝教學 Windows Pro](https://docs.docker.com/docker-for-windows/install/)
##### [官網安裝教學 Windows Home](https://docs.docker.com/docker-for-windows/install-windows-home/)  