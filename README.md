# CSAPP
Learning CSAPP ing

# DataLab
环境为Win10下的WSL，需要安装相应的C++环境，详情百度
通过VS Code的终端进行代码的修改和调试

实验中用make btest之后会报如下错误
	-bash: ./btest: cannot execute binary file: Exec format error
在他人的博客上找到了解决问题，即修改Makefile文件中的参数，以64位机器运行即可
	CFLAGS = -O -Wall -m64 # 只要修改这行，将-m32换成-m64即可

详情题解或分析在该lab目录下bits.c中，有部分搬运。且自身的代码并非最优解，仅作参考。