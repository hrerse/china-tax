读取文件使用python内置方法open()打开文件，使用.read()读取全部内容，示例如下：

path = "c:\doc\py.txt"
fi = open(path, "r")
print(fi.read())
fi.close()
with语法

with是python2.5引入的自动释放资源的语法模式，确保使用过程中不管是否发生了异常，都会释放资源. 使用with读取文件，是不需要自己手动close的，示例如下：

with open(path) as fi:
    print(fi.read())
逐行读取文件 .read()是读取文件的全部内容，使用.readlines()，示例如下：

with open(path, "r") as fi:
    lines = fi.readlines()
print(len(lines))
open方法的模式

上面的示例可以看出来，open(目录,操作模式)的时候必须指定操作模式，open的操作模式：

读取模式：'r'(默认模式) | 写入模式：'w' | 附加模式：'a'.

python模式是读取，所以"r"可以省略，示例如下：

path = "c:\py.txt"
fi = open(path)
print(fi.read())
fi.close()