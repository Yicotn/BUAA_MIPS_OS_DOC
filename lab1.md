#OS-lab1实验报告
##一、实验思考题
####1.1
各指令的作用如下：  
**ls -l**:	按列表显示出文件的详细信息  
**mv test1.c test2.c**:	将test1.c更名为test2.c  
**cp test1.c test2.c**:	新建test1.c的拷贝test2.c  
**cd ..**:	返回上一层
####1.2
grep指令后跟一个正则表达式，将会搜索文本并打印出来匹配的行。  
要查找项目中所有的宏，可以输入grep -r "#define" dir,dir是项目所在的目录  
要查找指定的函数名func可以输入grep -r "func" dir
####1.3
gcc的-Werror参数会把所有waring当成error，也就是说只要有waring就无法顺利通过编译，这样对程序的正确性要求很高，可以避免一些不构成error的错误。  
-Wall参数会把所有的waring打印出来，方便程序员查看自己的程序有什么waring。
####2.1
1.输入git checkout printf.c来恢复之前add过的printf.c  
2.输入git reset HEAD printf.c，然后再输入git checkout printf.c将之前提交过的printf.c恢复回来  
3.输入git rm --cached Tucao.txt
####2.2
1.正确，整个库都会被克隆。  
2.正确，这些操作都只访问或修改本地仓库。  
3.错误，整个库都会被克隆。  
4.正确。
##二、实验难点图示
![难点图示](./src/g1.jpeg)
##三、体会与感想
这次的实验毕竟是第一次，还是比较简单的，主要是学习git和vim的操作花了较长时间，不过刚开始看的时候还是比较懵，很多东西都不熟悉，不知道该怎么写，会花很多时间去纠结，尤其是exercise2.3中要跳转到main函数时纠结了很久main函数的地址是多少。不过熟悉了之后要完成任务还是很快的。

##四、残留难点
对makefile的细节还不是很熟悉。