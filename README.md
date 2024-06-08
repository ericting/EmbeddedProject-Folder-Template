# Project Folder Template

嵌入式工程目录结构模板

> 感觉这个文件结构比较贴合个人和公司里边的实际开发

目录结构介绍

```
├─00_Project_Management			# 开发前的文档
│  ├─00_需求导入_QFD
│  ├─01_需求约束_Pugh
│  ├─02_需求转化_Basic_Statics
│  ├─03_功能图谱_Function_Map
│  ├─04_功能风险管控_DFMEA
│  ├─04_法规认证_国内_国外
│  ├─04_知识产权_国内_国外
│  ├─05_敏捷开发_Scrum
│  ├─06_持续集成与测试_DevOps
│  ├─07_产品生产管理_Six_Sigma
│  └─08_缺陷管理追踪_Jira
├─00_Reference					#参考文档
├─01_Function_Map				#功能具体需求清单、流程图...
├─02_Hardware					#硬件相关：原理图、PCB
│  ├─00_Ref
│  │  └─00_HDK					#Hardware Develop Toolkit
│  └─01_Project
├─03_Firmware					#放置版本.hex/.bin固件
├─04_Software					#软件代码
│  ├─00_Ref
│  │  └─00_SDK
|  |  └─....
│  └─01_Source_Code
├─05_Mechanical					#机械结构部分
├─06_FCT						#产品发布后的上位机工具..
└─07_Tools						#开发过程中用到的工具：自动测试、固件加密..。
....
```



- 使用`git bash`删除每个目录下的`.gitkeep`文件

```bash
find . -type d -not -path "*/.git*" -exec rm -f {}/.gitkeep \;

```

- 为空文件夹增加`.gitkeep`文件

```bash
find ./ -type d -empty -not -path "./.git/*" -exec touch {}/.gitkeep \;
```



参考

- [搞嵌入式，文件很多很乱？当始一个新的嵌入式项目，必做的准备工作--工程文件夹归档](https://www.bilibili.com/video/BV1E1421i7wJ/)

