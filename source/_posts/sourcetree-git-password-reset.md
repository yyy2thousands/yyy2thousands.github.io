---
title: SourceTree重設Git密碼
abbrlink: 447131393
date: 2020-10-25 21:39:05
categories: 
- Git
tags: 
- git
- source tree
- github
---
## 遇到的問題  

一開始Github密碼輸入錯誤,或是修改了密碼誒，在push或是pull的時候source tree 會提示access denied，這是因為source tree一直使用錯誤的密碼到Github登入，當然是錯的拉！  

## 解決方法 

#### Mac 
1. 打開啟動程式 -> 搜索`鑰匙圈` 
 ![image](/image/post/sourcetree-git-password-reset-1.png)  
2. 打開鑰匙圈存取
3. 找到 `github.com Access Key for ${yourmail@mail}` 刪除

#### Windows
1. 打開C:\Users\${UserName}\AppData\Local\Atlassian\SourceTree\passwd
2. 刪除對應的key