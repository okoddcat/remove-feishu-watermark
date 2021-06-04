# 飞书去水印



## 飞书聊天去水印



### 步骤



1. 打开飞书网页版
2. 网页右键 审查元素 (inspect)
3. 选择 控制台 (console)
4. 复制下面的代码并回车
   1. `document.getElementsByClassName("lark-water-mark-main")[0].style.display = "none"`



## 飞书文档去水印

### 步骤

1. 打开飞书文档
2. 网页右键 审查元素 (inspect)
3. 选择 控制台 (console)
4. 复制下面的代码并回车
   1. `var index = 0; var ele; document.getElementsByTagName("div").forEach(element => {if (element.style.zIndex >= index){index = element.style.zIndex;ele = element;}}); ele.style.background = 'none';`

