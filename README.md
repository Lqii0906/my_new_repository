# Linux高级编程(第四阶段)
## Github
***关键字查询 awesome,去此标签类别中查询项目***<br>
***python tutorial,查询资料，书籍，文档***<br>
***socket sample,查询对应技术的代码样本***
## github三要素
### ***Repository 仓库***
***仓库是github项目管理存储基本单位***<br>
***一个仓库中存储一个项目，一个用户可以拥有多个仓库，一般仓库分为public,private***<br>
### ***Commit 提交***
***程序员在整个开发周期，有大量的对代码资源的迭代和修改，都可以通过commit的方式进行记录，便于程序员回溯代码，即使这些代码被删除提交便于使用者观察整个工程的开发流程以及设计流程***
### ***Branch 分支***
***在仓库中可以包含多个分支，分支才是代码文件的第一存储单位，默认的仓库主分支为master/main***<br>
\*不仅可以管理代码存储，便于多人协作开发
[![2.png](https://i.postimg.cc/FRVxSgNx/2.png)](https://postimg.cc/k6D83SVV)
<br>
## 仓库内容
***Code,资源存储，代码资源，二进制，项目管理脚本，许可证等等***<br>
***issues,使用时遇到的bug或进行提交，等待反馈***<br>
***README,使用markdown语言编写，工程自述文件，开发进度，版本更新，使用介绍等等***<br>
***LICENSE 许可证***<br>
***GPL 2.0,3.0 Apahce 2.0,Mit,这些许可证给使用者最大使用权限以及最少的限制***
## Git软件，分布式版本控制系统
***仓库管理软件，使用git管理私人代码或企业代码***<br>
[![3.png](https://i.postimg.cc/Kj9rqGKk/3.png)](https://postimg.cc/Lg11hM32)
<br>
## 设备认证
***1.如何让网站的账户与设备绑定，后续完成代码的管理，上传，下载***<br>
***git init //创建本地仓库        \*后续对仓库的操作，都在仓库位置(master)***<br>
***git config --list //查看git的配置文件***<br>
***git config --global user.email "邮箱"***<br>
***git config --global user.name "用户名"***<br>
***ssh-keygen -t rsa -C "注册邮箱" //创建本地密文***<br>
***SSH 远程访问***<br>
***\*去对应的目录查找密文文件***<br>
***rsa.pub 复制密文，粘贴 settings->SSH key and GPG -> new ssh key ->粘贴***<br>
***ssh -T git@github.com //测试关联成功***<br>
***2.为仓库起别名，定位目标仓库，后续上传***<br>
***git remote add origin "ssh地址" //为ssh仓库地址创建别名为origin***<br>
***git remote remove origin //删除origin别名***<br>
***git remote add origin "ssh地址" //为ssh仓库地址创建别名origin***<br>
## 本地设备与云端仓库的交互逻辑
[![4.png](https://i.postimg.cc/zGNKCH2t/4.png)](https://postimg.cc/BXhjsb0H)
***git add //添加内容***<br>
***git rm //删除冰帝文件并删除仓库数据***<br>
***git restroe //恢复被删除的(仓库存在)***<br>
## 代码更新的依赖关系被破坏
***本地内容要比云端新，完成更新替换，但是如果直接修改云端内容，导致本地内容无法再次提交***<br>
***\*先拉取git pull 云端内容 与本地内容合并或操作后再次提交即可***<br>
***git pull --rebase origin master***<br>
***git rebase --skip "忽略本地内容 保留云端内容"***<br>
***git rebase --abort "忽略云端内容 保留本地内容"***<br>
***git rebase --continue "合并两内容"***<br>
## 下载开源代码
***git clone "https仓库地址" //下载开源项目code资源***<br>
## 分支Branch
***\*关于分支的相关命令，创建分支，选择分支，合并分支等等***<br>
## Markdown 语言
***github可以编写readme，文本修饰语言***<br>
***MarkDown，文本修饰语言，用特殊符号修饰正文效果***<br>
## 标题修饰符\#
# 标题修饰符(一级标题)
## (二级标题)
### (三级标题)
#### (四级标题)
##### (五级标题)


## 正文内容
输入正文内容，需要换行用\<br\>标签<br>
## 修饰正文
*一段测试文本*
**一段测试文本**
***一段测试文本***
~~一段测试文本~~<br>

## 分割线
用\-\-\-表示分割线
--- 
## 引用效用\>表示
> 一级引用
>> 二级引用
>>> 三级引用
>>>> 四级引用<br>
## 列表修饰符
### 无序列表 \*
* 二次元游戏
	* 原神
		* 神里绫华
* 大逃杀
	* PUBG
	* APEX<br>
### 有序列表 1.
1. 物理学
	1. 粒子物理
	2. 原子核物理
	3. 凝聚态物理
2. 计算机科学
	1. 分布式架构
	2. 云计算
### 混合列表
1. 测试一级
	* 测试二级
	2. 测试三级
### 表格
名称|技能|排行
--|:--:|--:
蝙蝠侠|有钱|24
海王|游泳|12
闪电侠|跑步|23
### 代码片段
```c
#include<stdio.h>
int main()
{
	printf("test code\n");
	return 0;
}
```
```cpp
#include<iostream>
```
```python
import <os>
```
```bash
echo"测试"
```
<br>
### 超链接技术

[Github](https://www.github.com)

### 插入图片

[![1.png](https://i.postimg.cc/ZqdBD5Lh/1.png)](https://postimg.cc/XZnYr3h2)
