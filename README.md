# CSAPP
Learning CSAPP ing

# DataLab
## 准备环境
下载Win10下的WSL，Win10商店内就有Ubuntu供下载，需要安装相应的C/C++环境，详情百度

通过VS Code的终端进行代码的修改和调试，在终端敲入bash即可跳转至WSL下
## 实验问题
实验中用make btest之后会报如下错误

	-bash: ./btest: cannot execute binary file: Exec format error
	
在博客上找到了解决问题，即修改Makefile文件中的参数，以64位机器运行即可

	CFLAGS = -O -Wall -m64 #只要修改这行，将-m32换成-m64即可

## 关于实验
##### 测试要求
进行查询是否超出实验要求的运算符或非法字符等

	unix> ./dlc bits.c

##### 运行调试
通过makefile进行编译

	unix> make btest
	unix> ./btest

##### 题解
详情题解或分析在该lab目录下bits.c中，有部分搬运。且自身的代码并非最优解，仅作参考。
