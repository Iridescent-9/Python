
# 关于配置Python

---

- ## 环境变量

1. 将Python所在文件夹添加至系统PATH，例如

    >D:\Program Files (x86)\Microsoft Visual Studio\Shared\Python37_64

2. 将Python安装路径的*Scripts*文件夹添加至系统PATH，例如

    >D:\Program Files (x86)\Microsoft Visual Studio\Shared\Python37_64\Scripts

3. 将Python依赖包的*Scripts*文件夹添加至系统PATH，例如

    >C:\Users\10362\AppData\Roaming\Python\Python37\Scripts

---

- ## 依赖包

1. *requirements.txt*中存放依赖包列表

    使用`pip freeze > requirements.txt`命令生成*requirements.txt*文件
    每次修改依赖包后都生成一次依赖包列表

2. 安装依赖包

    使用`pip install XXX`进行依赖包的安装，单独这样会很满，使用镜像加速
    >镜像链接
    >><https://mirrors.aliyun.com/pypi/simple/>
    >>
    >><https://pypi.tuna.tsinghua.edu.cn/simple>
    >>
    >><http://pypi.doubanio.com/simple/>
    >>
    >><https://pypi.mirrors.ustc.edu.cn/simple/>

    使用`pip install XXX -i https://pypi.tuna.tsinghua.edu.cn/simple`进行镜像加速安装

    使用`pip install -r requirements.txt -i https://pypi.tuna.tsinghua.edu.cn/simple`从*requirements.txt*中批量安装依赖包
