# Github

## 关键字查询
	awesome   去此标签类别中查询项目

	tutorial  查询资料、书籍、文档
	
	sample    查询对应技术的代码样本

## github三要素
### repository仓库
	仓库是github项目管理存储基本单位

	一个仓库中存储一个项目，一个用户可以拥有多个仓库，一般仓库分为public、private

### commit提交
	程序员在整个开发周期，有大量的代码资源的迭代和修改，都可以通过commit的方式进行记录，便于程序员回溯代码，即使这些代码被删除

### 分支
	在仓库中可以包含多个分支，这些分支才是代码文件的第一存储单位，默认的仓库分支为master/main
	*不仅可以管理代码存储，便于多人协作开发
[![1.png](https://i.postimg.cc/brgbdmqg/1.png)](https://postimg.cc/q6tg5Xh6)

## 仓库内容
	code: 资源存储 代码资源、二进制、项目管理脚本、许可证等等

	issues: 使用时遇到的bug进行提交，等待反馈

	README：使用markdown语言编写，工程自述文件、开发进度、版本更新、使用介绍等等

	LICENSE: 许可证

		GPL 2.0 3.0、Apache 2.0、Mit  这些许可证给使用者最大使用权限和最少的限制

# Git软件，分布式版本控制系统
	仓库管理软件，使用git管理私人代码或企业代码
[![2.png](https://i.postimg.cc/WzdFbTfN/2.png)](https://postimg.cc/K3yv0S2w)

## 设备认证
1. 如何让网站的账户与设备绑定，后续完成代码的管理、上传下载
   * git init  *//创建本地仓库*
   * git config --list *//查看git的配置文件*
   * git config --global user.email "邮箱"
   * git config --global user.name "用户名"
   * ssh-keygen -t rsa -C "注册邮箱" *//创建本地文本*
 
2. 为目标仓库起别名，定位目标仓库，后续上传
   * git remote add origin "ssh地址"  *//为ssh仓库地址创建别名为origin*
   * git remote remove origin  *//删除origin别名*

## 本地设备与云端仓库的交互逻辑
[![3.png](https://i.postimg.cc/kg2m1DRX/3.png)](https://postimg.cc/k2PzDJyk)
	git add      //添加内容

	git rm	     //删除本地文件并删除仓库数据

	git restore  //回复被删除的文件（仓库存在）


## 代码更新的依赖关系被破坏
	本地内容要比云端新，完成更新替换，但是如果直接修改云端内容，会导致本地内容无法再次提交
<br>	先拉取 git pull 云端内容，与本地内容合并或操作，然后再次推即可
<br>	
* git pull --rebase origin master  *//拉回到本地master仓库*
* git rebase --skip  *//忽略本地内容  保留云端内容  更新本地后可以上传*
* git rebase --abort  *//忽略云端内容  保留本地内容  此时不能上传*
* git rebase --continue  *//合并内容  解决冲突后可直接上传*

# 分支Branch
	关于分支的相关命令，创建分支、选择分支、合并分支等

# markdown语言

## 标题修饰符\#
* \# 一级标题
* \#\# 二级标题
* \#\#\# 三级标题

## 正文内容
	可以直接输入正文内容，但是如果需要换行，用<br>标签或者空行

## 修饰正文
* \*内容\* 斜体 *测试文本*
* \*\*内容\*\* 粗体 **测试文本**
* \*\*\*内容\*\*\* 粗斜体 ***测试文本***
## 分割线
	用\-\-\-表示分割线
---
## 引用效果

