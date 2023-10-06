# Obsidian模版

## 一、说明

该仓库存储本人使用的`Obsidian`模版，实现了以下功能：

1. 附件统一存放
	1. 图片实现了本地存储/图床访问（将图片粘贴/拖拽后直接上传）
	2. 其他附件统一存放在`Attachment`文件中
2. 使用`Excalidraw`实现本地绘图
	1. 自定义中文字体
		![CleanShot 2023-10-06 at 17.20.53@2x.png](https://raw.githubusercontent.com/anglee0323/Picbed/main/CleanShot%202023-10-06%20at%2017.20.53%402x.png)
		
	2. 自定义常用素材库
	3. 使用`Slideshow`插件进行画布演示 
		![CleanShot 2023-10-06 at 17.40.13.gif](https://raw.githubusercontent.com/anglee0323/Picbed/main/CleanShot%202023-10-06%20at%2017.40.13.gif)

	4. 使用`Mindmap`插件快速绘制思维导图
		![CleanShot 2023-10-06 at 17.48.54.gif](https://raw.githubusercontent.com/anglee2002/Picbed/main/CleanShot%202023-10-06%20at%2017.48.54.gif)


3. 实现Obsidian内置Copilot（需要OpenAI API）
 ![CleanShot 2023-10-06 at 17.53.44.gif](https://raw.githubusercontent.com/anglee0323/Picbed/main/CleanShot%202023-10-06%20at%2017.53.44.gif)

4. 实现了Obsidian内置浏览器
   ![CleanShot 2023-10-06 at 17.58.14.gif](https://raw.githubusercontent.com/anglee0323/Picbed/main/CleanShot%202023-10-06%20at%2017.58.14.gif)

5. 实现代码高亮
6. 实现markdown代码片段直接运行
   ![CleanShot 2023-10-06 at 18.01.45.gif](https://raw.githubusercontent.com/anglee0323/Picbed/main/CleanShot%202023-10-06%20at%2018.01.45.gif)
7. 调整了UI为`Github`风格
8. 隐藏了菜单滚动
9. 使用`Github`进行同步
## 二、使用方法

1. 克隆仓库到本地
``` shell
cd 
cd Desktop
git clone https://github.com/anglee0323/ObsidianTemplate.git
```
2. 删除`.git`文件、`Readme.md`文件以及`Placeholder.txt `文件
``` shell
cd ObsidianTemplate
rm -rf .git
rm -rf Readme.md
cd ..
find ./ObsidianTemplate -name "Placeholder.txt" -delete
```
3. 新建`.git`文件，并配置仓库或使用icloud进行同步
``` shell
cd ~/Desktop/ObsidianTemplate
git init 
git add .
git commit -m "initial commit"
```

>若您使用icloud进行同步，则使用以下命令并忽略`4.`和`5.`步骤（若您的icloud文件位置不同请自行更改）

```shell
mv ~/Desktop/ObsidianTemplate ~/Library/Mobile\ Documents/iCloud~md~obsidian/Documents
```

> 关闭`Obsidian Git`插件

4. 添加远程仓库

``` shell
git remote add origin <your repo link.git>
git push --set-upstream origin main
```

5. 设置`Obsidian Git`插件自动推送时间

> 建议设置每10分钟自动备份一次


## 三、组织结构

```
Obsidian Template

├── README.md //README文档
├── Attachment //附件
│	     └── Placeholder.txt //占位文件，保证文件夹存在
│	     └── Copilot //AI对话副本
│	     └── Excalidraw //Excalidraw白板
│	     └── Templates //Obsidian模版文件
└── Plugins //插件
│   └── Excalidraw 
│        └── Fonts //字体
│	     │    └── DongJingJieJiaoDeXiaoLangMan-2 //中文Excalidraw风格字体
│        └── Library //绘图素材
│        └── Scripts //脚本
│             └── Downloaded //由第三方下载
└── Source //资源文件，用于存放Pdf，Epub，Hand-Write-Notes等
│	     └── Placeholder.txt //占位文件，保证文件夹存在
└── .git //git配置文件(需自行删除)
└── .obsidian //obsidian配置文件
	     └── plugins //插件文件
	     └── themes //主题文件
	     └── xxx.json //快捷键,工作区,插件配置文件
	 
```
## 四、其他

* 对于`Excalidraw`绘图，可以配合`Raycast插件`通过`icons8`网站获取矢量图片
> 具体参考: https://www.raycast.com/yug2005/icons8

![效果展示](https://raw.githubusercontent.com/anglee0323/Picbed/main/CleanShot%202023-10-06%20at%2017.03.49%402x.png)




